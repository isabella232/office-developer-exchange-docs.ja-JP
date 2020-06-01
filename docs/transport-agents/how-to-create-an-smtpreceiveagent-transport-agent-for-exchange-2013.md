---
title: Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Exchange 2013 で使用する、カスタムの SmtpReceiveAgent トランスポートエージェントを作成する方法について説明します。
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459140"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する

Exchange 2013 で使用する、カスタムの SmtpReceiveAgent トランスポートエージェントを作成する方法について説明します。
  
**製品:** Exchange Server 2013
  
関連するコードスニペットとサンプルアプリ:

- [Exchange 2013: 本文変換トランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスを使用すると、メールボックスサーバー上のクライアントアクセスサーバーまたはトランスポートサービス上のフロントエンドトランスポートサービスの動作を拡張することができます。 これらのクラスを使用して、組織に到着したメッセージに応答するように設計されたトランスポート エージェントを実装できます。 
  
[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスには、次の表に示すイベントが含まれています。 
  
**表1SmtpReceiveAgent クラスのイベント**

|**イベント**|**説明**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |どの種類の認証方法が使用されたかによって、メッセージ配信の試行を拒否または承認するエージェントなど、SMTP **AUTH** コマンドでのみ得られる情報を必要とするエージェントで使用します。  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |リモート SMTP サーバーのアドレスまたはドメインに基づいてアクションを実行するエージェントなど、フロント エンド トランスポート サービスへの SMTP による接続が開いているときにのみ得られる情報を必要とするエージェントで使用します。  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |このイベントは、SMTP **DATA** コマンドで得られる情報を必要とするエージェントで使用します。  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |時間の計算を実行するために、切断時に得られる現在の時刻と日付などの情報を必要とするエージェントで使用します。  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |SMTP **EHLO** コマンドで得られる情報を必要とするエージェントで使用します。たとえば、**EHLO** コマンドで得られる ID に基づいて、エージェントによってメッセージを承認または拒否する場合に使用します。  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |リモート サーバーが認証プロセスを完了したときに得られる情報を必要とするエージェントで使用します。たとえば、リモートの SMTP サーバーやクライアントから得られる認証情報に基づいてメッセージにアクションを実行するエージェントで使用します。  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |メッセージから得られるデータに基づいてアクションを実行する必要のあるエージェントで使用します。このイベントは、フロント エンド トランスポート サービスでは発生しません。このイベントをトランスポート エージェントで使用する必要がある場合は、そのエージェントをメールボックス サーバーにインストールする必要があります。  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |送信したメッセージのヘッダーから得られる情報に基づいてアクションを実行する必要のあるエージェントで使用します。  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>カスタム SmtpReceiveAgent トランスポート エージェントの作成

次に示す手順では、カスタムの SmtpReceiveAgent トランスポート エージェントを作成する方法について説明しています。 
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   これらの名前空間は、Exchange 2013 サーバーで見つけることができます。 これらの名前空間への参照を追加すると、 [Smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)メンバーだけでなく、Exchange 2013 で使用されている他のクラスにもアクセスできるようになります。[本文変換トランスポートエージェント](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)サンプルを作成します。 
    
2. [Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)クラスの派生クラスを実装します。 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。 
    
3. エージェントを定義します。
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では、 [Onendofdata](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)イベントがカスタムイベントハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

