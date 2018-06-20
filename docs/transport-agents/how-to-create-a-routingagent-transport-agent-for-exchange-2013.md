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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759241"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="f6689-103">Exchange 2013 RoutingAgent トランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6689-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="f6689-104">Exchange 2013 で使用するカスタム RoutingAgent トランスポート エージェントを作成する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="f6689-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="f6689-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f6689-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="f6689-106">コード スニペット、およびサンプル アプリケーションに関連します。</span><span class="sxs-lookup"><span data-stu-id="f6689-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="f6689-107">Exchange 2013: 帯域幅のログ出力のトランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6689-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="f6689-108">[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)および[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)のクラスは、Exchange Server 2013 メールボックス サーバー上のトランスポート サービスを実行するように設計されたトランスポート エージェントの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="f6689-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="f6689-109">[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスでは、対象の RoutingAgent、トランスポート エージェントのハンドラーを実装する場合があります次の表に記載されているイベントを提供します。</span><span class="sxs-lookup"><span data-stu-id="f6689-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="f6689-110">**表 1 です。RoutingAgent クラスのイベント**</span><span class="sxs-lookup"><span data-stu-id="f6689-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="f6689-111">**�C�x���g**</span><span class="sxs-lookup"><span data-stu-id="f6689-111">**Event**</span></span>|<span data-ttu-id="f6689-112">**���**</span><span class="sxs-lookup"><span data-stu-id="f6689-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6689-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="f6689-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="f6689-114">サーバーがコンテンツの変換を実行した後に発生します (コンテンツの変換が必要な場合)。</span><span class="sxs-lookup"><span data-stu-id="f6689-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="f6689-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="f6689-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="f6689-116">メッセージのすべての受信者の解決後、ルーティングが決定する前に発生します。</span><span class="sxs-lookup"><span data-stu-id="f6689-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="f6689-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="f6689-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="f6689-118">必要な場合は、サーバーが次ホップにメッセージをルーティングし、コンテンツの変換を実行した後に発生します。</span><span class="sxs-lookup"><span data-stu-id="f6689-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="f6689-119">サーバーはサーバーは、必要なコンテンツ変換を実行し、メッセージのルートの次ホップを決定するために、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントよりも[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント内の各メッセージを処理するのにはより多くのリソースを使用する場合があります。前に[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)イベント ハンドラーにコードを実行します。</span><span class="sxs-lookup"><span data-stu-id="f6689-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="f6689-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="f6689-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="f6689-121">送信キューからメッセージが作成された後に発生します。</span><span class="sxs-lookup"><span data-stu-id="f6689-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="f6689-122">[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)イベントは、RoutingAgent トランスポート エージェントがコンテンツの変換、受信者の解決、またはルーティングのデータを必要としない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="f6689-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="f6689-123">カスタム RoutingAgent トランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="f6689-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="f6689-124">次に示す手順では、カスタムの RoutingAgent トランスポート エージェントを作成する方法について説明しています。 </span><span class="sxs-lookup"><span data-stu-id="f6689-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="f6689-125">トランスポート エージェントを作成するには</span><span class="sxs-lookup"><span data-stu-id="f6689-125">To create the transport agent</span></span>

1. <span data-ttu-id="f6689-126">名前空間に参照を追加します。</span><span class="sxs-lookup"><span data-stu-id="f6689-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="f6689-127">Exchange サーバーでこれらの名前空間を検索できます。</span><span class="sxs-lookup"><span data-stu-id="f6689-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="f6689-128">これらの名前空間への参照を追加すると、する必要がある[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)のメンバーへのアクセスも、他のクラスで使用されている、 [Exchange 2013: 帯域幅のログ出力のトランスポート エージェントをビルド](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)のサンプルです。</span><span class="sxs-lookup"><span data-stu-id="f6689-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="f6689-129">[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスの派生クラスを実装します。</span><span class="sxs-lookup"><span data-stu-id="f6689-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="f6689-130">このコードは、派生クラスのインスタンスを作成し、新しいカスタム ・ エージェントのインスタンスを作成する**CreateAgent**メソッドをオーバーライドします。</span><span class="sxs-lookup"><span data-stu-id="f6689-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="f6689-131">**閉じる**などの他のメソッドは、カスタム コードを実行するには、このクラスでもオーバーライドできます。</span><span class="sxs-lookup"><span data-stu-id="f6689-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="f6689-132">エージェントを定義します。</span><span class="sxs-lookup"><span data-stu-id="f6689-132">Define your agent.</span></span>
    
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

   <span data-ttu-id="f6689-133">エージェント クラスを定義した後は独自の機能を追加することができます。</span><span class="sxs-lookup"><span data-stu-id="f6689-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="f6689-134">この例では、 [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx)と[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)の 2 つのイベントは、カスタム イベント ハンドラーにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="f6689-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="f6689-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6689-135">See also</span></span>

- [<span data-ttu-id="f6689-136">トランスポート エージェントの概念には、Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6689-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="f6689-137">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="f6689-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="f6689-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="f6689-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="f6689-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="f6689-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

