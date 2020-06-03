---
title: Exchange 2013 用の RoutingAgent トランスポートエージェントの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Exchange 2013 で使用するカスタムの RoutingAgent トランスポートエージェントを作成する方法について説明します。
ms.openlocfilehash: 9acf30be0dd795098f757effaa34b2e72183b000
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463700"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Exchange 2013 用の RoutingAgent トランスポートエージェントの作成

Exchange 2013 で使用するカスタムの RoutingAgent トランスポートエージェントを作成する方法について説明します。
  
**製品:** Exchange Server 2013
  
関連するコードスニペットとサンプルアプリ:

- [Exchange 2013: 帯域幅ログトランスポートエージェントを構築する](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
[Routingagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスと[routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスは、Exchange Server 2013 メールボックスサーバー上のトランスポートサービス上で実行するように設計されたトランスポートエージェントの基本クラスです。 [Routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスには、次の表に示されているイベントがあります。これには、routingagent トランスポートエージェントでハンドラーを実装することができます。 
  
**表1RoutingAgent クラスのイベント**

|**イベント**|**説明**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |サーバーがコンテンツの変換を実行した後に発生します (コンテンツの変換が必要な場合)。  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |メッセージのすべての受信者の解決後、ルーティングが決定する前に発生します。  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |サーバーがメッセージを次ホップにルーティングし、必要に応じてコンテンツ変換を実行した後に発生します。 サーバーは、Onroutedmessage[イベントハンドラー](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)でコードを実行する前に、必要なコンテンツ変換を実行し、メッセージのルート内の次ホップを決定するので、 [onroutedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) [イベントの](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)各メッセージの処理により多くのリソースが使用される可能性があります。  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |メッセージが送信キューから取り出されたときに発生します。 ルーティングエージェントトランスポートエージェントがコンテンツの変換、解決された受信者、またはルーティングデータを必要としない場合は、 [Onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントを使用します。  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>カスタム RoutingAgent トランスポート エージェントの作成

次に示す手順では、カスタムの RoutingAgent トランスポート エージェントを作成する方法について説明しています。 
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   該当する名前空間は、Exchange サーバーで見つかります。 これらの名前空間への参照を追加することによって、 [routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)メンバーだけでなく、Exchange 2013 で使用される他のクラスにアクセスでき[ます。帯域幅ログトランスポートエージェント](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)サンプルを作成する。 
    
2. [Routingagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスの派生クラスを実装します。 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。 このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。 
    
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

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では、2つのイベント[Onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)と[onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)がカスタムイベントハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

