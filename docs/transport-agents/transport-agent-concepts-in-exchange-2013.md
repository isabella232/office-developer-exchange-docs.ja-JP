---
title: Exchange 2013 におけるトランスポート エージェントの概念
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Exchange 2013 のトランスポート エージェント パイプラインとサーバー役割アーキテクチャがトランスポート エージェントの開発に与える影響、およびトランスポート エージェントの開発に使用できるクラスについて説明します。
ms.openlocfilehash: 9116c9b7811958a2479421a642052df3cee24e34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537162"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Exchange 2013 におけるトランスポート エージェントの概念

Exchange 2013 のトランスポート エージェント パイプラインとサーバー役割アーキテクチャがトランスポート エージェントの開発に与える影響、およびトランスポート エージェントの開発に使用できるクラスについて説明します。 
  
**製品:** Exchange Server 2013 
  
Exchange Server 2013 で提供されているクラス ライブラリを使用して、イベントに登録し、トランスポート パイプラインを通過するメッセージに対してアクションを実行するトランスポート エージェントを実装できます。 また、メッセージの変更とコンテンツの変換にも、トランスポート エージェントを使用できます。 
  
この記事では、トランスポート エージェントとトランスポート パイプライン アーキテクチャに関する情報を提供します。トランスポート パイプラインのアーキテクチャについて理解することは重要です。そうすることで、組織のニーズに合わせてトランスポートの動作を変更できるようになります。この記事では、トランスポート エージェントに影響する Exchange 2013 アーキテクチャの変更内容と、トランスポート エージェントの開発に使用できるクラスに関する情報についても提供します。  
  
## <a name="transport-agents-in-the-transport-pipeline"></a>トランスポート パイプライン内のトランスポート エージェント
<a name="Pipeline"> </a>

トランスポート エージェントは、次に示す 3 つのクラスのいずれかから派生します。
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
トランスポート パイプラインとは、Exchange 2013 組織の境界内でのメッセージ データの流れのことを意味します。パイプラインは、次の表に示したサービスによって成立します。
  
**表 1.トランスポート パイプライン サービス**

|**サービス**|**説明**|**サポートされるクラス**|
|:-----|:-----|:-----|
|フロント エンド トランスポート  <br/> |すべてのクライアント アクセス[サーバーで](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx)実行され、2013 組織のすべての受信および送信外部 SMTP トラフィックのステートレス プロキシExchangeします。 フロント エンド トランスポート サービスは、メッセージ コンテンツを検査することも、メッセージをローカルにキューに格納することもありません。 メールボックス サーバー上のトランスポート サービスと [通信します](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx)。  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |すべてのメールボックス サーバーで実行され、2010 年のハブ トランスポート サーバーの役割Exchange Serverされます。 [](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx) トランスポート サービスは、それ自体とメールボックス トランスポート サービスとフロントエンド トランスポート サービスの間でメッセージをルーティングします。 このサービスは、メールボックス データベースと直接通信しない。  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|メールボックス トランスポート  <br/> |すべてのメールボックス サーバーで実行され、メールボックス トランスポート送信とメールボックス トランスポート配信の 2 つの異なるサービスで構成されます。 メールボックス トランスポート配信は、トランスポート サービスから SMTP メッセージを受信し、Exchange リモート プロシージャ 呼び出し (RPC) を使用してメールボックス データベースに接続してメッセージを配信します。 メールボックス トランスポート送信は RPC を使用してメールボックス データベースに接続してメッセージを取得し、SMTP 経由でメッセージをトランスポート サービスに送信します。  <br/> |なし。  <br/> |
   
### <a name="transport-events"></a>トランスポート イベント
<a name="Events"> </a>

トランスポート エージェントは、まずイベントを登録して、そのイベントが発生したときにアクションを起こすことで実装します。3 種類のそれぞれのエージェントで、異なるイベントのセットを登録できます。
  
次の図は、トランスポート エージェントがトランスポート パイプラインのどの部分でイベントを登録できるかを示しています。
  
**図 1.トランスポート イベント**

![トランスポート パイプラインを介したメッセージ フロー、および各エージェントが登録できるイベントを示すイメージ。SmtpReceivedAgent の SMTP イベントから始まり、RoutingAgent の Categorizor イベント、そして最後に DeliveryAgent の配信イベントが続きます。](media/TAConceptsFig1.png)
  
メッセージがトランスポート パイプラインに入った場合 [、SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) クラスから派生したトランスポート エージェントは、エージェントが登録した SMTP イベントの間にメッセージに対して処理できます。 [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)クラスから派生したエージェントは、登録されている 4 つのカテゴライザー イベントに対して実行できます。 [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)クラスから派生したエージェントは、登録されている配信イベントの間にメッセージに対して処理できます。 
  
## <a name="transport-agents-and-server-roles"></a>トランスポート エージェントとサーバーの役割
<a name="ServerRoles"> </a>

2013 年 2013 年のサーバー役割アーキテクチャの変更はExchangeエージェントと、トランスポート エージェントが実行できる操作に影響します。 Exchange 2013 には、次のサーバーの役割が含まれています。
  
- メールボックス サーバー: クライアント アクセス プロトコル、トランスポート サービス、メールボックス データベース、ユニファイド メッセージング コンポーネントが含まれます。メールボックス サーバーは、Active Directory ドメイン サービス (AD DS)、クライアント アクセス サーバー、および Outlook などのメール クライアントと直接通信します。
    
- クライアント アクセス サーバー: 認証、制限付きリダイレクト、プロキシ サービス、およびクライアント アクセス プロトコル (HTTP、POP、IMAP、SMTP など) を提供します。
    
- エッジ トランスポート サーバー: 電子メールを組織の内外にルーティングします。エッジ トランスポート サーバーは、通常、Exchange トポロジの境界に配置されます。
    
この統合構造により、Exchange 2013 環境に展開する必要のあるサーバー数が少なくなります。管理者はメールボックス サーバーが含まれる Active Directory サイトごとにハブ トランスポート サーバーとクライアント アクセス サーバーを展開する必要がなくなりました。また、新しい機能を利用するために、サーバーの役割をすべて更新するという必要もなくなりました。
  
このようなサーバーの役割アーキテクチャに対する変更は、カスタムのエージェントがパイプラインのどの部分でイベントに応答できるかに影響を及ぼす可能性があります。Exchange 2013 よりも前の Exchange の各バージョンに対応したトランスポート エージェントを作成してある場合は、アーキテクチャの変更点を確認して、カスタムのエージェントに変更を加える必要があるかどうかを判断してください。
  
次の図は、Exchange 2013 のアーキテクチャ上の変更点が、どのようにトランスポート パイプラインを合理化および統合化しているかについて示しています。この図では、クライアント アクセス サーバーに「CAS」というラベルが付けられています。また、メールボックス サーバーには「MBX」というラベルが付けられています。
  
**図 2.Exchange 2013 サーバーの役割アーキテクチャ**

![外部のファイアウォールを通過するクライアント トラフィックを示すイメージ。左側にはレイヤー 4 の負荷分散から統合 CAS 配列にトラフィックを渡すエッジ トランスポートがあり、右側にはデータベース アクセシビリティ グループの一連のメールボックス サーバーがあります。](media/Transport_Agent_Concepts_Fig_3.png)
  
次の図は、Exchange 2013 のサーバーの役割間での相互作用を示しています。
  
**図 3.メールボックスとクライアント アクセス サーバーの操作**

![CAS に 4 つのターゲット (IIS/HTTP Proxy、POP/IMAP、SMTP、および UM) が存在するレイヤー 4 の負荷分散を通過するクライアント トラフィックから矢印が始まるやり取りを示すイメージ。矢印は、メールボックス ストアのコンプリメンタリ ターゲットを通過します。](media/Transport_Agent_Concepts_Fig_4.png)
  
Exchange 2013 サーバーの役割アーキテクチャの変更の詳細については[、「Exchange 201](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) [Exchange 3](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)年の新機能」を参照してください。 
  
## <a name="transport-agent-classes"></a>トランスポート エージェントのクラス
<a name="Create"> </a>

カスタムのトランスポート エージェントの派生元クラスにより、そのエージェントで登録できるイベントが決まります。通常、カスタムのエージェントには、1 つのエージェント クラス、1 つのエージェント ファクトリ、1 つ以上のイベント ハンドラー、およびエージェントで処理するアクションを実行するコードが含まれています。
  
次の表は、それぞれのエージェントの種類の派生元になるクラスを示しています。
  
**表 2.エージェント クラス**

||||
|:-----|:-----|:-----|
|エージェントの種類  <br/> |ファクトリの基底クラス  <br/> |エージェントの基底クラス  <br/> |
|SMTP の受信  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|ルーティング  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Delivery  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
これらのファクトリとエージェントの基底クラスには、トランスポート イベントとメッセージへのアクセスに使用できるプロパティとメソッドが用意されています。カスタムのエージェントには、これらのクラスから継承するクラスを実装します。エージェント ファクトリ派生クラスでは、**CreateAgent** メソッドをオーバーライドして、カスタムのエージェント クラスの新しいインスタンスを返すようにします。 
  
イベントに渡される引数には [、EmailMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) クラスのインスタンスを含め、基になるメッセージのプロパティと内容を変更するために使用できます。 すべてのメッセージ情報が、各イベントで使用できるわけではありません。 実行するタスクにとって最適なエージェントとイベントを判断する必要があります。 
  
次に示す名前空間には、トランスポート パイプライン内のメッセージを読み取り、書き込み、および変更するために使用できる型が含まれています。
  
- [Microsoft。Exchange。Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft。Exchange。Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft。Exchange。Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft。Exchange。Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft。Exchange。Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
トランスポート エージェントを作成した後は[](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)、管理シェルを使用してエージェントをインストールExchangeします。 詳細については、「[Exchange 2013 のトランスポート エージェントの作成](creating-transport-agents-for-exchange-2013.md)」を参照してください。 
  
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)   
- [Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [2013 年の新機能Exchange](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Exchange 2013 Server Role Architecture](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [メールボックスおよびクライアント アクセス サーバー](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Exchange Server 2013 メール Flow](https://technet.microsoft.com/library/aa996349.aspx)
- [Exchange Server 2013 メール ルーティング](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

