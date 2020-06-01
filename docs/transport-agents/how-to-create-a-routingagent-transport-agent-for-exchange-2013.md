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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463700"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="21273-103">Exchange 2013 用の RoutingAgent トランスポートエージェントの作成</span><span class="sxs-lookup"><span data-stu-id="21273-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="21273-104">Exchange 2013 で使用するカスタムの RoutingAgent トランスポートエージェントを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="21273-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="21273-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="21273-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="21273-106">関連するコードスニペットとサンプルアプリ:</span><span class="sxs-lookup"><span data-stu-id="21273-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="21273-107">Exchange 2013: 帯域幅ログトランスポートエージェントを構築する</span><span class="sxs-lookup"><span data-stu-id="21273-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="21273-108">[Routingagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスと[routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスは、Exchange Server 2013 メールボックスサーバー上のトランスポートサービス上で実行するように設計されたトランスポートエージェントの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="21273-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="21273-109">[Routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスには、次の表に示されているイベントがあります。これには、routingagent トランスポートエージェントでハンドラーを実装することができます。</span><span class="sxs-lookup"><span data-stu-id="21273-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="21273-110">**表1RoutingAgent クラスのイベント**</span><span class="sxs-lookup"><span data-stu-id="21273-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="21273-111">**イベント**</span><span class="sxs-lookup"><span data-stu-id="21273-111">**Event**</span></span>|<span data-ttu-id="21273-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="21273-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21273-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="21273-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="21273-114">サーバーがコンテンツの変換を実行した後に発生します (コンテンツの変換が必要な場合)。</span><span class="sxs-lookup"><span data-stu-id="21273-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="21273-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="21273-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="21273-116">メッセージのすべての受信者の解決後、ルーティングが決定する前に発生します。</span><span class="sxs-lookup"><span data-stu-id="21273-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="21273-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="21273-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="21273-118">サーバーがメッセージを次ホップにルーティングし、必要に応じてコンテンツ変換を実行した後に発生します。</span><span class="sxs-lookup"><span data-stu-id="21273-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="21273-119">サーバーは、Onroutedmessage[イベントハンドラー](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)でコードを実行する前に、必要なコンテンツ変換を実行し、メッセージのルート内の次ホップを決定するので、 [onroutedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) [イベントの](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)各メッセージの処理により多くのリソースが使用される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="21273-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="21273-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="21273-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="21273-121">メッセージが送信キューから取り出されたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="21273-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="21273-122">ルーティングエージェントトランスポートエージェントがコンテンツの変換、解決された受信者、またはルーティングデータを必要としない場合は、 [Onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントを使用します。</span><span class="sxs-lookup"><span data-stu-id="21273-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="21273-123">カスタム RoutingAgent トランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="21273-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="21273-124">次に示す手順では、カスタムの RoutingAgent トランスポート エージェントを作成する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="21273-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="21273-125">トランスポート エージェントを作成するには</span><span class="sxs-lookup"><span data-stu-id="21273-125">To create the transport agent</span></span>

1. <span data-ttu-id="21273-126">名前空間に参照を追加します。</span><span class="sxs-lookup"><span data-stu-id="21273-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="21273-127">該当する名前空間は、Exchange サーバーで見つかります。</span><span class="sxs-lookup"><span data-stu-id="21273-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="21273-128">これらの名前空間への参照を追加することによって、 [routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)メンバーだけでなく、Exchange 2013 で使用される他のクラスにアクセスでき[ます。帯域幅ログトランスポートエージェント](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)サンプルを作成する。</span><span class="sxs-lookup"><span data-stu-id="21273-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="21273-129">[Routingagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスの派生クラスを実装します。</span><span class="sxs-lookup"><span data-stu-id="21273-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="21273-130">このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。</span><span class="sxs-lookup"><span data-stu-id="21273-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="21273-131">このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。</span><span class="sxs-lookup"><span data-stu-id="21273-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="21273-132">エージェントを定義します。</span><span class="sxs-lookup"><span data-stu-id="21273-132">Define your agent.</span></span>
    
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

   <span data-ttu-id="21273-133">独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。</span><span class="sxs-lookup"><span data-stu-id="21273-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="21273-134">この例では、2つのイベント[Onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)と[onsubmittedmessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)がカスタムイベントハンドラーにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="21273-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="21273-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="21273-135">See also</span></span>

- [<span data-ttu-id="21273-136">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="21273-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="21273-137">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="21273-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="21273-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="21273-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="21273-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="21273-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

