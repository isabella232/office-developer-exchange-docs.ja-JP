---
title: Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: サブスクリプション グループとメールボックス サーバー間のアフィニティの維持について説明します。
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455758"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する

サブスクリプション グループとメールボックス サーバー間のアフィニティの維持について説明します。
  
アフィニティは、特定のメールボックス サーバーと一連の要求および応答メッセージの関連付けです。 Exchange のほとんどの機能では、アフィニティはサーバーによって処理されます。 ただし、通知は例外です。 通知サブスクリプションについては、クライアントがメールボックス サーバーとのアフィニティを維持します。 このアフィニティにより、クライアントとサーバーの間のロード バランサーとクライアント アクセス サーバーは、通知サブスクリプションと関連する要求を、サブスクリプションを維持するメールボックス サーバーにルーティングします。 アフィニティを使用しない場合、要求はクライアントのサブスクリプションを含まない別のメールボックスサーバーにルーティングされ、 [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)エラーが返されることがあります。 
  
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
  
1. 各メールボックスで [Autodiscover を呼び出して](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) GroupingInformation と ExternalEwsUrl のユーザー設定を取得します。SOAP の自動検出では [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) 要素を使用し、POX の自動検出では [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) 要素を使用します。 
    
2. 自動検出応答からの GroupingInformation と ExternalEwsUrl 設定を使用して、メールボックスを同じグループの ExternalEwsUrl と GroupingInformation の連結された値に配置します。グループに 200 個を超えるメールボックスがある場合は、グループをさらに分解して、各グループが 200 個を超えるメールボックスを持たないようにします。
    
3. 手順の残りの部分には、1つの[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx)オブジェクトを作成して使用します。 同じ **ExchangeService** オブジェクトを使用する場合、Cookie とヘッダー (設定されている場合) は自動的に維持されます。 ストリーミングのサブスクリプションを単一の接続にグループ化する予定がない場合は、偽装されたユーザーごとに様々な **ExchangeService** オブジェクトを自由に作成できます。 
    
4. グループ内のすべてのユーザーがアルファベット順に並べ替えられるときに、最初にユーザー名が表示されるユーザーの[サブスクリプション要求を送信](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)します (このユーザーは、アンカーメールボックスユーザーと呼ばれます)。 以下のことを行います。 
    
  - アンカーのメールボックス ユーザーの SMTP アドレスに設定された値を持つ X-AnchorMailbox ヘッダーを含めます。
    
  - 値が true に設定された X-PreferServerAffinity ヘッダーを含めます。
    
  - [Applicationimpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)役割 ( [exchangeimpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)型) を使用します。 
    
5. サブスクリプションの応答で、X-BackEndOverrideCookie の値を取得します。 このグループ内のユーザーに対するそれ以降のサブスクリプション要求のそれぞれに、この値を含めます。
    
6. グループ内の追加ユーザーごとに、サブスクリプション要求を送信して、次の操作を行います。
    
  - グループのアンカーのメールボックス ユーザーの SMTP アドレスに設定された値と X-AnchorMailbox ヘッダーを含めます。
    
  - 値が true に設定された X-PreferServerAffinity ヘッダーを含めます。
    
  - アンカーメールボックスユーザーのサブスクリプション応答で返された X-backendoverridecookie を含めます。
    
  - [Applicationimpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)役割 ( [exchangeimpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)型) を使用します。 
    
    サーバーは X-PreferServerAffinity と X-BackendOverrideCookie の値を一緒に使用して、メールボックス サーバーへのルーティングを実行することに注意してください。X-AnchorMailbox ヘッダーも必要ですが、他の 2 つの値が有効な場合、サーバーでは無視されます。X-AnchorMailbox と X-PreferServerAffinity が要求内にあり、X-BackendOverrideCookie が含まれていない場合、X-AnchorMailbox の値が要求のルーティングに使用されます。
    
    X-PreferServerAffinity と X-BackendOverrideCookie の値がルーティングを実行するため、アンカーのメールボックスが別のグループまたはサーバーに移動する場合、X-BackendOverrideCookie が要求をグループの適切なサーバーにルーティングし、ロジックは変わりません。
    
7. グループに対して 1 つの [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) または [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) 要求を送信し、次の操作を行います。 
    
  - グループ内のメールボックスの各サブスクリプションの応答で返される [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) の値を含めます。 
    
  - グループで 200 以上のサブスクリプションが存在する場合は、複数の要求を作成してください。要求に含める [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) の値の最大数は 200 です。 
    
  - 対象となるメールボックスで使用できるよりもより多くの接続が必要な場合は、サービス アカウントを使用してグループのアンカーのメールボックスを偽装します。それ以外の場合は、偽装を使用しません。理想的には、[GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) または [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) 要求ごとに一意のメールボックスを偽装すると、調整の制限が発生しません。 
    
  - [対象となるメールボックスで利用できるよりも多くの接続](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)が必要な場合は、ApplicationImpersonation を使用します。それ以外の場合、ApplicationImpersonation を使用しません。
    
  - X-PreferServerAffinity ヘッダーを含め、値を true に設定します。 手順 2 で作成した **ExchangeService** オブジェクトを使用している場合、この値は自動的に含められます。 
    
  - グループの X-backendoverridecookie (アンカーメールボックスユーザーのサブスクリプション応答で返された X-backendoverridecookie) を含めます。 手順 2 で作成した **ExchangeService** オブジェクトを使用している場合、この値は自動的に含められます。 
    
8. 返されたイベントを別のスレッドに渡して処理します。
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>考慮に入れる必要がある調整の値は何ですか？
<a name="bk_throttling"> </a>

通知の実装を計画する際には、2つの値を考慮する必要があります。接続数、およびサブスクリプション数。 次の表に、各[調整](ews-throttling-in-exchange.md)の設定の既定値と設定の使用方法を示します。 値ごとに、割り当て量が、対象のメールボックスに割り当てられます。 このため、多くのシナリオで、追加の接続を得るために偽装を使用することが必要な手順となります。 
  
**表1既定の調整値**

|**考慮すべき領域**|**調整設定**|**既定値**|**説明**|
|:-----|:-----|:-----|:-----|
|ストリーミング接続  <br/> |既定の接続切断の制限  <br/> |Exchange Online では 10  <br/> Exchange 2013 では 3  <br/> |アカウントがサーバー上で同時に開くことができる同時ストリーミング接続の最大数。 この制限内で作業するには、対象のメールボックスに割り当てられている ApplicationImpersonation の役割を持つサービス アカウントを使用して、ストリーミングされたイベントを取得するときに、各サブスクリプション ID のグループの最初のユーザーを偽装します。  <br/> |
|プルまたはプッシュの接続  <br/> |EWSMaxConcurrency  <br/> |27  <br/> |アカウントがサーバー上で同時に開いておくことができる並行プルまたはプッシュの最大接続数 (受信されているが、まだ応答されていない要求)。  <br/> |
|サブスクリプション  <br/> |EWSMaxSubscriptions  <br/> |Exchange Online では 20  <br/> Exchange 2013 では 5000  <br/> |アカウントが同時に持つことができる、期限が切れていないサブスクリプションの最大数。この値は、サーバーでサブスクリプションが作成されたときに減少します。  <br/> |
   
次の例は、ターゲットメールボックスと、ターゲットメールボックスに対して[Applicationimpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)役割が割り当てられているサービスアカウントの間で、予算がどのように処理されるかを示しています。 
  
- ServiceAccount1 (sa1) は、(m1、m2、m3 など) の多くのユーザーを偽装し、メールボックスごとにサブスクリプションを作成します。サブスクリプションが作成されると、サブスクリプションの所有者は sa1 となり、sa1 がサブスクリプションとの接続を開くと、EWS が強制してサブスクリプションが sa1 に所有されます。
    
- sa1 は、次の方法で接続を開くことができます。
    
1. 偽装をせず、接続が sa1 に対して課金されます。
    
2. ユーザーのいずれか (たとえば、m1) を偽装することによって、接続が m1's の予算のコピーに対して課金されるようにします。 (M1 自体は Exchange Online を使用して10個の接続を開くことができ、m1 を偽装するすべてのサービスアカウントは、コピーされた予算を使用して10個の接続を開くことができます)。
    
- 接続制限に達した場合、次の回避策を利用できます。
    
  - オプション 1 が使用されている場合、管理者は、追加のユーザーを偽装するように複数のサービス アカウントを作成できます。
    
  - オプション 2 が使用されている場合、コードが別のユーザー (m2 など) を偽装できます。
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>例:サブスクリプション グループとメールボックス サーバー間のアフィニティを維持する
<a name="bk_ce"> </a>

それでは、アクションを見てみましょう。 次のコード例は、ユーザーをグループ化し、X-AnchorMailbox ヘッダー、X-PreferServerAffinity ヘッダー、および X-BackendOverrideCookie Cookie を使用して、メールボックス サーバーとのアフィニティを維持する方法を示します。 ヘッダーおよび Cookie はアフィニティのストーリーの中で重要であるため、この例は、EWS の XML 要求と応答に焦点を当てています。 EWS マネージ API を使用して、サブスクリプション要求と応答の本文を作成するには、「exchange[での ews を使用したメールボックスイベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」と「 [EXCHANGE での ews を使用したメールボックスイベントに関するプル通知](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」を参照してください。 このセクションには、アフィニティを維持し、要求にヘッダーを追加するための、特定の追加の手順が含まれています。
  
この例では、4 人のユーザーとして alfred@contoso.com、alisa@contoso.com、ronnie@contoso.com、および sadie@contoso.com が含まれています。次の図では、ユーザーの GroupingInformation と ExternalEwsUrl の[自動検出の設定](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)を示します。 
  
**図1。メールボックスのグループ化に使用される自動検出の設定**

![各ユーザーの GroupingInformation および ExternalEwsUrl の値を表示している表。](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
自動検出応答からの設定を使用して、GroupingInformation と ExternalEwsUrl の設定の連結された値により、メールボックスがグループ化されます。この例では、Alfred と Sadie は同じ値を持つ 1 つのグループであり、Alisa および Ronnie は別のグループにいて同じ値を共有しています。
  
**図2メールボックスグループの作成**

![Autodiscover 設定を使用してどのようにメールボックス グループが作成されるかを示した表。](media/Exchange2013_NotificationAffinityGrouping.png)
  
この例の目的のために、グループ A に注目します。グループ B と同じ手順を使用しますが、そのグループには別の X-anchormailbox 値を使用します。
  
[Applicationimpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)を使用して、アンカーメールボックスのサブスクリプション要求 (alfred@contoso.com) を作成し、x-anchormailbox ヘッダーを自分の電子メールアドレスに設定し、x-x-preferserveraffinity header 値を true に設定します。 これらの2つのヘッダー値を設定すると、サーバーによって応答の X-backendoverridecookie が作成されます。
  
EWS マネージ API を使用している場合は、次に示すように、 [Httpheaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)の[add](https://msdn.microsoft.com/library/cy7xta5e)メソッドを使用して、2つのヘッダーをサブスクリプション要求に追加します。 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

そのため、このような形式のサブスクリプション要求は次のようになります。
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

次の XML メッセージは、Alfred のサブスクリプション要求に対する応答で、X-backendoverridecookie が含まれています。 このグループ内のユーザーのすべての後続の要求に対して、この Cookie を再送信します。 応答には、Exchange 2010 で使用されている exchangecookie Cookie など、追加の Cookie も含まれていることに注意してください。 Exchange Online 、Office 365 の一部としての Exchange Online、および Exchange 2013 以降のバージョンの Exchange は、後続のサブスクリプション要求に含まれている場合に、exchangecookie を無視します。
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

X-backendoverridecookie を Alfred の応答と X-anchormailbox ヘッダーで使用すると、サブスクリプション要求が s e に対して作成され、その他のグループのサブスクリプション要求は次のようになります。
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
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

このように、サブスクリプション応答は次のようになります。 X-BackEndOverrideCookie が含まれていないことに注意してください。 以降の要求では、クライアントがその値をキャッシュします。
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

サブスクリプション応答からの [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) の値を使用して、[GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) 操作の要求がグループ内のすべてのサブスクリプションに対して作成されました。このグループのサブスクリプションが 200 未満であるため、すべて 1 つの要求で送信されます。X-PreferServerAffinity ヘッダーが true に設定され、X-BackEndOverrideCookie が含められます。  
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Exchange 2010 では、図 3 に示すようにサブスクリプションがクライアント アクセス サーバーで維持されます。 Exchange 2010 以降のバージョンの Exchange では、図 4 に示すようにメールボックス サーバーでサブスクリプションが維持されます。
  
**図 3.Exchange 2010 でアフィニティを維持するためのプロセス**

![Exchange 2010 のクライアント アクセス サーバーで、アクティブ サブスクリプションのテーブルがどのように維持されるかを示す図。](media/Exchange2013_NoficationAffinity2010.png)
  
**図 4.Exchange Online および Exchange 2013 でアフィニティを維持するためのプロセス**

![ロード バランサーおよびクライアント アクセス サーバーが、要求をどのように Exchange Server および Exchange Online でアクティブ サブスクリプションのテーブルを維持するメールボックス サーバーにルーティングするかを示す図。](media/Exchange2013_NoficationAffinity2013.png)
  
Exchange 2010 では、クライアントはロード バランサーのアドレスのみを認識し、サーバーによって返される exchangecookie により、要求が適切なクライアント アクセス サーバーにルーティングされます。 ただし、それ以降のバージョンでは、ロード バランサーとクライアント アクセス サーバーの役割の両方で、メールボックス サーバーに到達する前に、適切に要求をルーティングする必要があります。 そのためには追加情報が必要であり、これが新しいヘッダーおよび Cookie が導入された理由です。 記事「[Exchange での通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)」では、Exchange 2013 でサブスクリプションを維持する方法について説明しています。 
  
Exchange 2010 が使用する exchangecookie が、以降のバージョンで依然として返されることに気付くかもしれません。 この cookie を要求に含めるには害はありませんが、それ以降のバージョンの Exchange は無視します。
  
## <a name="see-also"></a>関連項目

- [Exchange の通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Exchange での EWS を使用したメールボックス イベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Exchange での EWS を使用したメールボックス イベントに関するプル通知](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
- [EWS サブスクリプションのアフィニティの管理の変更...](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [Exchange での EWS 調整](ews-throttling-in-exchange.md)
    

