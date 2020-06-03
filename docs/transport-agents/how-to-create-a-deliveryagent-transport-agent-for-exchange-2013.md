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
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成

Exchange 2013 で使用するカスタムの DeliveryAgent トランスポートエージェントを作成する方法について説明します。
  
**製品:** Exchange Server 2013
  
[Deliveryagentfactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)および[Deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスは、Exchange Server 2013 メールボックスサーバー上のトランスポートサービス上で実行するように設計されたトランスポートエージェントの基本クラスです。 次の表に、 [deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスによって提供されるイベントについて、deliveryagent トランスポートエージェントのハンドラーを実装することができます。 
  
**表1DeliveryAgent クラスのイベント**

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

   該当する名前空間は、Exchange サーバーで見つかります。 これらの名前空間への参照を追加すると、 [Deliveryagent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)メンバーにアクセスできるようになります。 
    
2. [Deliveryagentfactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx)クラスの派生クラスを実装します。 
    
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

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。 このクラスの別のメソッド (**Close** など) も、カスタム コードを実行するようにオーバーライドできます。 [Deliveryagentmanager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)クラスは、 [supporteddeliveryprotocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx)プロパティを上書きし、エージェントが使用するプロトコルを設定するために作成されます。 
    
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

   独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。 この例では、3つの events、 [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)、 [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)、 [onopenconnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)がカスタムイベントハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)          

 