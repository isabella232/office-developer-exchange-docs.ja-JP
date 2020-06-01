---
title: Exchange の自動検出
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: da0f9402-4e35-42c7-a15e-1e9e4e966e8b
description: Exchange 自動検出サービスについて説明します。
localization_priority: Priority
ms.openlocfilehash: 913ec3fef93900a1b5fa7aa342e8bca149c88b7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44437760"
---
# <a name="autodiscover-for-exchange"></a>Exchange の自動検出

Exchange 自動検出サービスについて説明します。
  
Exchange 自動検出サービスは、最小限のユーザー入力でカスタムのクライアント アプリケーションが構成されるようにするための簡単な方法を提供します。ほとんどのユーザーは、自分の電子メール アドレスとパスワードを知っています。それら 2 つの情報の断片によって、稼働に必要なその他の詳細のすべてを取得できます。Exchange Web サービス (EWS) クライアントの場合、通常、自動検出は EWS エンドポイント URL を見つけるために使用されますが、その他のプロトコルを使用するクライアントを構成する情報も自動検出によって得られます。自動検出は、ファイアウォールの内側または外側のクライアント アプリケーションに有効であり、リソース フォレストおよび複数フォレストのシナリオで動作します。
  
## <a name="overview-of-the-autodiscover-process"></a>自動検出プロセスの概要
<a name="bk_Before"> </a>

自動検出プロセスには、基本的に 3 つのフェーズがあります。フェーズ 1 では潜在的な自動検出サーバーの一覧を生成して、フェーズ 2 では成功の応答 (可能な場合) が得られるまで一覧の各サーバーを試します。いずれの候補もうまくいかなかった場合は、フェーズ 3 に移行します。このフェーズは、自動検出エンドポイントを見つけるための「最後の努力」を表します。
  
EWS マネージ API の [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドにより、このプロセスの 3 つのフェーズはすべて実装されます。そのため、EWS マネージ API を使用する場合は、独自に自動検出を実装することについて心配する必要はありません。 次の図は、自動検出プロセスの 3 つのフェーズを示しています。 
  
**図 1. 自動検出プロセスの 3 つのフェーズ**

![候補プールの定義、エンドポイントの試行、他の選択肢の試行の 3 つのフェーズを示す自動検出プロセスの図。](media/Ex15_Autodiscover_Overview.png)
  
### <a name="phase-1-defining-the-candidate-pool"></a>フェーズ 1: 候補プールを定義する
<a name="bk_Phase1"> </a>

自動検出を使用するには、まず、ユーザーに正しい自動検出サーバーの場所を示す必要があります。好都合なことに、自動検出の定義により、探す場所の数は限られています。複数の候補が見つかった場合、自動検出では[一覧の生成して優先度を設定する方法](how-to-generate-a-list-of-autodiscover-endpoints.md)も定義されています。
  
**表 1. 自動検出エンドポイント候補のソース**

|**探す場所**|**見つかるもの**|
|:-----|:-----|
|Active Directory Domain Services (AD DS)  <br/> |ドメインに参加しているクライアントの場合は、最初に探す場所になります。Exchange は AD DS にサービス接続ポイント (SCP) オブジェクトを公開します。これにより、自動検出の要求は Active Directory サイトに基づいてサーバーにルーティングできるようになります。[SCP 検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)の結果は、候補一覧の最上位にする必要があります。<br/><br/>**注**: SCP 検索は、ドメインに参加していないクライアントや Active Directory サーバーにアクセスできないクライアントには使用できません。 この場合は、SCP 検索を省略する必要があります。 <br/>|
|ユーザーの電子メール アドレス ドメイン  <br/> | 自動検出では、標準エンドポイント URL の形式が 2 つ定義されています。これは、ユーザーの電子メール アドレスのドメイン部分から派生します。  <br/>`"https://" + domain + "/autodiscover/autodiscover" +  *fileExtension*`  <br/>`"https://autodiscover." + domain + "/autodiscover/autodiscover" +  *fileExtension*`<br/><br/>  *fileExtension* の値は、自動検出のアクセス方式に [SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) と [POX](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) のどちらを使用しているかによって決まります。 SOAP サービスではファイル拡張子 ".svc" が使用され、POX では ".xml" が使用されます。  <br/> |
   
次の図は、自動検出エンドポイント一覧の生成方法を示しています。
  
**図 2. 自動検出エンドポイント一覧の生成プロセス**

![図は自動検出エンドポイントのリストを生成するためのプロセスを示しています。矢印は、エンドポイントのリストが SCP 参照や、ユーザーの電子メールアドレスから生じることを示しています。](media/Ex15_Autodiscover_Overview_Phase1.png)
  
### <a name="phase-2-trying-each-candidate"></a>フェーズ 2: 各候補を試してみる
<a name="bk_Phase2"> </a>

潜在的な候補の順序付き一覧を生成したら、[URL に要求を送信](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)して結果を検証することで、一覧の各候補を試してみます。図 3 を参照してください。成功の応答が得られた時点で完了です。 
  
**図 3. 各エンドポイント候補を順に試す**

![サーバーが正常な応答を受信するまで優先順位順に各エンドポイントを試行することを示す図。](media/Ex15_Autodiscover_Overview_Phase2.png)
  
候補に要求を送信する前に、その候補が信頼可能であることを確認します。ユーザーの資格情報を送信することを忘れてはいけません。その情報の共有は信頼できるサーバーに限定することが重要です。少なくとも、次の事項を確認する必要があります。
  
- エンドポイントが HTTPS エンドポイントであること。クライアント アプリケーションは、非 SSL エンドポイントに対して認証やデータの送信を行ってはいけません。
    
- サーバーが提示した SSL 証明書が信頼された機関からのものであり有効であること。
    
> [!NOTE]
> これらは、基本的なセキュリティの推奨事項にすぎません。認証を扱うときには、コードが組織のセキュリティ要件を満たしていることを常に確認します。 
  
送信する要求の種類は、自動検出サービスにアクセスする方法によって決まります。
  
**表 2. 自動検出の要求の種類**

|**使用するもの**|**要求を送信する手段**|
|:-----|:-----|
|EWS マネージ API  <br/> |[GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) メソッド。  <br/> |
|SOAP 自動検出サービス  <br/> |[GetUserSettings](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) 操作。  <br/> |
|POX 自動検出サービス  <br/> |[自動検出要求本文](https://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx)が含まれる HTTP POST。  <br/> |
   
### <a name="phase-3-trying-other-alternatives"></a>フェーズ 3: その他の方法を試す
<a name="bk_Phase3"> </a>

一覧に含まれるすべてのエンドポイントを試してみたときに、それらすべてがエラーを返すことがあります。あきらめる前に、いくつか別のものを試してみることができます。認証されていない GET 要求を送信したり、SRV レコードについて DNS を照会したりできます。これらの試行でも成果が得られない場合は、自動検出サービスに接続できません。
  
**図 4. その他の方法を試す**

![認証されていない GET 要求および DNS クエリを介して生成された新しいエンドポイントを示す図。](media/Ex15_Autodiscover_Overview_Phase3.png)
  
#### <a name="sending-an-unauthenticated-get-request"></a>認証されていない GET 要求の送信

最初に試してみることは、ユーザーの電子メール アドレスから派生したエンドポイントに向けて、認証されていない GET 要求を送信することです。 そのエンドポイントは、"http://autodiscover" + domain + "/autodiscover/autodiscover.xml" の形式です。 これは SSL エンドポイントでない点に注意してください。 サーバーが 302 リダイレクト応答を返す場合は、その応答の Location ヘッダーに含まれるエンドポイント URL に向けて[自動検出要求の再送信](handling-autodiscover-error-messages.md#bk_ResendRequest)を試してみます。 
  
#### <a name="querying-dns-for-an-srv-record"></a>SRV レコードについての DNS の照会

認証されていない GET 要求が失敗した場合に、最後に試してみることは、自動検出サービスに関する SRV レコードに対する DNS クエリです。このレコードは、"_autodiscover._tcp." + ドメインの形式になります。このクエリは複数のレコードを返すことがありますが、最高の優先度と重みが付けられた SSL エンドポイントをポイントするレコードのみを使用します。
  
## <a name="options-for-using-autodiscover"></a>自動検出を使用する場合のオプション
<a name="bk_Options"> </a>

自動検出には、SOAP Web サービスまたは POX Web サービスを使用してアクセスできます。どのメソッドを使用するかは、要件と環境に応じて決まります。ただし、可能であれば SOAP Web サービスの使用をお勧めします。EWS マネージ API も選択肢の 1 つになります。これにより、SOAP と POX の両方の自動検出サービスのクライアント部分が実装されます。
  
**表 3: 自動検出にアクセスする場合のオプション**

|**オプション**|**利点**|**欠点**|
|:-----|:-----|:-----|
|[EWS マネージ API](get-started-with-ews-managed-api-client-applications.md) <br/> | 自動検出プロセスが実装される。<br/><br/>SOAP と POX の両方の自動検出サービスを使用する。<br/><br/>Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降の Exchange の各バージョンで動作する。<br/><br/>使いやすい。  <br/> | [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) 列挙体で使用できるユーザー設定に制限される。<br/><br/>.NET Framework アプリケーションにのみ使用できる。  <br/> |
|[SOAP 自動検出](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) <br/> | プラットフォームに依存しない。<br/><br/>監視のある設定のみを要求できる。  <br/> | Exchange 2007 では使用できない。  <br/> |
|[POX 自動検出](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) <br/> | プラットフォームに依存しない。<br/><br/>Exchange Online および Exchange 2007 SP1 以降のすべてのバージョンでサポートされる。  <br/> | 特定の設定を要求できない。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容

- [Exchange の SCP 参照を使用して自動検出エンドポイントを見つける](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)
    
- [自動検出を使用して接続ポイントを検索する](how-to-use-autodiscover-to-find-connection-points.md)
    
- [自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Exchange サーバーからドメイン設定を取得する](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [自動検出を使用して構成情報を更新する](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [自動検出のエラー メッセージを処理する](handling-autodiscover-error-messages.md)
    
- [Exchange の自動検出を使用するときにパフォーマンスを向上させる](improving-performance-when-using-autodiscover-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)    
- [Exchange 2013: 自動検出によるユーザー設定の取得](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)
- [Autodiscover Checker サンプル](https://code.msdn.microsoft.com/exchange/Autodiscover-Checker-e1ebca42)  
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

