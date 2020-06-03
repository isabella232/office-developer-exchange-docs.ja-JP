---
title: Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Exchange 2013 で使用するカスタムの DeliveryAgent トランスポートエージェントを作成する方法について説明します。
ms.openlocfilehash: b349f0b6d835ba3d6195b43e80d1dcd21750bf82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527573"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="5bc62-103">Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成</span><span class="sxs-lookup"><span data-stu-id="5bc62-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="5bc62-104">Exchange 2013 で使用するカスタムの DeliveryAgent トランスポートエージェントを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="5bc62-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5bc62-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="5bc62-106">[Deliveryagentfactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)および[Deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスは、Exchange Server 2013 メールボックスサーバー上のトランスポートサービス上で実行するように設計されたトランスポートエージェントの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="5bc62-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) and [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="5bc62-107">次の表に、 [deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスによって提供されるイベントについて、deliveryagent トランスポートエージェントのハンドラーを実装することができます。</span><span class="sxs-lookup"><span data-stu-id="5bc62-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="5bc62-108">**表1DeliveryAgent クラスのイベント**</span><span class="sxs-lookup"><span data-stu-id="5bc62-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="5bc62-109">**イベント**</span><span class="sxs-lookup"><span data-stu-id="5bc62-109">**Event**</span></span>|<span data-ttu-id="5bc62-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bc62-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5bc62-111">[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="5bc62-111">[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="5bc62-112">最後のメール アイテムが配信され、接続が閉じられた後に発生します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|<span data-ttu-id="5bc62-113">[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="5bc62-113">[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="5bc62-114">メール アイテムの配信準備が整ったときに発生します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|<span data-ttu-id="5bc62-115">[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="5bc62-115">[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="5bc62-116">配信エージェントが、メール配信のために起動されたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="5bc62-117">カスタム DeliveryAgent トランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="5bc62-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="5bc62-118">次に示す手順では、カスタムの DeliveryAgent トランスポート エージェントを作成する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="5bc62-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="5bc62-119">トランスポート エージェントを作成するには</span><span class="sxs-lookup"><span data-stu-id="5bc62-119">To create the transport agent</span></span>

1. <span data-ttu-id="5bc62-120">名前空間に参照を追加します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="5bc62-121">該当する名前空間は、Exchange サーバーで見つかります。</span><span class="sxs-lookup"><span data-stu-id="5bc62-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="5bc62-122">これらの名前空間への参照を追加すると、 [Deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)メンバーにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="5bc62-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) members.</span></span> 
    
2. <span data-ttu-id="5bc62-123">[Deliveryagentfactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)クラスの派生クラスを実装します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) class.</span></span> 
    
   ```cs
      public class MyDeliveryAgentFactory : DeliveryAgentFactory<MyDeliveryAgentFactory.MyDeliveryAgentManager>
      {
          static MyDeliveryAgentFactory()
          {
          }
          public override DeliveryAgent CreateAgent(SmtpServer server)
          {
              return new MyDeliveryAgent(server);
          }
          public sealed class MyDeliveryAgentManager : DeliveryAgentManager
          {
              /// <summary>
              /// Gets the supported delivery protocol.
              /// </summary>
              public override string SupportedDeliveryProtocol
              {
                  get { return "MyProtocol"; }
              }
          }
      }
  
   ```

   <span data-ttu-id="5bc62-124">このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。</span><span class="sxs-lookup"><span data-stu-id="5bc62-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="5bc62-125">このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。</span><span class="sxs-lookup"><span data-stu-id="5bc62-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="5bc62-126">[Deliveryagentmanager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)クラスは、 [supporteddeliveryprotocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx)プロパティを上書きし、エージェントが使用するプロトコルを設定するために作成されます。</span><span class="sxs-lookup"><span data-stu-id="5bc62-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="5bc62-127">エージェントを定義します。</span><span class="sxs-lookup"><span data-stu-id="5bc62-127">Define your agent.</span></span>
    
   ```cs
      public class MyDeliveryAgent : DeliveryAgent
      {
          public MyDeliveryAgent(SmtpServer server)
          {
              this.OnCloseConnection += CloseConnection;
              this.OnDeliverMailItem += DeliverMailItem;
              this.OnOpenConnection += OpenConnection;
          }
      }
  
   ```

   <span data-ttu-id="5bc62-128">独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。</span><span class="sxs-lookup"><span data-stu-id="5bc62-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="5bc62-129">この例では、3つの events、 [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)、 [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)、 [onopenconnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)がカスタムイベントハンドラーにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="5bc62-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx), and [OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="5bc62-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5bc62-130">See also</span></span>

- [<span data-ttu-id="5bc62-131">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="5bc62-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="5bc62-132">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="5bc62-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)          

 