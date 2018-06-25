---
title: Exchange 2013 SmtpReceiveAgent トランスポート エージェントを作成します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Exchange 2013 で使用するカスタム SmtpReceiveAgent トランスポート エージェントを作成する方法を確認します。
ms.openlocfilehash: a74d5baae6334c5e17acb6335206964b48f320e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759357"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Exchange 2013 SmtpReceiveAgent トランスポート エージェントを作成します。

Exchange 2013 で使用するカスタム SmtpReceiveAgent トランスポート エージェントを作成する方法を確認します。
  
**に適用されます:** Exchange Server 2013
  
コード スニペット、およびサンプル アプリケーションに関連します。

- [Exchange 2013: 本文の変換のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)と[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスを使用すると、クライアント アクセス サーバーのフロント エンド トランスポート サービスまたはメールボックス サーバー上のトランスポート サービスの動作を拡張できます。 組織になるように、メッセージに応答するのにように設計されたトランスポート エージェントを実装するためにこれらのクラスを使用できます。 
  
[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)のクラスには、次の表に記載されているイベントが含まれます。 
  
**表 1 です。SmtpReceiveAgent クラスのイベント**

|**�C�x���g**|**���**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |受け入れるか拒否するエージェントが使用する認証方法の種類に基づいてメッセージを配信しようとした場合などに、エージェントが SMTP**認証**でのみ提供されている情報を必要とする場合に使用します。  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |リモート SMTP サーバーのアドレスまたはドメインに基づいてアクションを実行するエージェントなど、フロント エンド トランスポート サービスへの SMTP による接続が開いているときにのみ得られる情報を必要とするエージェントで使用します。  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |エージェントは、SMTP**データ**コマンドで提供される情報を必要とする場合は、このイベントを使用します。  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |時間の計算を実行するために、切断時に得られる現在の時刻と日付などの情報を必要とするエージェントで使用します。  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |エージェントは、SMTP **EHLO**コマンドで提供される情報を必要とする場合に使用たとえば、次のように、エージェントを受け入れる、または**EHLO**コマンドで指定された id に基づいて、メッセージを拒否します。  <br/> |
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

   Exchange 2013 サーバーにこれらの名前空間を検索できます。 これらの名前空間への参照を追加するときにする必要がある[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)のメンバーへのアクセスも、他のクラスで使用される、 [Exchange 2013: 本文の変換のトランスポート エージェントをビルド](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)のサンプルです。 
    
2. [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)クラスの派生クラスを実装します。 
    
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

   このコードは、派生クラスのインスタンスを作成し、新しいカスタム ・ エージェントのインスタンスを作成する**CreateAgent**メソッドをオーバーライドします。 
    
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

   エージェント クラスを定義した後、カスタム機能を追加できます。 この例では、 [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)イベントは、カスタム イベント ハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

