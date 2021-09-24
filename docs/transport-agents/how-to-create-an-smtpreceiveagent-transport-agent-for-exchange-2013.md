---
title: 2013 年の SmtpReceiveAgent トランスポート エージェントExchangeする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: 2013 で使用するカスタム SmtpReceiveAgent トランスポート エージェントを作成するExchangeします。
ms.openlocfilehash: a441f93113798c10421e9073e266c28fd87bca8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513032"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>2013 年の SmtpReceiveAgent トランスポート エージェントExchangeする

2013 で使用するカスタム SmtpReceiveAgent トランスポート エージェントを作成するExchangeします。
  
**製品:** Exchange Server 2013
  
関連するコード スニペットとサンプル アプリ:

- [Exchange 2013: 本文変換トランスポート エージェントを作成する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)クラスと[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスを使用すると、クライアント アクセス サーバー上のフロントエンド トランスポート サービスまたはメールボックス サーバー上のトランスポート サービスの動作を拡張できます。 これらのクラスを使用して、組織に到着したメッセージに応答するように設計されたトランスポート エージェントを実装できます。 
  
[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)クラスと[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスには、次の表に示すイベントが含まれます。 
  
**表 1.SmtpReceiveAgent クラス イベント**

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

   これらの名前空間は、2013 Exchangeで確認できます。 これらの名前空間への参照を追加すると[、smtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)メンバー、および[Exchange 2013:](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)ビルドの本文変換トランスポート エージェント サンプルで使用される他のクラスにアクセスできます。 
    
2. [SmtpReceiveAgentFactory クラスの派生クラスを実装](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)します。 
    
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

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では [、OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) イベントがカスタム イベント ハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

