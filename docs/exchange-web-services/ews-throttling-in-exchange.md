---
title: Exchange での EWS 調整
manager: sethgros
ms.date: 05/10/2019
ms.audience: Developer
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。
localization_priority: Priority
ms.openlocfilehash: 27db12c01180abbaf92b5b9a09a072212b6012ec
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012553"
---
# <a name="ews-throttling-in-exchange"></a>Exchange での EWS 調整

Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。

**著者:** Glen Scales、Michael Mainer (Microsoft Corporation)

The article provides information about EWS throttling in Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange 2010. Throttling in Exchange helps to ensure server reliability and uptime by limiting the amount of server resources that a single user or application can consume. Throttling is a reactive response to overuse of system resources that may affect service reliability and functionality. Exchange constantly monitors the health of critical infrastructure resources, such as mailbox databases. When high load factors are detected that degrade the performance of these resources, EWS connections are throttled proportionally based on the amount that each caller has contributed to this high load condition. The result is that a user may be within their throttling limit and still experience slowdowns until the health of the resource is back to operational levels.

Each client access protocol in Exchange, including EWS, has a throttling policy. When you design applications that use EWS, it is important to account for throttling policies, to help ensure application reliability and the health of your Exchange server. This article identifies the different throttling policies and service limits for EWS, whether you are targeting Exchange Online or versions of Exchange on-premises starting with Exchange Server 2010. As applicable, this article also identifies differences in throttling policies in different versions of Exchange.

> [!IMPORTANT]
> Default throttling policy, access to throttling policy, and throttling policy configuration differs between Exchange Online and Exchange on-premises. Specific throttling setting values are only accurate for a specific version of Exchange. Because setting values vary across versions, and because Exchange administrators can change the default throttling policies for on-premises deployments, this article does not provide the default setting values. It is more important for you to be aware of the considerations for designing an application that functions within throttling limits and reacts appropriately to throttling scenarios.

アプリケーション開発者である場合は、アプリケーションデザインに対する調整を考慮する必要があります。 Exchange のバージョンによって、EWS 調整パラメーターの既定値が異なります。 異なるバージョンの Exchange にアクセスするように設計されたクライアントおよびサービスアプリケーションは、これらの設定を考慮する必要があります。これらの設定には、既定値、Exchange 管理者が設定したカスタム値、Exchange Online の場合と同様に、既定で設定され、検出可能ではありません。 調整パラメーターの値はプログラムによって検出できないため、さまざまな調整の制限に適応させるためのアプリケーションの計画がクライアント設計仕様に含まれている必要があります。 多数のメールボックスにアクセスするマルチスレッドアプリケーションを設計する場合、または多数のクライアントが同じメールボックスにアクセスする場合は、既定のポリシーが Exchange に適用される同時実行の制限を考慮してください。

## <a name="throttling-policies-that-affect-ews"></a>EWS に影響を与える調整ポリシー

Exchange の調整ポリシーは、EWS だけでなく、Office Outlook、Outlook Web App、Exchange ActiveSync によって使用されるプロトコルを含む、Exchange サーバーへのすべてのクライアント接続にも影響します。

Exchange 2010 を実行している場合、**CPUStartPercent** 調整ポリシーは EWS のパフォーマンスに影響を与える可能性があります。 クライアント アクセス サーバー上で実行される Exchange プロセス (EWS プロセスなど) の平均 CPU 使用率がこのポリシーで指定された値を超えると、受信要求が遅れて、CPU 使用率を減少させます。 このポリシーの値を変更することはできませんが、これを理解しているとパフォーマンスの問題のトラブルシューティングに役立つことがあります。 この値に対してクライアント アクセス サーバーが実行するサンプリングのロジックは、10 秒間のローリング ウィンドウの平均です。 これにより、プロセスが CPU 使用率の急なスパイクに適切に対応できます。 このしきい値を超えた場合、EWS への受信接続が遅延します。 この遅延の上限は、CPU 使用率が 100% (理論上でしかあり得ない数字) の場合、EWS 要求あたり 500 ミリ秒 (msec) です。 100 項目を取得するバッチ EWS 要求が渡されると、サーバーは CPU 使用率を 100 回 (1 項目あたり 1 回) 確認し、最大で 50 秒の遅延になります。 遅延時間は、CPU 使用率に直線的に比例します。 **CPUStartPercent** では、遅延は 0 であり (1 つのスレッドが生成)、CPU 使用率が 100% の場合に 500 ミリ秒まで直線的に増加します。 調整ポリシーはすべての Exchange ユーザーに適用されるため、CPU 使用率が Exchange クライアント アクセス サーバーの **CPUStartPercent** の制限を超過することはないと考えられます。これは、サーバーの運用に影響するほどの CPU 使用率を個々のユーザーまたはアプリケーションで占めることはできないためです。

次の表は、EWS を使用するアプリケーションに影響を与える調整ポリシー パラメーターをまとめています。

**表 1. EWS に影響を与える調整ポリシー パラメーター**

|**調整ポリシー パラメーター名**|**適用対象**|**説明**|
|:-----|:-----|:-----|
|**DiscoveryMaxConcurrency** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが同時に接続できる同時探索検索の数を指定します。  <br/> |
|**DiscoveryMaxKeywords** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが探索検索に含めることができるキーワードの最大数を指定します。  <br/> |
|**DiscoveryMaxKeywordsPerPage** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |統計情報を表示するキーワードの数を指定します。  <br/> |
|**DiscoveryMaxMailboxes** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが探索検索に含めることができるソース メールボックスの最大数を指定します。  <br/> |
|**DiscoveryMaxMailboxesResultsOnly** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |インプレースの電子情報開示検索において、統計情報の表示は不可であっても検索可能なメールボックスの最大数を指定します。  <br/> |
|**DiscoveryPreviewSearchResultsPageSize** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |電子情報開示検索のプレビューの応答で返されるメッセージの数を指定します。  <br/> |
|**EwsCutoffBalance** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |EWS ユーザーのリソース消費制限を定義し、これを超えたら特定のコンポーネントの操作を実行できないよう、ユーザーを完全にブロックするようにします。  <br/> |
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Defines the amount of time that an EWS user can consume an elevated amount of resources before being throttled. This is measured in milliseconds. This value is set separately for each component.  <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |予算時間中に EWS ユーザーの予算を回復する速度 (予算の増加単位) を定義します。  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Defines the maximum number of active push, pull, and streaming notification subscriptions that a user can have on a specific Client Access server at one time. This is budgeted differently for different Exchange versions.  <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |EWS で Exchange Search を使用して行われる高速な検索を続けて、タイムアウトするまでの時間を秒単位で定義します。高速な検索は、[FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)の高度な検索テクニック (AQS) のクエリ文字列を使用して行われる検索です。  <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |クライアント アクセス サーバーのメモリ内で、1 人のユーザーに対して一度に存在できる [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)または [FindFolder 操作](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)からの項目の最大数を定義します。 このプロパティの既定値は 1000 です。 この値の[フォールバック値](https://technet.microsoft.com/library/dd297964%28v=exchg.141%29.aspx#fallback)は 1000 です。  <br/> In Exchange Online and on-premises versions of Exchange starting with Exchange 2013, this throttling policy cannot be queried or configured by a cmdlet. In Exchange Online and on-premises versions of Exchange starting with Exchange 2013, the EWSFindCountLimit for [AQS search](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) and any Exchange search with a restriction is 250 results. An Exchange search without a restriction will return up to 1000 results.  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |特定のユーザーが Active Directory の要求を実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |特定のユーザーがクライアント アクセス サーバーのコードを実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |特定のユーザーがメールボックス RPC の要求を実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Defines the number of concurrent open connections that a specific user can have against an Exchange server that is using EWS at one time. The default value for Exchange 2010 is 10. The default value for Exchange 2013 and Exchange Online is 27.  <br/> このポリシーは、ストリーミング通知以外のすべての操作に適用されます。 ストリーミング通知では、利用可能な開かれたストリーミング イベント接続の数を示すために **HangingConnectionLimit** を使用します。 詳細については、「[考慮に入れる必要がある調整の値](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)」をご覧ください。  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |送信可能な 1 分あたりのメッセージ数を定義します。  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中にユーザーが宛先として指定できる受信者数の制限を定義します。  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中に受信トレイの転送またはリダイレクト操作の対象にできる受信者数の制限を定義します。  <br/> |
|**ConcurrentSyncCalls** <br/> |Exchange 2019  <br/> Exchange 2016  <br/> Exchange Online  <br/> |ユーザーの同時同期呼び出し数 (SyncFolderHierarchy、Syncfolderhierarchy) の数に対する制限を定義します。 <br/> |

> [!CAUTION]
> 調整ポリシーを **null 値**に設定しないでください。 そのように設定すると、ポリシーは無制限に等しい設定になり、これは調整ポリシーが設定されていないことを示します。

## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Exchange のメールボックスに適用するポリシーを表示する

Exchange on-premises provides Exchange Management Shell cmdlets that you can use to set and get throttling policy. Exchange Online does not provide access to the throttling policy cmdlets.

次のコマンドレットを使用して、オンプレミスの Exchange Server の展開の調整ポリシーを表示できます。

- **Get-ThrottlingPolicy** — 1 つ以上の調整ポリシーに関するクライアント調整設定を取得します。 詳細については、TechNet の「 [new-throttlingpolicy](https://technet.microsoft.com/library/dd351264.aspx) 」を参照してください。

- **Get-ThrottlingPolicyAssociation** – オブジェクトとそれに関連付けられた調整ポリシーとの間の関係を表示できます。 選択できるオブジェクトは、メールボックスを持つユーザー、メールボックスを持たないユーザー、または連絡先です。 詳細については、TechNet の「[Get-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459241.aspx)」を参照してください。

Exchange 2010 の既定の調整ポリシーを表示するには、次のコマンドを使用します。

**Get-ThrottlingPolicy | Where-Object {$_.IsDefault -eq "True"} | format-list**

Exchange 2013 のグローバル調整ポリシー (Exchange 2010 の既定の調整ポリシーに等しい) を表示するには、次のコマンドを使用します。

**Get-ThrottlingPolicy | Where-Object {$_.ThrottlingPolicyScope -eq "Global"} | format-list**

Use the following command to show the throttling policy associated with a user in Exchange 2010 or Exchange 2013. Replace the user name john@contoso.com with the user name of the target user for whom you want to get throttling policy information.

**Get-ThrottlingPolicyAssociation john@contoso.com | format-list**

Exchange 管理シェルでこのコマンドを実行すると、次のような出力が生成されます。

```powershell
PS C:\>Get-ThrottlingPolicyAssociation john@contoso.com
RunspaceId               : 72153d6-9dce-2fae-8dbd-5ca5f760g2df
ObjectId                 : john
ThrottlingPolicyId       :
Name                     : john
Identity                 : FHXB-28178dom.contoso.com/Users/john
IsValid                  : True
NeedsToSuppressPii       : False
ExchangeVersion          : 0.10 (15.0.0.0)
DistinguishedName        : CN=john,CN=Users,DC=FHXB-28178dom,DC=contoso,DC=com
Guid                     : 2c10dab6-de28-1937-ad8g-535832613a08
```

> [!NOTE]
> **ThrottlingPolicyId** のプロパティが空白の場合、既定のポリシーがメールボックスに適用されます。

[Set-ThrottlingPolicy](https://technet.microsoft.com/library/dd298094.aspx) コマンドレットと [Set-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459231.aspx) コマンドレットを使用して、Exchange サーバーで調整ポリシーを設定できます。 既定以外の調整ポリシーは、 [new-throttlingpolicy](https://technet.microsoft.com/library/dd351045.aspx)および[new-throttlingpolicy](https://technet.microsoft.com/library/dd351178.aspx)コマンドレットを使用して作成および削除できます。

> [!TIP]
> We recommend that you design your applications to adhere to the default throttling policy. Only make changes to default throttling policies if your client application design cannot accommodate the default policy. Be aware that less restrictive throttling policies can negatively affect service reliability.

## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>EWS の偽装を使用するアプリケーションの調整の考慮事項

[Impersonation](impersonation-and-ews-in-exchange.md) is an authorization method that enables a single account to access many accounts. When a service account impersonates users, it acts as the users and therefore assumes the rights that are assigned to those users. Log files record the access as the impersonated user. Administrators use role-based access control (RBAC) to configure impersonation via the Exchange Management Shell.

偽装を使用すると、調整のしきい値すべての予算は Exchange のバージョンごとに異なって適用されます。 予算の計算は、偽装される側のアカウントか、サービス アカウントのいずれかに対して行われます。 アプリケーションがマルチスレッド化され、複数のメールボックスに対する同時要求を行う場合は、調整しきい値がアプリケーションのパフォーマンスにどのように影響するかを考慮する必要があります。 一般に、偽装ですべてのメールボックスにアクセスするサービス ベースのアプリケーションを作成するときには、サービス アカウントの次の制限にご注意ください。

- 偽装を使用する場合、サービス アカウントは、次のポリシー パラメーターに関して別個の予算を持ちます。

  - **EWSMaxConcurrency**

  - **EWSPercentTimeInAD**

  - **EWSPercentTimeInCAS**

  - **EWSPercentTimeInMailboxRPC**

  - **EWSMaxSubscriptions**

  - **EWSFastSearchTimeoutInSeconds**

  - **EWSFindCountLimit**

- Exchange 2010 Service Pack 2 (SP2) Update Rollup 4 (RU4) より前のバージョンの Exchange に対して行われるすべての接続に関して、**EWSMaxConcurrency** の予算は、サービス アカウントと偽装される側のアカウントの間で共有されます。 Exchange Online を含め、Exchange 2010 SP2 RU4 以降では、サービス アカウントのアクセスは、ユーザーの **EWSMaxConcurrency** の予算とは別の予算を使用します。 EWS に対する Exchange の同時接続の調整ポリシーの更新の詳細については、「[Exchange Server 2010 Service Pack 2 の更新プログラムのロールアップ 4 について](https://support.microsoft.com/kb/2706690)」をご覧ください。

    EWS streaming notifications in versions of Exchange starting with Exchange 2010, and including Exchange Online, have an additional cloned **EWSMaxConcurrency** budget from all other EWS client connections. Streaming notification connections are counted against a separate budget than all other EWS operations. The streaming notification maximum concurrency budget is actually two different budgets: one budget is for all service accounts, and one budget is for the account being impersonated. Streaming notifications in Exchange Online and versions of Exchange starting with Exchange 2013 use the [HangingConnectionLimit](#throttling-considerations-for-ews-notification-applications) to limit the number of connections.

    たとえば、**EWSMaxConcurrency** が 5 に等しいと仮定しましょう。 ユーザーは 5 つのプル通知接続を開くことができますが、サービス アカウントは、ユーザーと同時に、ユーザーのメールボックスに対して 5 つの並列プル通知接続を行うことができます。

- 次の表で、サービス アカウントと偽造するアカウントとの間で **EWSMaxSubscriptions** の調整の予算を計算する方法について示します。

   **表 2. EWSMaxSubscriptions の予算の計算**

   |**Exchange のバージョン**|**EWSMaxSubscriptions の調整された予算の計算**|
   |:-----|:-----|
   |Exchange Online  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2013  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP3  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP2  <br/> |Charged against the calling account. Starting with Exchange 2010 SP2 RU4, the budget is charged against the target mailbox.  <br/> |
   |Exchange 2010 SP1  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |
   |Exchange 2010  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |

- **EWSMaxSubscriptions** の調整予算は偽装される側のアカウントに対して適用されるため、偽装が使用されている限り、サービス アカウントがストリーミング通知をサブスクライブおよび受信できるメールボックスの数に制限はありません。 偽装されるアカウントでは、対象となるメールボックスごとに _n_ 個を超える同時要求を行うことはできません。ここで _n_ は **EWSMaxSubscriptions** の値です。 偽装を使用していない場合は、同じサービス アカウントで同時要求の合計が _n_ を超えることはできません。 このため、サービス アカウントで偽装を使用することで、提供できるメールボックスの数が指数関数的に増加します。 詳細については、「[Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)」を参照してください。

- The **EWSPercentTimeInMailboxRPC**, **EWSPercentTimeInCAS**, and **EWSPercentTimeInAD** policy parameters refer to actions performed by a single thread. When an application performs multiple concurrent operations, you should account for the cumulative effect of these operations on the user resource budget.

## <a name="throttling-implications-for-ews-batch-requests"></a>EWS のバッチ要求の調整の影響

EWS enables you to batch multiple item requests into a single request that is executed by the Client Access server. This allows for greater efficiency and performance. When an Exchange server executes a batched request, it checks the user's budget after the execution of each item within the batch. If the application is over budget, the processing of the next item in the batch is delayed until the budget for that user has recharged. To ensure that applications that use batch operations run successfully, limit the number of item requests that can be included in a single batch, and divide large batches across multiple smaller batches to increase the reliability of the results. The effect that a batch operation has on particular throttling thresholds depends on the type of the request, the size of the items to be processed (for example in **UploadItems** or **ExportItems** operations) and the mailbox content. Throttling policies affect batch operations by causing the request to take longer to process. The caller will therefore have to wait longer for the response, and, because EWS limits the execution time of a batch request to one minute, the call could time out.

アプリケーションのバッチの最適なサイズを決定するには、様々な入力セットを使用して単体テストを実行し、運用環境でアプリケーションにエラーが発生しないことを確認します。

## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>EWS の検索操作に影響を与える調整ポリシーのパラメーター

[Search operations in EWS](search-and-ews-in-exchange.md) can require large amounts of time and resources, depending on how the search is run and what information is requested. To control resource usage during searches, two policy parameters take effect: **EWSFastSearchTimeoutInSeconds** and **EWSFindCountLimit**.

**EWSFastSearchTimeoutInSeconds** ポリシー パラメーターは、EWS の高速な検索 (コンテンツ インデックス検索とも言う) を実行してタイムアウトするまでの時間を秒単位で指定します。高速な検索は、[FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)で、高度な検索テクニック (AQS) のクエリ文字列を使用して行われる検索です。

Exchange のメールボックス フォルダーの検索には、以下の 2 種類の方法があります。

- Exchange ストアの検索を使用します。これにより、ターゲット検索スコープ内のすべてのメッセージの順次スキャンを実行します。

- Exchange Search サービス (コンテンツ インデックス) を使用します。

Both of these types of searches can result in timeouts. When possible, use the Exchange Search service because these searches are often targeted against mailbox indexes and use AQS queries. The following example shows how to perform an AQS search of the Inbox by using EWS and the Exchange Search service.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

If you can't use an AQS search, avoid using overly complex search filters. Also try to avoid creating search filters based on computed values if the query involves extended MAPI properties. AQS search was introduced in Exchange 2010.

> [!NOTE]
> 複雑な Exchange ストア検索クエリを初めて実行するときは、実行が非常に遅く、タイムアウトになることがあります。その後、クエリはより迅速に応答するようになります。 Exchange ストアの検索クエリ中に発生するバックエンドの Exchange サーバー プロセスの詳細については、TechNet の「[アイテム数の多さと制限付きビューがパフォーマンスに与える影響について](https://technet.microsoft.com/library/cc535025%28EXCHG.80%29.aspx)」を参照してください。 **SearchFilter** を使用すると、類似のクエリを将来実行するときに役立つ動的な制限が作成されますが、これらの制限は動的な性質のため、永続性や信頼性がなく、最長で 3 日後に削除されます。

The **EWSFindCountLimit** policy parameter specifies the maximum number of items from the results of a **FindItem** or **FindFolder** operation that can exist in memory on a Client Access server at the same time for one user. Every item or folder that EWS processes in a **FindItem** or **FindFolder** request is counted against the budget specified in the **EWSFindCountLimit** element. When the response is sent back to the requester, the find count charge for the current call is released. The response the server returns to a requester when the budget is exceeded is based on the **RequestServerVersion** element value and whether the requester specified paging. When the value of the **RequestServerVersion** element indicates Exchange 2010 or an earlier version of Exchange, the server sends a failure response with error code **ErrorServerBusy**. If the value of the **RequestServerVersion** element indicates a version of Exchange starting with Exchange 2010 SP1 or Exchange Online, and the client is using paging, EWS may return a partial result set instead of an error. Your application should expect that EWS might not return all items. If the value of the **IncludesLastItemInRange** element is false, the application should make another **FindItem** or **FindFolder** request with the new offset and continue until the **IncludesLastItemInRange** element returns true.

When you use a **FindItem** or **FindFolder** operation, it is important to use paging. The EWS Managed API enforces the use of paging, but if you are using other methods, such as EWS proxy objects or raw SOAP, you need to explicitly set paging. The following example shows how to use paging in the EWS Managed API.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> The default policy in Exchange limits the page size to 1000 items. Setting the page size to a value that is greater than this number has no practical effect.

同時要求を行うアプリケーションの場合、_EWSFindCountLimit_ 調整パラメーターの値により、部分的な結果セットが返される可能性があることも考慮に入れる必要があります。 次の例では、EWS マネージ API で **MoreAvailable** プロパティを使用して、すべての結果が 1 つのクエリに含まれるようにする方法を示します。

```cs
ItemView iv = new ItemView(1000);
service.TraceEnabled = false;
FindItemsResults<Item> fiResults = null;
Do
{
    fiResults = service.FindItems(WellKnownFolderName.Inbox, iv);
    PropertySet itItemPropSet = new PropertySet(BasePropertySet.IdOnly) { EmailMessageSchema.Body };
    //Process Items in Result Set
    iv.Offset += fiResults.Items.Count;
}
while (fiResults.MoreAvailable == true);
```

## <a name="throttling-policies-and-concurrency"></a>調整ポリシーと同時実行

Concurrency refers to the number of connections from a specific user. A connection is held from the moment a request is received until a response is sent to the requester. If users try to make more concurrent requests than their policy allows, the new connection attempt fails. However, the existing connections remain valid. Throttling policies can affect concurrency in a number of different ways.

The **EWSMaxConcurrency** throttling policy parameter sets the number of concurrent connections that a specific user can have against an Exchange server at one time. To determine the maximum number of concurrent connections to allow, consider the connections that Outlook clients will use. Outlook 2007 and Outlook 2010 use EWS to access availability and Out of Office (OOF) information. Mac Outlook 2011 uses EWS for all client access functionality. Depending on the number of Outlook clients that are actively connecting to a user's mailbox, the number of concurrent connections available for a user might be limited. Also, if your application has to connect to multiple mailboxes simultaneously while using a single security context, it is important to take the value of the **EWSMaxConcurrency** policy into account. For more information about using a single security context with concurrent connections, see [Throttling considerations for applications that use EWS impersonation](#throttling-considerations-for-applications-that-use-ews-impersonation) earlier in this article.

Applications that concurrently connect to multiple mailboxes have to be able to track resource usage on the client side. Because EWS operations are request/response-based, you can ensure that your applications function well within the **EWSMaxConcurrency** threshold by tracking the number of connections that occur between the start of a request and when the response is received and ensuring that no more than ten open requests occur concurrently.

**EWSFindCountLimit** ポリシー パラメーターは、**FindItem** または **FindFolder** の操作がクライアント アクセス サーバー上で 1 人のユーザーに対して同時に使用できる結果の最大サイズを指定します。 1 つのアプリケーション (複数のアプリケーションの可能性もあります) が特定のユーザーのためにそれぞれ 100 項目を返す 2 つの同時 EWS **FindItem** 要求を行う場合、その特定のユーザーの予算に対する **EWSFindCountLimit** の使用分は 200 になります。 最初の要求を返すときに予算は 100 まで下がり、2 番目の要求を返すときに予算はゼロまで下がります。 同じアプリケーションが 1000 項目の 2 つの同時要求を行う場合、予算の値は 2000 項目になり、**EWSFindCountLimit** の値を超えます。 項目に対するユーザーの予算がゼロを下回る場合、ユーザーの予算が 1 以上に回復するまで、次の要求がエラーになります。

## <a name="throttling-considerations-for-ews-notification-applications"></a>EWS 通知アプリケーションに関する調整の考慮事項

プッシュ、プル、またはストリーミング通知を利用する EWS 通知アプリケーションを作成する場合、**EWSMaxSubscriptions** および **EWSMaxConcurrency** 調整ポリシーと **HangingConnectionLimit** の影響をご考慮ください。

**EWSMaxSubscriptions** ポリシー パラメーターは、ユーザーが特定のクライアント アクセス サーバーに対して同時に保持できるアクティブなプッシュ、プル、ストリーミング サブスクリプションの最大数を指定します。 このパラメーターの既定値は Exchange のバージョンごとに異なります。 ユーザーは **SubscribeToAllFolders** プロパティを使用して、メールボックス内のすべてのフォルダーをサブスクライブできます。これは **EWSMaxSubscriptions** の予算に対して 1 つのサブスクリプションを使用します。 ユーザーは個別のフォルダーをサブスクライブできます。各フォルダーのサブスクリプションが **EWSMaxSubscriptions** の予算に対してカウントされていき、最大で **EWSMaxSubscriptions** パラメーターの値で設定された制限にまで至ります (たとえば、**EWSMaxSubscriptions** が 20 に設定されている場合、ユーザーは様々なメールボックスの 20 の予定表フォルダーをサブスクライブできます)。

偽装と **EWSMaxSubscriptions** パラメーターの詳細については、この記事で前述した「[EWS の偽装を使用するアプリケーションの調整の考慮事項](#throttling-considerations-for-applications-that-use-ews-impersonation)」をご覧ください。

**EWSMaxConcurrency** ポリシー パラメーターが EWS 通知で問題になる可能性があります。例を挙げます。

- EWS がサブスクリプションの所有者の接続数を増分させる一方で、プッシュ サブスクリプションによって通知が生成される場合。

- アプリケーションが複数のユーザーのメールボックスをリッスンするように設計されており、配布リストに送信されたメッセージのインスタンスに関する同時の通知をユーザーたちが受信する場合。

通知アプリケーションがマルチスレッドで、同時に接続要求を行って、ユーザーアカウントによって受信された特定のメッセージに関する詳細情報を取得する場合は、 **Ewsmaxconcurrency**ポリシーの制限を超えることができます。 これに対処するには、サーバーが使用するものも含めて同時接続をアプリケーションで監視し、クライアントに要求のキューを実装することをご検討ください。

**HangingConnectionLimit**は、ストリーミング通知にのみ適用されます。 この制限は web.config ファイルで設定されます。 Exchange 管理者はオンプレミスの Exchange サーバーでこの値を設定できますが、exchange Online のメールボックスではこの制限の既定値を使用する必要があります。これは、exchange Online、Exchange 2019、Exchange 2016、exchange 2013 の場合は10です。 詳細については、「[考慮する必要のある調整値](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)」を参照してください。

## <a name="throttling-policy-and-application-performance"></a>調整ポリシーとアプリケーションのパフォーマンス

**PercentTimeIn** 調整ポリシーの次の 3 つのパラメーターは、EWS アプリケーションがクライアント アクセス サーバー上で使用できる時間数に影響します。 

- **EWSPercentTimeInAD**

- **EWSPercentTimeInCAS**

- **EWSPercentTimeInMailboxRPC**

The values specified in the **PercentTimeIn** policy parameters indicate the amount of time that one thread making one request is allocated. For example, assuming a **EWSPercentTimeInCAS** value of 90, if a process makes two concurrent requests that spend 54 seconds each running code on the Client Access server, the process uses 108 seconds in a 60 second window. This represents an **EWSPercentTimeInCAS** parameter value of 180 percent.

> [!NOTE]
> The **EWSPercentTimeInCAS** parameter value is an overlapping superset of the **EWSPercentTimeInAD** and **EWSPercentTimeInMailboxRPC** parameter values. This means that the expenditure in Client Access server processing time will always be larger than the expenditures in **EWSPercentTimeInAD** and **EWSPercentTimeInMailboxRPC**. This is because for the Exchange component to make an Active Directory or RPC call, it must already be running Client Access server code. In addition, the expenditure in processing time for **EWSPercentTimeInCAS** doesn't stop while LDAP or RPC calls are being made. Although the request might be synchronously waiting for a response from Active Directory Domain Services (AD DS) or the Exchange store, the process is still consuming a thread on the server, and therefore the thread should continue to be charged for that usage.

アプリケーションが60秒以内に実行される CPU 時間の量は、これらの調整制限を超える可能性があります。そのため、要求の量と種類を考慮することが重要です。 たとえば、同時に実行される**ResolveNames**操作の大きなバッチは、 **EWSPercentTimeInAD** policy パラメーターの値を超える場合があります。 既定の調整ポリシーに含まれているポリシー値は、ほとんどの EWS アプリケーションが問題なく機能するように設計されています。ただし、マルチスレッドの高ボリュームアプリケーションでは、1つの特定のクライアントアクセスサーバーに大量の要求が配置されると、問題が発生する可能性があります。 これを回避するには、サーバーに対して実行するバッチのサイズを制限することを検討してください。

## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>調整ポリシーと、大量の電子メールを送信するアプリケーション

既定の調整ポリシーには、EWS を使用して大量のメッセージを送信したり、短期間で大量のメッセージを送信したりするアプリケーションに影響を与える可能性がある、3 つのレート制限ポリシー パラメーターがあります。

> [!NOTE]
> In general, we recommend that you do not use EWS to send bulk email. Use an SMTP host that specializes in bulk mail services to submit frequent large bulk email messages.

The **MessageRateLimit** policy parameter specifies the number of messages per minute that can be submitted by any Exchange client, including EWS. By default, this policy is set to 30 messages per minute. For ordinary users, this is generally sufficient. However, applications that send large batches of email messages, for example as part of an invoicing program, can run into problems. When this policy limit is exceeded, message delivery for the mailbox is delayed. Specifically, messages will appear in the Outbox or Drafts folder for longer periods of time when a user or application submits a larger number of messages than the value specified by the **MessageRateLimit** parameter. Be sure to consider this when you are developing a delivery tracking system, especially if your application uses a mailbox that users connect to via Outlook. When deferred items are stored in the Outbox or drafts folder, users might interpret that as an error.

The **RecipientRateLimit** policy parameter specifies the limit on the number of recipients that a user can address in a 24-hour period. For example, if this value is set to 500, it means that a single Exchange mailbox account can send messages to no more than 500 recipients each day. This limit applies to messages to recipients that are inside and outside the organization. This default limit might cause problems for some line-of-business applications that do end-of-month invoice runs and need to send messages to more than this number of recipients. You can use external services that enable batch processing of messages or separate on-premises outbound relay solutions to work around this limitation.

The **ForwardeeLimit** policy parameter specifies the maximum number of recipients that messages can be forwarded or redirected to by means of Inbox rules. This parameter doesn't limit the number of messages that can be forwarded or redirected to the recipients.

## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>調整の制限を超過したときに生成されるエラー

調整ポリシーを超過すると、EWS は次の表に記載するエラーのいずれかを生成します。

**表 3. 調整制限のエラー**

|**エラー**|**調整ポリシー パラメーター**|**説明**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |サーバーに対する同時要求が、ユーザーのポリシーで許可されているものより多いことを示します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |ユーザーの調整ポリシーのサブスクリプションの最大数を超過したことを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |検索操作の呼び出しが、返すことのできる項目の合計数を超えたことを示します。  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |Occurs when the server is busy. The BackOffMilliseconds value returned with ErrorServerBusy errors indicates to the client the amount of time it should wait until it should resubmit the request that caused the response that returned this error code.  <br/> |

次の表は、調整エラーによって返される HTTP ステータス コードを示します。

**表 4. 調整エラーによって返される HTTP ステータス コード**

|**HTTP ステータス コード**|**説明**|
|:-----|:-----|
|HTTP 503  <br/> |Indicates that EWS requests are queuing with IIS. The client should delay sending additional requests until a later time.  <br/> |
|HTTP 500  <br/> |Indicates an internal server error with the ErrorServerBusy error code. This indicates that the client should delay sending additional requests until a later time. The response may contain a back off hint called BackOffMilliseconds. If present, the value of BackOffMilliseconds should be used as the duration until the client resubmits a request.  <br/> |
|HTTP 200  <br/> |Contains an EWS schema-based error response with an ErrorInternalServerError error code. An inner ErrorServerBusy error code may be present. This indicates that the client should delay sending additional requests until a later time.  <br/> |

## <a name="see-also"></a>関連項目

- [Exchange ワークロード管理](https://technet.microsoft.com/library/jj150503.aspx)
- [New-ThrottlingPolicy コマンドレット](https://technet.microsoft.com/library/dd351045.aspx)
- [クライアント調整ポリシーについて](https://technet.microsoft.com/library/dd297964.aspx)
- [ThrottlingPolicy クラス](https://msdn.microsoft.com/library/ff342496%28v=EXCHG.140%29.aspx)
- [調整ポリシーと EWSFindCountLimit](https://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [IIS ログの予算のスナップショット](https://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)

- [Exchange 2010 SP1 の展開の調整の効果](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Exchange 2010 SP1 の調整ポリシーの関連付け](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [調整ポリシーと CPUStartPercent](https://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Exchange での認証と EWS](impersonation-and-ews-in-exchange.md)
