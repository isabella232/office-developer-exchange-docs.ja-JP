---
title: Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Exchange 2013 で使用するカスタム DeliveryAgent トランスポート エージェントを作成する方法を確認します。
ms.openlocfilehash: bc36c7b5e0fb8006c5927d423d7767dcc7382ce0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353309"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="88af2-103">Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="88af2-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="88af2-104">Exchange 2013 で使用するカスタム DeliveryAgent トランスポート エージェントを作成する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="88af2-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="88af2-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="88af2-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="88af2-106">[DeliveryAgentFactory\<マネージャー\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) 、 [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスは、Exchange Server 2013 メールボックス サーバーのトランスポート サービスを実行するように設計されたトランスポート エージェントの基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="88af2-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) and [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="88af2-107">DeliveryAgent トランスポート エージェントの次の表に記載されている[DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスによって提供されるイベントのハンドラーを実装する場合があります。</span><span class="sxs-lookup"><span data-stu-id="88af2-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="88af2-108">**表 1 です。DeliveryAgent クラスのイベント**</span><span class="sxs-lookup"><span data-stu-id="88af2-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="88af2-109">**イベント**</span><span class="sxs-lookup"><span data-stu-id="88af2-109">**Event**</span></span>|<span data-ttu-id="88af2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="88af2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88af2-111">[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="88af2-111">[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="88af2-112">最後のメール アイテムが配信され、接続が閉じられた後に発生します。</span><span class="sxs-lookup"><span data-stu-id="88af2-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|<span data-ttu-id="88af2-113">[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="88af2-113">[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="88af2-114">メール アイテムの配信準備が整ったときに発生します。</span><span class="sxs-lookup"><span data-stu-id="88af2-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|<span data-ttu-id="88af2-115">[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="88af2-115">[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="88af2-116">配信エージェントが、メール配信のために起動されたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="88af2-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="88af2-117">カスタム DeliveryAgent トランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="88af2-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="88af2-118">次に示す手順では、カスタムの DeliveryAgent トランスポート エージェントを作成する方法について説明しています。 </span><span class="sxs-lookup"><span data-stu-id="88af2-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="88af2-119">トランスポート エージェントを作成するには</span><span class="sxs-lookup"><span data-stu-id="88af2-119">To create the transport agent</span></span>

1. <span data-ttu-id="88af2-120">名前空間に参照を追加します。</span><span class="sxs-lookup"><span data-stu-id="88af2-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="88af2-121">Exchange サーバーでこれらの名前空間を検索できます。</span><span class="sxs-lookup"><span data-stu-id="88af2-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="88af2-122">これらの名前空間への参照を追加すると、 [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)メンバーへのアクセスがあります。</span><span class="sxs-lookup"><span data-stu-id="88af2-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) members.</span></span> 
    
2. <span data-ttu-id="88af2-123">派生クラスの実装、 [DeliveryAgentFactory\<マネージャー\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx)クラス。</span><span class="sxs-lookup"><span data-stu-id="88af2-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) class.</span></span> 
    
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

   <span data-ttu-id="88af2-124">このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。</span><span class="sxs-lookup"><span data-stu-id="88af2-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="88af2-125">**閉じる**などの他のメソッドは、カスタム コードを実行するには、このクラスでもオーバーライドできます。</span><span class="sxs-lookup"><span data-stu-id="88af2-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="88af2-126">[SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx)プロパティをオーバーライドし、エージェントが使用するプロトコルを設定するには、 [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)クラスが作成されます。</span><span class="sxs-lookup"><span data-stu-id="88af2-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="88af2-127">エージェントを定義します。</span><span class="sxs-lookup"><span data-stu-id="88af2-127">Define your agent.</span></span>
    
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

   <span data-ttu-id="88af2-128">エージェント クラスを定義した後は独自の機能を追加することができます。</span><span class="sxs-lookup"><span data-stu-id="88af2-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="88af2-129">この例を 3 つのイベント、 [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)、 [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)、および[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)は、カスタム イベント ハンドラーにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="88af2-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx), and [OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="88af2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="88af2-130">See also</span></span>

- [<span data-ttu-id="88af2-131">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="88af2-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="88af2-132">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="88af2-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)          

 