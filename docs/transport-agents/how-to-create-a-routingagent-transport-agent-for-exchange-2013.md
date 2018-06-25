---
title: Exchange 2013 RoutingAgent トランスポート エージェントを作成します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Exchange 2013 で使用するカスタム RoutingAgent トランスポート エージェントを作成する方法を確認します。
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759241"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Exchange 2013 RoutingAgent トランスポート エージェントを作成します。

Exchange 2013 で使用するカスタム RoutingAgent トランスポート エージェントを作成する方法を確認します。
  
**に適用されます:** Exchange Server 2013
  
コード スニペット、およびサンプル アプリケーションに関連します。

- [Exchange 2013: 帯域幅のログ出力のトランスポート エージェントを作成します。](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)および[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)のクラスは、Exchange Server 2013 メールボックス サーバー上のトランスポート サービスを実行するように設計されたトランスポート エージェントの基本クラスです。 [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスでは、対象の RoutingAgent、トランスポート エージェントのハンドラーを実装する場合があります次の表に記載されているイベントを提供します。 
  
**表 1 です。RoutingAgent クラスのイベント**

|**�C�x���g**|**���**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |サーバーがコンテンツの変換を実行した後に発生します (コンテンツの変換が必要な場合)。  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |メッセージのすべての受信者の解決後、ルーティングが決定する前に発生します。  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |必要な場合は、サーバーが次ホップにメッセージをルーティングし、コンテンツの変換を実行した後に発生します。 サーバーはサーバーは、必要なコンテンツ変換を実行し、メッセージのルートの次ホップを決定するために、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントよりも[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント内の各メッセージを処理するのにはより多くのリソースを使用する場合があります。前に[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント ハンドラーにコードを実行します。  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |送信キューからメッセージが作成された後に発生します。 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントは、RoutingAgent トランスポート エージェントがコンテンツの変換、受信者の解決、またはルーティングのデータを必要としない場合に使用します。  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>カスタム RoutingAgent トランスポート エージェントの作成

次に示す手順では、カスタムの RoutingAgent トランスポート エージェントを作成する方法について説明しています。  
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Exchange サーバーでこれらの名前空間を検索できます。 これらの名前空間への参照を追加すると、する必要がある[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)のメンバーへのアクセスも、他のクラスで使用されている、 [Exchange 2013: 帯域幅のログ出力のトランスポート エージェントをビルド](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)のサンプルです。 
    
2. [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスの派生クラスを実装します。 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   このコードは、派生クラスのインスタンスを作成し、新しいカスタム ・ エージェントのインスタンスを作成する**CreateAgent**メソッドをオーバーライドします。 **閉じる**などの他のメソッドは、カスタム コードを実行するには、このクラスでもオーバーライドできます。 
    
3. エージェントを定義します。
    
   ```cs
      public class BandwidthLogger : RoutingAgent
      {
          // Your custom code goes here
          public BandwidthLogger(SmtpServer server)
          {
              Debug.WriteLine(logPrefix + "Agent constructor");
              this.server = server;
              this.OnSubmittedMessage += SubmittedMessage;
              this.OnRoutedMessage += RoutedMessage;
          }
      }
  
   ```

   エージェント クラスを定義した後は独自の機能を追加することができます。 この例では、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)と[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)の 2 つのイベントは、カスタム イベント ハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

