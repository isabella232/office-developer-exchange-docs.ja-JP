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
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。

Exchange 2013 で使用するカスタム DeliveryAgent トランスポート エージェントを作成する方法を確認します。
  
**に適用されます:** Exchange Server 2013
  
[DeliveryAgentFactory\<マネージャー\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) 、 [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスは、Exchange Server 2013 メールボックス サーバーのトランスポート サービスを実行するように設計されたトランスポート エージェントの基本クラスです。 DeliveryAgent トランスポート エージェントの次の表に記載されている[DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)クラスによって提供されるイベントのハンドラーを実装する場合があります。 
  
**表 1 です。DeliveryAgent クラスのイベント**

|**イベント**|**説明**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |最後のメール アイテムが配信され、接続が閉じられた後に発生します。  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |メール アイテムの配信準備が整ったときに発生します。  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |配信エージェントが、メール配信のために起動されたときに発生します。  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>カスタム DeliveryAgent トランスポート エージェントの作成

次に示す手順では、カスタムの DeliveryAgent トランスポート エージェントを作成する方法について説明しています。  
  
### <a name="to-create-the-transport-agent"></a>トランスポート エージェントを作成するには

1. 名前空間に参照を追加します。
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Exchange サーバーでこれらの名前空間を検索できます。 これらの名前空間への参照を追加すると、 [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx)メンバーへのアクセスがあります。 
    
2. 派生クラスの実装、 [DeliveryAgentFactory\<マネージャー\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx)クラス。 
    
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

   このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。 **閉じる**などの他のメソッドは、カスタム コードを実行するには、このクラスでもオーバーライドできます。 [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx)プロパティをオーバーライドし、エージェントが使用するプロトコルを設定するには、 [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)クラスが作成されます。 
    
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

   エージェント クラスを定義した後は独自の機能を追加することができます。 この例を 3 つのイベント、 [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)、 [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)、および[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)は、カスタム イベント ハンドラーにリダイレクトされます。 
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)          

 