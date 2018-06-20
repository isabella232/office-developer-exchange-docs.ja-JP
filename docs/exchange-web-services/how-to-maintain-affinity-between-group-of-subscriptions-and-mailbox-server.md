---
title: Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: サブスクリプション グループとメールボックス サーバー間のアフィニティの維持について説明します。
ms.openlocfilehash: 7cfbfb5cc19e092c37e3d48a7fcc4f27023516e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758972"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。

サブスクリプション グループとメールボックス サーバー間のアフィニティの維持について説明します。
  
アフィニティは、特定のメールボックス サーバーと一連の要求および応答メッセージの関連付けです。 Exchange のほとんどの機能のため、アフィニティは、サーバーによって処理されます。 ただしは、通知を使用すると、例外です。 クライアントの通知サブスクリプションをメールボックス サーバーとの類似性を維持するための責任です。 このアフィニティは、負荷分散装置とクライアント アクセス サーバーのクライアントとサーバーがルートの通知サブスクリプションとサブスクリプションを保持しているメールボックス サーバーに関連する要求の間で有効にします。 関係なしには、クライアントのサブスクリプションでは、返される[ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)エラーが発生することができますが含まれていない別のメールボックス サーバーに要求をルーティングを取得可能性があります。 
  
## <a name="how-is-affinity-maintained"></a>アフィニティはどのように維持されますか？
<a name="bk_howmaintained"> </a>

Exchange でのアフィニティは、Cookie に基づきます。クライアントがサブスクリプション要求に特定のヘッダーを含めることにより、Cookie の作成をトリガーし、次いでサブスクリプションの応答に Cookie が含められます。クライアントは、要求が適切なメールボックス サーバーにルーティングされるようにするために、それ以降の要求で Cookie を送信します。
  
具体的には、Exchange でのアフィニティは、次のように処理されます。  
  
- X-AnchorMailbox – 初期サブスクリプション要求に含まれる HTTP ヘッダー。同じメールボックス サーバーとアフィニティを共有するメールボックスのグループの最初のメールボックスを識別します。
    
- X-PreferServerAffinity – X-AnchorMailbox ヘッダーを持つ最初のサブスクリプション要求に含まれる HTTP ヘッダー。アフィニティがメールボックス サーバーで維持されるようクライアントが要求していることを示す場合に true に設定されます。
    
- X-BackEndOverrideCookie – 最初のサブスクリプション応答に含まれる Cookie。後続の要求を同じメールボックス サーバーにルーティングするためにロード バランサーとクライアント アクセス サーバーが使用する Cookie を含みます。
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>EWS Managed API または EWS を使用してアフィニティを維持する方法
<a name="bk_howdoimaintain"> </a>

同じ手順を使用して、複数のメールボックスのサブスクリプションとメールボックス サーバーに対するアフィニティを維持できます。ストリーミング、プル、またはプッシュの通知のどれを使用しているかには関係なく、オンプレミスの Exchange Server または Exchange Online のどちらを対象としているかにも関係ありません。
  
1. メールボックスごとに[自動検出を呼び出す](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)し、GroupingInformation と ExternalEwsUrl のユーザー設定を取得します。 SOAP の自動検出の[設定](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)要素を使用して POX の自動検出は、 [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx)要素を使用します。 
    
2. 自動検出応答からの GroupingInformation と ExternalEwsUrl 設定を使用して、メールボックスを同じグループの ExternalEwsUrl と GroupingInformation の連結された値に配置します。グループに 200 個を超えるメールボックスがある場合は、グループをさらに分解して、各グループが 200 個を超えるメールボックスを持たないようにします。
    
3. 作成し、プロシージャの残りの部分の 1 つの[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx)オブジェクトを使用します。 使用すると、同じ**ExchangeService**オブジェクト、cookie およびヘッダー (設定している) 場合は自動的に維持されます。 グループ ストリーミングのサブスクリプションの単一の接続にする予定がない場合としている偽装されたユーザーごとに別の**ExchangeService**オブジェクトを作成するに注意してください。 
    
4. グループ内のすべてのユーザーがアルファベット順に並べ替えられたときに、ユーザー名が最初に表示するユーザーの要求を[送信するサブスクリプション](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)(私たちを参照してくださいアンカーのメールボックスのユーザーとしてこのユーザー)。 次の操作を行います。 
    
  - アンカーのメールボックス ユーザーの SMTP アドレスに設定された値を持つ X-AnchorMailbox ヘッダーを含めます。
    
  - 値が true に設定された X-PreferServerAffinity ヘッダーを含めます。
    
  - [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)ロール ( [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)型) を使用します。 
    
5. サブスクリプションの応答で、X-BackEndOverrideCookie の値を取得します。このグループ内のユーザーに対するそれ以降のサブスクリプション要求のそれぞれに、この値を含めます。
    
6. グループ内の追加ユーザーごとに、サブスクリプション要求を送信して、次の操作を行います。
    
  - グループのアンカーのメールボックス ユーザーの SMTP アドレスに設定された値と X-AnchorMailbox ヘッダーを含めます。
    
  - 値が true に設定された X-PreferServerAffinity ヘッダーを含めます。
    
  - サブスクリプションのアンカーのメールボックス ユーザーの応答で返された X BackEndOverrideCookie が含まれます。
    
  - [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)ロール ( [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)型) を使用します。 
    
    サーバーは X-PreferServerAffinity と X-BackendOverrideCookie の値を一緒に使用して、メールボックス サーバーへのルーティングを実行することに注意してください。X-AnchorMailbox ヘッダーも必要ですが、他の 2 つの値が有効な場合、サーバーでは無視されます。X-AnchorMailbox と X-PreferServerAffinity が要求内にあり、X-BackendOverrideCookie が含まれていない場合、X-AnchorMailbox の値が要求のルーティングに使用されます。
    
    X-PreferServerAffinity と X-BackendOverrideCookie の値がルーティングを実行するため、アンカーのメールボックスが別のグループまたはサーバーに移動する場合、X-BackendOverrideCookie が要求をグループの適切なサーバーにルーティングし、ロジックは変わりません。
    
7. グループの 1 つの[GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx)または[GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx)要求を送信して、次の操作を行います。 
    
  - 各グループ内のメールボックスの 1 つのサブスクリプションの応答で返された[サブスクリプション Id](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx)値が含まれます。 
    
  - グループに対しては、200 以上のサブスクリプションが存在する場合は、複数の要求を作成します。 要求に含める[サブスクリプション Id](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx)値の最大数は、200 です。 
    
  - 移動先のメールボックスを使用できるよりもより多くの接続が必要な場合にサービス アカウントを使用してグループのアンカーのメールボックスの偽装それ以外の場合、偽装を使用しません。 理想的には、調整の制限を受けることはありませんように[GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx)または[GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx)要求ごとに一意のメールボックスの権限を借用します。 
    
  - ApplicationImpersonation を使用して、[移動先のメールボックスを使用できるよりもより多くの接続](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)が必要な場合それ以外の場合、ApplicationImpersonation を使用しません。
    
  - X PreferServerAffinity ヘッダーをインクルードし、true に設定します。 この値は、手順 2 で作成した**ExchangeService**オブジェクトを使用している場合に自動的に含まれます。 
    
  - グループ (、X-BackEndOverrideCookie アンカー メールボックス ユーザーのサブスクリプションの応答で返された) の X-BackEndOverrideCookie が含まれます。 この値は、手順 2 で作成した**ExchangeService**オブジェクトを使用している場合に自動的に含まれます。 
    
8. 返されたイベントを別のスレッドに渡して処理します。
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>考慮に入れる必要がある調整の値は何ですか？
<a name="bk_throttling"> </a>

通知の実装を計画するときは、2 つの値を考慮に入れるたい: 接続の数をおよびサブスクリプションの数です。 次の表は、各[調整](ews-throttling-in-exchange.md)の設定の既定値と設定を使用する方法です。 、値ごとに、予算は、移動先のメールボックスに割り当てられます。 このため、多くのシナリオで必要な手順は、追加の接続を得るために偽装を使用します。 
  
**表 1 です。既定のスロットル値**

|**領域の考慮事項**|**調整設定**|**既定値**|**説明**|
|:-----|:-----|:-----|:-----|
|ストリーミング接続  <br/> |既定の接続切断の制限  <br/> |Exchange のオンライン 10  <br/> Exchange 2013 の 3  <br/> |アカウントを持つことができる、ストリーミングの同時接続の最大数は、サーバー上で同時に開きます。 この制限内で作業対象のメールボックスに割り当てられている ApplicationImpersonation の役割を持つサービス アカウントを使用して、イベントをストリームを取得するときは、各サブスクリプション ID のグループの最初のユーザーを偽装します。  <br/> |
|プルまたはプッシュの接続  <br/> |EWSMaxConcurrency  <br/> |27  <br/> |アカウントがサーバー上で同時に開いておくことができる並行プルまたはプッシュの最大接続数 (受信されているが、まだ応答されていない要求)。  <br/> |
|サブスクリプション  <br/> |EWSMaxSubscriptions  <br/> |Exchange のオンライン 20  <br/> Exchange 2013 5000  <br/> |アカウントが同時に持つことができる、期限が切れていないサブスクリプションの最大数。この値は、サーバーでサブスクリプションが作成されたときに減少します。  <br/> |
   
次の例では、すべてターゲット メールボックスと対象のメールボックスに割り当てられている[ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)の役割を持つサービス アカウントの間で予算を処理する方法を示します。 
  
- ServiceAccount1 (sa1) は、(m1、m2、m3 など) の多くのユーザーを偽装し、メールボックスごとにサブスクリプションを作成します。サブスクリプションが作成されると、サブスクリプションの所有者は sa1 となり、sa1 がサブスクリプションとの接続を開くと、EWS が強制してサブスクリプションが sa1 に所有されます。
    
- sa1 は、次の方法で接続を開くことができます。
    
1. 偽装をせず、接続が sa1 に対して課金されます。
    
2. すべてのユーザーを偽装して、たとえば m1-接続は m1 の予算のコピーを請求するためです。 (M1 自体、Exchange Online を使用して、10 個の接続を開くことができ、m1 を偽装しているすべてのサービス アカウントは、コピー元の予算を使用して 10 個の接続を開くことができます)。
    
- 接続制限に達した場合、次の回避策を利用できます。
    
  - オプション 1 が使用されている場合、管理者は、追加のユーザーを偽装するように複数のサービス アカウントを作成できます。
    
  - オプション 2 が使用されている場合、コードが別のユーザー (m2 など) を偽装できます。
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>例:サブスクリプション グループとメールボックス サーバー間のアフィニティを維持する
<a name="bk_ce"> </a>

ですが、アクションの説明を参照してください。 次のコード例は、ユーザーをグループ化し、メールボックス サーバーとのアフィニティを維持するために X AnchorMailbox X PreferServerAffinity のヘッダーと X BackendOverrideCookie の cookie を使用する方法を示しています。 ヘッダーおよび cookie はアフィニティのストーリーの中で重要であるために、次の使用例は、EWS の XML 要求と応答について説明します。 EWS のマネージ API を使用して、サブスクリプションの要求と応答の本文を作成するのには、 [EWS を使用して Exchange でのメールボックスのイベントに関する通知をストリーム](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)し[、EWS を使用して Exchange メールボックスのイベントに関する通知をプル](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)を参照してください。 このセクションには、アフィニティを維持し、要求にヘッダーを追加する特定追加の手順にはが含まれています。
  
この例では、4 つのユーザー: alfred@contoso.com、alisa@contoso.com、ronnie@contoso.com、および sadie@contoso.com。 次の図は、GroupingInformation と ExternalEwsUrl の[自動検出の設定](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)ユーザーを示します。 
  
**図 1 です。グループのメールボックスに使用される自動検出の設定**

![各ユーザーの GroupingInformation および ExternalEwsUrl の値を表示している表。](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
自動検出応答からの設定を使用して、GroupingInformation と ExternalEwsUrl の設定の連結された値により、メールボックスがグループ化されます。この例では、Alfred と Sadie は同じ値を持つ 1 つのグループであり、Alisa および Ronnie は別のグループにいて同じ値を共有しています。
  
**図 2 になります。メールボックスのグループを作成します。**

![Autodiscover 設定を使用してどのようにメールボックス グループが作成されるかを示した表。](media/Exchange2013_NotificationAffinityGrouping.png)
  
この例では、グループ A にフォーカスします私たちはグループ B に同じ手順を使用ですが、別の X AnchorMailbox 値を使用して、そのグループの。
  
X AnchorMailbox ヘッダーを設定とアンカーのメールボックス (alfred@contoso.com)、サブスクリプション要求を作成する[ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)を使用して、その電子メール アドレスと、X PreferServerAffinity ヘッダーの値が true です。 これら 2 つのヘッダー値を設定すると、応答の X BackEndOverrideCookie を作成するサーバーが発生します。
  
EWS のマネージ API を使用する場合は、ように、サブスクリプション要求に 2 つのヘッダーを追加するのには[立てて](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e)メソッドを使用します。 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

アルフレッドのサブスクリプションの要求は次のような。
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

アルフレッドのサブスクリプションの要求への応答は、次の XML メッセージと、X の BackEndOverrideCookie が含まれています。 このグループ内のユーザーのすべての後続の要求に対しては、この cookie を再送信します。 応答が Exchange 2010 によって使用される exchangecookie クッキーなどの他の cookie にはも含まれていることを確認します。 Exchange Online、Exchange オンライン Office 365 の一部のバージョンの Exchange が Exchange 2013 年から始まるとそれ以降のサブスクリプション要求に含まれている場合、exchangecookie を無視します。
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

アルフレッドの応答からの X-BackEndOverrideCookie を使用して、X AnchorMailbox ヘッダー、Sadie のサブスクリプション要求が作成される、グループ a: Sadie のサブスクリプション要求の他のメンバーは次のようになります。
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@consoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@consoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

Sadie のサブスクリプションの応答は、次のように検索します。 X-BackEndOverrideCookie が含まれていないことに注意してください。 クライアントは、以降の要求は、その値をキャッシュします。
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

グループ内のすべてのサブスクリプションのサブスクリプション応答の[サブスクリプション Id](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx)値を使用すると、 [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx)操作の要求が作成されました。 このグループの数が 200 未満のサブスクリプションがあるため、すべての送信要求が 1 つ。 X PreferServerAffinity ヘッダーの設定を true に、X の BackEndOverrideCookie が含まれています。 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

返されたイベントは、別のスレッドに渡して処理します。
  
## <a name="how-has-affinity-changed"></a>アフィニティはどのように変化したのでしょうか？
<a name="bk_howchanged"> </a>

Exchange 2010 では、サブスクリプションが使用されます、クライアント アクセス サーバーで、図 3 に示すように。 図 4 に示すようには、Exchange 2010 以降のバージョンの Exchange メールボックス サーバーで、サブスクリプションが維持されます。
  
**図 3 です。Exchange 2010 での類似性を維持するためのプロセス**

![Exchange 2010 のクライアント アクセス サーバーで、アクティブ サブスクリプションのテーブルがどのように維持されるかを示す図。](media/Exchange2013_NoficationAffinity2010.png)
  
**図 4 です。オンラインの Exchange および Exchange 2013 のアフィニティを維持するためのプロセス**

![ロード バランサーおよびクライアント アクセス サーバーが、要求をどのように Exchange Server および Exchange Online でアクティブ サブスクリプションのテーブルを維持するメールボックス サーバーにルーティングするかを示す図。](media/Exchange2013_NoficationAffinity2013.png)
  
Exchange 2010 クライアントだけを知っているロード バランサーのアドレスとサーバーによって返される exchangecookie が適切なクライアント アクセス サーバーに要求がルーティングされることを保証します。 ただし、それ以降のバージョン、ロード バランサー、およびクライアント アクセス サーバーの役割の両方があるメールボックス サーバーを取得する前に、適切に要求をルーティングします。 追加情報が必要であるには、新しいヘッダーおよび cookie が導入された理由であります。 [通知サブスクリプション、メールボックス イベント、および Exchange 内](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)の資料では、Exchange 2013 のサブスクリプションを維持する方法について説明します。 
  
以降のバージョンで Exchange 2010 を使用する exchangecookie がまだ返されることがわかります可能性があります。 要求でこの cookie を含む危害はありませんが、それ以降のバージョンの Exchange を無視すること。
  
## <a name="see-also"></a>関連項目

- [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Exchange の EWS を使用してメールボックスのイベントに関する通知をストリーム](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [EWS を使用して Exchange でメールボックスのイベントに関する通知をプルします。](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
- [EWS サブスクリプション用の関係を管理するうえで変更しています.](http://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [EWS の交換で調整](ews-throttling-in-exchange.md)
    

