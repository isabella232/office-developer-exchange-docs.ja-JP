---
title: Exchange 2013 におけるトランスポート エージェントの概念
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Exchange 2013 のトランスポートエージェントパイプラインおよびサーバーの役割のアーキテクチャがトランスポートエージェントの開発に及ぼす影響、およびトランスポートエージェントの開発に使用できるクラスについて説明します。
ms.openlocfilehash: b9552ea4398ac8135a11b48eb7e7bdf5ec81985e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527559"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Exchange 2013 におけるトランスポート エージェントの概念

Exchange 2013 のトランスポートエージェントパイプラインおよびサーバーの役割のアーキテクチャがトランスポートエージェントの開発に及ぼす影響、およびトランスポートエージェントの開発に使用できるクラスについて説明します。 
  
**製品:** Exchange Server 2013 
  
Exchange Server 2013 で提供されるクラスライブラリを使用して、イベントを登録し、トランスポートパイプラインを通過するメッセージに対してアクションを実行するトランスポートエージェントを実装できます。 また、メッセージの変更とコンテンツの変換にも、トランスポート エージェントを使用できます。 
  
この記事では、トランスポートエージェントとトランスポートパイプラインのアーキテクチャについて説明します。 トランスポート動作を変更して組織のニーズを満たすことができるように、トランスポートパイプラインのアーキテクチャを理解しておくことが重要です。 この記事では、トランスポートエージェントとトランスポートエージェントの開発に使用できるクラスに影響する Exchange 2013 アーキテクチャの変更についても説明します。 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>トランスポート パイプライン内のトランスポート エージェント
<a name="Pipeline"> </a>

トランスポート エージェントは、次に示す 3 つのクラスのいずれかから派生します。
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
トランスポート パイプラインとは、Exchange 2013 組織の境界内でのメッセージ データの流れのことを意味します。パイプラインは、次の表に示したサービスによって成立します。
  
**表1トランスポートパイプラインサービス**

|**サービス**|**説明**|**サポートされるクラス**|
|:-----|:-----|:-----|
|フロント エンド トランスポート  <br/> |すべての[クライアントアクセスサーバー](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx)上で実行され、Exchange 2013 組織のすべての受信および送信外部 SMTP トラフィックのステートレスプロキシとして機能します。 フロント エンド トランスポート サービスは、メッセージ コンテンツを検査することも、メッセージをローカルにキューに格納することもありません。 [メールボックスサーバー](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx)上のトランスポートサービスと通信します。  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |すべてのメールボックスサーバー上で実行され、Exchange Server 2010 の[ハブトランスポートサーバー](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx)の役割に似ています。 トランスポートサービスは、メールボックストランスポートサービスとフロントエンドトランスポートサービスの間でメッセージをルーティングします。 このサービスは、メールボックスデータベースと直接通信しません。  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|メールボックス トランスポート  <br/> |すべてのメールボックスサーバー上で実行され、メールボックストランスポート発信とメールボックストランスポート配信という2つの個別のサービスで構成されます。 メールボックストランスポート配信は、トランスポートサービスから SMTP メッセージを受信し、Exchange リモートプロシージャコール (RPC) を使用してメッセージを配信することによって、メールボックスデータベースに接続します。 メールボックストランスポート発信は、メッセージを取得するために RPC を使用してメールボックスデータベースに接続し、SMTP を介してトランスポートサービスにメッセージを送信します。  <br/> |なし。  <br/> |
   
### <a name="transport-events"></a>トランスポート イベント
<a name="Events"> </a>

トランスポート エージェントは、まずイベントを登録して、そのイベントが発生したときにアクションを起こすことで実装します。3 種類のそれぞれのエージェントで、異なるイベントのセットを登録できます。
  
次の図は、トランスポート エージェントがトランスポート パイプラインのどの部分でイベントを登録できるかを示しています。
  
**図1。トランスポートイベント**

![トランスポート パイプラインを介したメッセージ フロー、および各エージェントが登録できるイベントを示すイメージ。SmtpReceivedAgent の SMTP イベントから始まり、RoutingAgent の Categorizor イベント、そして最後に DeliveryAgent の配信イベントが続きます。](media/TAConceptsFig1.png)
  
メッセージがトランスポートパイプラインに入ると、 [Smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスから派生したトランスポートエージェントは、エージェントが登録した SMTP イベントの中でメッセージを処理することができます。 [Routingagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスから派生したエージェントは、に登録されている4つのカテゴライザーイベントのいずれかに対して動作できます。 [Deliveryagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)クラスから派生したエージェントは、に登録されている配信イベントのいずれかでメッセージを処理できます。 
  
## <a name="transport-agents-and-server-roles"></a>トランスポート エージェントとサーバーの役割
<a name="ServerRoles"> </a>

Exchange 2013 のサーバーの役割のアーキテクチャに対する変更は、トランスポートエージェントとトランスポートエージェントが実行できることに影響します。 Exchange 2013 には、次のサーバーの役割が含まれています。
  
- メールボックス サーバー: クライアント アクセス プロトコル、トランスポート サービス、メールボックス データベース、ユニファイド メッセージング コンポーネントが含まれます。 メールボックス サーバーは、Active Directory ドメイン サービス (AD DS)、クライアント アクセス サーバー、および Outlook などのメール クライアントと直接通信します。
    
- クライアント アクセス サーバー: 認証、制限付きリダイレクト、プロキシ サービス、およびクライアント アクセス プロトコル (HTTP、POP、IMAP、SMTP など) を提供します。
    
- エッジ トランスポート サーバー: 電子メールを組織の内外にルーティングします。エッジ トランスポート サーバーは、通常、Exchange トポロジの境界に配置されます。
    
この統合構造を使用すると、Exchange 2013 環境に展開する必要があるサーバーの数を減らすことができます。 管理者は、メールボックスサーバーを含むすべての Active Directory サイトにハブトランスポートサーバーとクライアントアクセスサーバーを展開する必要がなくなり、新しい機能を利用するためにすべてのサーバーの役割を更新する必要がなくなりました。
  
このようなサーバーの役割アーキテクチャに対する変更は、カスタムのエージェントがパイプラインのどの部分でイベントに応答できるかに影響を及ぼす可能性があります。 Exchange 2013 よりも前の Exchange の各バージョンに対応したトランスポート エージェントを作成してある場合は、アーキテクチャの変更点を確認して、カスタムのエージェントに変更を加える必要があるかどうかを判断してください。
  
次の図は、Exchange 2013 のアーキテクチャ上の変更点が、どのようにトランスポート パイプラインを合理化および統合化しているかについて示しています。この図では、クライアント アクセス サーバーに「CAS」というラベルが付けられています。また、メールボックス サーバーには「MBX」というラベルが付けられています。
  
**図2Exchange 2013 のサーバーの役割のアーキテクチャ**

![外部のファイアウォールを通過するクライアント トラフィックを示すイメージ。左側にはレイヤー 4 の負荷分散から統合 CAS 配列にトラフィックを渡すエッジ トランスポートがあり、右側にはデータベース アクセシビリティ グループの一連のメールボックス サーバーがあります。](media/Transport_Agent_Concepts_Fig_3.png)
  
次の図は、Exchange 2013 のサーバーの役割間での相互作用を示しています。
  
**図3メールボックスおよびクライアントアクセスサーバーの相互作用**

![CAS に 4 つのターゲット (IIS/HTTP Proxy、POP/IMAP、SMTP、および UM) が存在するレイヤー 4 の負荷分散を通過するクライアント トラフィックから矢印が始まるやり取りを示すイメージ。矢印は、メールボックス ストアのコンプリメンタリ ターゲットを通過します。](media/Transport_Agent_Concepts_Fig_4.png)
  
Exchange 2013 サーバーの役割アーキテクチャの変更の詳細については、「exchange [2013 の新機能](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)」の「 [exchange 2013 アーキテクチャ](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch)」を参照してください。 
  
## <a name="transport-agent-classes"></a>トランスポート エージェントのクラス
<a name="Create"> </a>

カスタムのトランスポート エージェントの派生元クラスにより、そのエージェントで登録できるイベントが決まります。通常、カスタムのエージェントには、1 つのエージェント クラス、1 つのエージェント ファクトリ、1 つ以上のイベント ハンドラー、およびエージェントで処理するアクションを実行するコードが含まれています。
  
次の表は、それぞれのエージェントの種類の派生元になるクラスを示しています。
  
**表2エージェントクラス**

||||
|:-----|:-----|:-----|
|エージェントの種類  <br/> |ファクトリの基底クラス  <br/> |エージェントの基底クラス  <br/> |
|SMTP の受信  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|承認  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Delivery  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
これらのファクトリとエージェントの基底クラスには、トランスポート イベントとメッセージへのアクセスに使用できるプロパティとメソッドが用意されています。カスタムのエージェントには、これらのクラスから継承するクラスを実装します。エージェント ファクトリ派生クラスでは、**CreateAgent** メソッドをオーバーライドして、カスタムのエージェント クラスの新しいインスタンスを返すようにします。 
  
イベントに渡される引数には、[電子メールメッセージ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx)クラスのインスタンスを含めることができます。これは、基になるメッセージのプロパティとコンテンツを変更するために使用できます。 すべてのメッセージ情報が、各イベントで使用できるわけではありません。 実行するタスクにとって最適なエージェントとイベントを判断する必要があります。 
  
次に示す名前空間には、トランスポート パイプライン内のメッセージを読み取り、書き込み、および変更するために使用できる型が含まれています。
  
- [(データの場合)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [ContentTypes を行います。](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. データの Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [ContentTypes (. Tnef)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [ContentTypes (. vCard)](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
トランスポートエージェントを作成したら、Exchange 管理シェルを使用して[エージェントをインストールおよび管理](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)します。 詳細については、「[Exchange 2013 のトランスポート エージェントの作成](creating-transport-agents-for-exchange-2013.md)」を参照してください。 
  
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)   
- [Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Exchange 2013 の新機能](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Exchange 2013 のサーバーの役割のアーキテクチャ](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [メールボックスサーバーとクライアントアクセスサーバー](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Exchange Server 2013 メールフロー](https://technet.microsoft.com/library/aa996349.aspx)
- [Exchange Server 2013 メールルーティング](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

