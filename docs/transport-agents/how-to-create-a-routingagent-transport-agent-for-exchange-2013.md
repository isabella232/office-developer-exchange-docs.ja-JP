---
title: 2013 年の RoutingAgent トランスポート エージェントExchangeする
manager: sethgros
ms.date: 09/21/2021
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: 2013 で使用するカスタム RoutingAgent トランスポート エージェントを作成するExchangeします。
ms.openlocfilehash: 89c70e7d021b9b2cc46f65ee3bbff334430fecc7
ms.sourcegitcommit: f13a3a4a61fa23ca6414b7c96ddf087adbe3dc9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2021
ms.locfileid: "60262212"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>2013 年の RoutingAgent トランスポート エージェントExchangeする

2013 で使用するカスタム RoutingAgent トランスポート エージェントを作成するExchangeします。
  
**製品:** Exchange Server 2013
  
関連するコード スニペットとサンプル アプリ:

- [Exchange 2013: 帯域幅ログ トランスポート エージェントの作成](/exchange/client-developer/transport-agents/transport-agent-code-samples-for-exchange-2013.md)
  
[RoutingAgentFactory](https://docs.microsoft.com/previous-versions/office/exchange-server-api/aa564164(v=exchg.150))クラスと[RoutingAgent](https://docs.microsoft.com/previous-versions/office/exchange-server-api/aa564421(v=exchg.150))クラスは、2013 メールボックス サーバー上のトランスポート サービスで実行するように設計されたトランスポート エージェントの基本クラスExchange Serverです。 [RoutingAgent クラスは](https://docs.microsoft.com/previous-versions/office/exchange-server-api/aa564421(v=exchg.150))、RoutingAgent トランスポート エージェントにハンドラーを実装する可能性があるイベントを次の表に示します。 
  
**表 1.RoutingAgent クラス イベント**

|**イベント**|**説明**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |サーバーがコンテンツの変換を実行した後に発生します (コンテンツの変換が必要な場合)。  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |メッセージのすべての受信者の解決後、ルーティングが決定する前に発生します。  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |サーバーがメッセージを次ホップにルーティングし、必要に応じてコンテンツ変換を実行した後に発生します。 サーバーは[、OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント ハンドラーでコードを実行する前に、必要なコンテンツ変換を実行し、メッセージのルート内の次ホップを決定するために[、OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント内の各メッセージを[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントよりも多くのリソースで処理する場合があります。  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |メッセージが送信キューから取り出されたときに発生します。 RoutingAgent トランスポート エージェントがコンテンツ変換、解決済み受信者、またはルーティング データを必要としない場合は [、OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) イベントを使用します。  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>カスタム RoutingAgent トランスポート エージェントの作成

次に示す手順では、カスタムの RoutingAgent トランスポート エージェントを作成する方法について説明しています。 
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   該当する名前空間は、Exchange サーバーで見つかります。 これらの名前空間への参照を追加すると[、RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)メンバーと[、Exchange 2013:](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)ビルドの帯域幅ログ トランスポート エージェント サンプルで使用される他のクラスにアクセスできます。 
    
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

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。 
    
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

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では [、OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) と [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)の 2 つのイベントがカスタム イベント ハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

