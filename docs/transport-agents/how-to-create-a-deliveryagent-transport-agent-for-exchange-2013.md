---
title: 2013 年の DeliveryAgent トランスポート エージェントExchangeする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: 2013 で使用するカスタム DeliveryAgent トランスポート エージェントを作成するExchangeします。
ms.openlocfilehash: b465c3bbd4658bea700d5be9f4eb16ae81693717
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526934"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>2013 年の DeliveryAgent トランスポート エージェントExchangeする

2013 で使用するカスタム DeliveryAgent トランスポート エージェントを作成するExchangeします。
  
**製品:** Exchange Server 2013
  
[DeliveryAgentFactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)クラスと[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスは、2013 メールボックス サーバー上のトランスポート サービスで実行するように設計されたトランスポート エージェントの基本クラスExchange Serverです。 次の表に示す DeliveryAgent クラスによって提供されるイベントに対して [、DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) トランスポート エージェントにハンドラーを実装できます。 
  
**表 1.DeliveryAgent クラスのイベント**

|**イベント**|**説明**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |最後のメール アイテムが配信され、接続が閉じられた後に発生します。  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |メール アイテムの配信準備が整ったときに発生します。  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |配信エージェントが、メール配信のために起動されたときに発生します。  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>カスタム DeliveryAgent トランスポート エージェントの作成

次に示す手順では、カスタムの DeliveryAgent トランスポート エージェントを作成する方法について説明しています。 
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   該当する名前空間は、Exchange サーバーで見つかります。 これらの名前空間への参照を追加すると [、DeliveryAgent メンバーにアクセス](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) できます。 
    
2. [DeliveryAgentFactory クラスの派生クラスを実装 \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)します。 
    
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

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。 このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。 [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)クラスは[、SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx)プロパティをオーバーライドし、エージェントが使用するプロトコルを設定するために作成されます。 
    
3. エージェントを定義します。
    
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

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では、OnCloseConnection、OnDeliverMailItem、OnOpenConnection[](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)の 3 つのイベントがカスタム イベント ハンドラーにリダイレクトされます。 [](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) [](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)          

 