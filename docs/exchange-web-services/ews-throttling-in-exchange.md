---
title: Exchange での EWS 調整
manager: sethgros
ms.date: 05/10/2019
ms.audience: Developer
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。
localization_priority: Priority
ms.openlocfilehash: 0c6ac49629ad4cdb4419cc8638d8e60ecb6509d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455402"
---
# <a name="ews-throttling-in-exchange"></a>Exchange での EWS 調整

Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。

**著者:** Glen Scales、Michael Mainer (Microsoft Corporation)

この記事は、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2010 以降のオンプレミス バージョンの Exchange の EWS の調整に関する情報を提供します。Exchange の調整は、1 人のユーザーまたは 1 つのアプリケーションが使用できるサーバー リソースの量を制限して、サーバーの信頼性と稼働時間を確保するのに役立ちます。調整は、サービスの信頼性と機能に影響を与える可能性があるシステム リソースの過剰使用への事後対応です。Exchange は常に、メールボックス データベースなどの重要なインフラストラクチャ リソースの稼働状態を監視します。これらのリソースのパフォーマンスを低下させる高負荷の要因が検出された場合、EWS の接続は、各呼び出し元がこの高負荷状態に関与する量に比例して調整されます。結果として、あるユーザーが調整制限内に収まっていても、リソースの稼働状態が運用レベルに戻るまで、パフォーマンス低下が発生する可能性があります。

EWS を含む、Exchange のクライアント アクセス プロトコルには、それぞれ調整ポリシーがあります。EWS を使用するアプリケーションを設計するときに、アプリケーションの信頼性と Exchange サーバーの正常性を確保できるように、調整ポリシーについて考慮することは重要です。この記事では、Exchange Online と Exchange Server 2010 以降のバージョンの Exchange On-Premises のどちらを対象としているかを問わず、EWS の様々な調整ポリシーやサービスの制限を示します。必要に応じて、この記事では様々なバージョンごとの Exchange の調整ポリシーの違いも示します。

> [!IMPORTANT]
> 既定の調整ポリシー、調整ポリシーへのアクセス、調整ポリシーの構成は、Exchange Online と Exchange On-Premises で異なります。特定の調整設定の値は、Exchange の特定のバージョンにのみ該当します。設定値はバージョン間で異なり、オンプレミスの展開では Exchange の管理者が既定の調整ポリシーを変更できるため、この記事では既定の設定値を示しません。より重要なのは、調整の制限内で機能し、調整のシナリオに合わせて適切に対応するアプリケーションを設計するための考慮事項に注意することです。

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
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |増加したリソースを EWS ユーザーが消費できる時間の長さを定義し、これを超えたら調整を行うようにします。これは、ミリ秒単位で測定されます。この値は、コンポーネントごとに個別に設定されます。   <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |予算時間中に EWS ユーザーの予算を回復する速度 (予算の増加単位) を定義します。  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが特定のクライアント アクセス サーバーに対して同時に保持できるアクティブなプッシュ、プル、ストリーミング通知のサブスクリプションの最大数を定義します。この予算は Exchange のバージョンごとに異なります。   <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |EWS で Exchange Search を使用して行われる高速な検索を続けて、タイムアウトするまでの時間を秒単位で定義します。高速な検索は、[FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)の高度な検索テクニック (AQS) のクエリ文字列を使用して行われる検索です。  <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |クライアント アクセス サーバーのメモリ内で、1 人のユーザーに対して一度に存在できる [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)または [FindFolder 操作](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)からの項目の最大数を定義します。 このプロパティの既定値は 1000 です。 この値の[フォールバック値](https://technet.microsoft.com/library/dd297964%28v=exchg.141%29.aspx#fallback)は 1000 です。  <br/> Exchange Online と Exchange 2013 以降のオンプレミス バージョンの Exchange では、この調整ポリシーに対してクエリを実行したり、コマンドレットによってこれを構成したりすることはできません。Exchange Online と Exchange 2013 以降のオンプレミス バージョンの Exchange では、[AQS 検索](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)と制限付きの Exchange Search の EWSFindCountLimit は、250 件の結果です。制限のない Exchange Search は、最大で 1000 件の結果を返します。  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |特定のユーザーが Active Directory の要求を実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |特定のユーザーがクライアント アクセス サーバーのコードを実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |特定のユーザーがメールボックス RPC の要求を実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |EWS を使用している Exchange サーバーに対して特定のユーザーが同時に並列で開くことができる接続の数を定義します。Exchange 2010 の既定値は 10 です。Exchange 2013 および Exchange Online の既定値は 27 です。 <br/> このポリシーは、ストリーミング通知以外のすべての操作に適用されます。 ストリーミング通知では、利用可能な開かれたストリーミング イベント接続の数を示すために **HangingConnectionLimit** を使用します。 詳細については、「[考慮に入れる必要がある調整の値](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)」をご覧ください。  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |送信可能な 1 分あたりのメッセージ数を定義します。  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中にユーザーが宛先として指定できる受信者数の制限を定義します。  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中に受信トレイの転送またはリダイレクト操作の対象にできる受信者数の制限を定義します。  <br/> |
|**ConcurrentSyncCalls** <br/> |Exchange 2019  <br/> Exchange 2016  <br/> Exchange Online  <br/> |ユーザーの同時同期呼び出し数 (SyncFolderHierarchy、Syncfolderhierarchy) の数に対する制限を定義します。 <br/> |

> [!CAUTION]
> 調整ポリシーを **null 値**に設定しないでください。 そのように設定すると、ポリシーは無制限に等しい設定になり、これは調整ポリシーが設定されていないことを示します。

## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Exchange のメールボックスに適用するポリシーを表示する

Exchange On-Premises には、調整ポリシーを設定および取得するために使用できる Exchange 管理シェル コマンドレットが用意されています。Exchange Online は、調整ポリシーのコマンドレットを利用できません。

次のコマンドレットを使用して、オンプレミスの Exchange Server の展開の調整ポリシーを表示できます。

- **Get-ThrottlingPolicy** — 1 つ以上の調整ポリシーに関するクライアント調整設定を取得します。 詳細については、TechNet の「 [new-throttlingpolicy](https://technet.microsoft.com/library/dd351264.aspx) 」を参照してください。

- **Get-ThrottlingPolicyAssociation** – オブジェクトとそれに関連付けられた調整ポリシーとの間の関係を表示できます。 選択できるオブジェクトは、メールボックスを持つユーザー、メールボックスを持たないユーザー、または連絡先です。 詳細については、TechNet の「[Get-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459241.aspx)」を参照してください。

Exchange 2010 の既定の調整ポリシーを表示するには、次のコマンドを使用します。

**Get-ThrottlingPolicy | Where-Object {$_.IsDefault -eq "True"} | format-list**

Exchange 2013 のグローバル調整ポリシー (Exchange 2010 の既定の調整ポリシーに等しい) を表示するには、次のコマンドを使用します。

**Get-ThrottlingPolicy | Where-Object {$_.ThrottlingPolicyScope -eq "Global"} | format-list**

Exchange 2010 または Exchange 2013 のユーザーに関連付けられた調整ポリシーを表示するには、次のコマンドを使用します。ユーザー名 john@contoso.com を、調整ポリシー情報を取得する対象ユーザーのユーザー名で置き換えます。

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
> 既定の調整ポリシーに従うようにアプリケーションを設計することをお勧めします。クライアント アプリケーションの設計が既定のポリシーに対応できない場合にのみ、既定の調整ポリシーに変更を加えてください。制限の少ない調整ポリシーは、サービスの信頼性に悪影響を及ぼす可能性があることにご注意ください。

## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>EWS の偽装を使用するアプリケーションの調整の考慮事項

[偽装](impersonation-and-ews-in-exchange.md)とは、1 つのアカウントで多くのアカウントにアクセスできるようにする認証方法です。サービス アカウントは、ユーザーを偽装するときにユーザーとして動作するため、それらのユーザーに割り当てられている権限を引き継ぐことになります。ログ ファイルには、偽装されたユーザーとしてアクセスが記録されます。管理者は、Exchange 管理シェルを介し、役割ベースのアクセス制御 (RBAC) を利用して偽装を構成します。

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

    Exchange Online を含め、Exchange 2010 以降のバージョンの Exchange の EWS のストリーミング通知には、その他のすべての EWS のクライアント接続からの、複製された追加の **EWSMaxConcurrency** 予算があります。ストリーミング通知の接続は、他のすべての EWS の操作とは別の予算としてカウントされます。ストリーミング通知の最大同時実行の予算は、実際には 2 つの異なる予算です。1 つの予算はすべてのサービス アカウント用で、もう 1 つの予算は偽装される側のアカウント用です。Exchange Online と Exchange 2013 以降のバージョンの Exchange のストリーミング通知では、[HangingConnectionLimit](#throttling-considerations-for-ews-notification-applications) を使用して接続数を制限します。

    たとえば、**EWSMaxConcurrency** が 5 に等しいと仮定しましょう。 ユーザーは 5 つのプル通知接続を開くことができますが、サービス アカウントは、ユーザーと同時に、ユーザーのメールボックスに対して 5 つの並列プル通知接続を行うことができます。

- 次の表で、サービス アカウントと偽造するアカウントとの間で **EWSMaxSubscriptions** の調整の予算を計算する方法について示します。

   **表 2. EWSMaxSubscriptions の予算の計算**

   |**Exchange のバージョン**|**EWSMaxSubscriptions の調整された予算の計算**|
   |:-----|:-----|
   |Exchange Online  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2013  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP3  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP2  <br/> |呼び出し元のアカウントに対して適用されます。Exchange 2010 SP2 RU4 以降では、予算は対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP1  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |
   |Exchange 2010  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |

- **EWSMaxSubscriptions** の調整予算は偽装される側のアカウントに対して適用されるため、偽装が使用されている限り、サービス アカウントがストリーミング通知をサブスクライブおよび受信できるメールボックスの数に制限はありません。 偽装されるアカウントでは、対象となるメールボックスごとに _n_ 個を超える同時要求を行うことはできません。ここで _n_ は **EWSMaxSubscriptions** の値です。 偽装を使用していない場合は、同じサービス アカウントで同時要求の合計が _n_ を超えることはできません。 このため、サービス アカウントで偽装を使用することで、提供できるメールボックスの数が指数関数的に増加します。 詳細については、「[Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)」を参照してください。

- **EWSPercentTimeInMailboxRPC**、**EWSPercentTimeInCAS**、**EWSPercentTimeInAD** のポリシー パラメーターは、1 つのスレッドによって実行されるアクションを表します。アプリケーションが複数の同時操作を実行するときは、ユーザーのリソースの予算に対するこれらの操作の累積的な影響を考慮する必要があります。

## <a name="throttling-implications-for-ews-batch-requests"></a>EWS のバッチ要求の調整の影響

EWS を使用すると、複数の項目要求をバッチ化して、クライアント アクセス サーバーで実行される単一の要求にまとめることができます。これにより、効率性とパフォーマンスが向上します。Exchange サーバーは、バッチ化された要求を実行するとき、バッチ内の各項目が実行された後にユーザーの予算を確認します。アプリケーションが予算オーバーの場合は、そのユーザーの予算が回復するまで、バッチ内の次の項目の処理が遅延します。バッチ操作を使用するアプリケーションが必ず正常に実行されるようにするには、1 つのバッチに含めることができる項目の要求の数を制限し、大きいバッチを複数の小さいバッチに分割して、結果の信頼性を高めます。バッチ操作が特定の調整しきい値に対して与える影響は、要求の種類、処理する項目のサイズ (**UploadItems** や **ExportItems** の操作などの場合)、およびメールボックスの内容に応じて異なります。調整ポリシーが課されると、要求の処理により長時間を要するため、バッチ操作に影響します。したがって呼び出し元はより長く応答を待機する必要がありますが、EWS はバッチ要求の実行時間を 1 分に制限しているため、呼び出しがタイムアウトする可能性があります。

アプリケーションのバッチの最適なサイズを決定するには、様々な入力セットを使用して単体テストを実行し、運用環境でアプリケーションにエラーが発生しないことを確認します。

## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>EWS の検索操作に影響を与える調整ポリシーのパラメーター

[EWS の検索操作](search-and-ews-in-exchange.md)は、検索を実行する方法と、どのような情報が要求されるかによって、大量の時間とリソースを必要とすることがあります。検索中にリソースの使用状況を制御するには、**EWSFastSearchTimeoutInSeconds** と **EWSFindCountLimit** という 2 つのポリシー パラメーターが有効です。

**EWSFastSearchTimeoutInSeconds** ポリシー パラメーターは、EWS の高速な検索 (コンテンツ インデックス検索とも言う) を実行してタイムアウトするまでの時間を秒単位で指定します。高速な検索は、[FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)で、高度な検索テクニック (AQS) のクエリ文字列を使用して行われる検索です。

Exchange のメールボックス フォルダーの検索には、以下の 2 種類の方法があります。

- Exchange ストアの検索を使用します。これにより、ターゲット検索スコープ内のすべてのメッセージの順次スキャンを実行します。

- Exchange Search サービス (コンテンツ インデックス) を使用します。

これらの種類の検索は、両方ともタイムアウトになることがあります。これらの検索はメールボックスのインデックスを対象とし、AQS クエリを使用しているため、できれば Exchange Search サービスを使用します。次の例では、EWS および Exchange Search サービスを使用して受信トレイの AQS 検索を実行する方法を示します。

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

AQS 検索を使用できない場合は、過度に複雑な検索フィルターを使用しないようにします。また、クエリに拡張 MAPI プロパティが含まれる場合は、計算された値に基づいて検索フィルターを作成しないようにもご注意ください。AQS 検索は Exchange 2010 で導入されました。

> [!NOTE]
> 複雑な Exchange ストア検索クエリを初めて実行するときは、実行が非常に遅く、タイムアウトになることがあります。その後、クエリはより迅速に応答するようになります。 Exchange ストアの検索クエリ中に発生するバックエンドの Exchange サーバー プロセスの詳細については、TechNet の「[アイテム数の多さと制限付きビューがパフォーマンスに与える影響について](https://technet.microsoft.com/library/cc535025%28EXCHG.80%29.aspx)」を参照してください。 **SearchFilter** を使用すると、類似のクエリを将来実行するときに役立つ動的な制限が作成されますが、これらの制限は動的な性質のため、永続性や信頼性がなく、最長で 3 日後に削除されます。

**EWSFindCountLimit** ポリシー パラメーターは、1 人のユーザーに対してクライアント アクセス サーバー上でメモリに同時に存在できる **FindItem** または **FindFolder** 操作の結果の項目の最大数を指定します。**FindItem** または **FindFolder** 要求で EWS が処理するすべての項目やフォルダーが、**EWSFindCountLimit** 要素で指定された予算に対してカウントされます。要求側に応答が送り返されるとき、現在の呼び出しの検索数の使用分が解放されます。予算を超えた場合にサーバーが要求側に返す応答は、**RequestServerVersion** 要素の値と、要求側がページングを指定したかどうかに基づきます。**RequestServerVersion** 要素の値が Exchange 2010 以前のバージョンの Exchange を示す場合、サーバーはエラー コード **ErrorServerBusy** と共にエラー応答を送信します。**RequestServerVersion** 要素の値が Exchange 2010 SP1 以降のバージョンの Exchange、または Exchange Online を示し、かつクライアントがページングを使用している場合、EWS はエラーの代わりに部分的な結果セットを返すことがあります。アプリケーションは、EWS がすべての項目を返さない可能性があることを想定する必要があります。**IncludesLastItemInRange** 要素の値が False の場合、アプリケーションは新しいオフセットを使用してもう一度 **FindItem** または **FindFolder** 要求を実行しなければならず、**IncludesLastItemInRange** 要素が true を返すまでこれを繰り返します。

**FindItem** または **FindFolder** 操作を使用する場合は、ページングを使用することが重要です。EWS マネージ API はページングの使用を強制しますが、EWS プロキシ オブジェクトや、未加工の SOAP など、他の方式を使用する場合は、ページングを明示的に設定する必要があります。次の例では、EWS マネージ API でページングを使用する方法を示します。

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> Exchange の既定のポリシーでは、ページ サイズを 1000 項目に制限します。この数よりも大きい値にページ サイズを設定しても、実際的な効果はありません。

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

同時実行とは、特定のユーザーからの接続の数を指します。接続は、要求が受信された時点から応答が要求側に送信されるまで保持されます。ユーザーがポリシーの許可数を超える同時要求を試みると、新しい接続試行は失敗します。ただし、既存の接続は有効なまま維持されます。調整ポリシーは、様々な方法で同時実行に影響を与える可能性があります。

**EWSMaxConcurrency** 調整ポリシー パラメーターは、Exchange サーバーに対して特定のユーザーが同時に開くことができる接続の数を設定します。許可する同時接続の最大数を判断するには、Outlook クライアントが使用する接続をご検討ください。Outlook 2007 および Outlook 2010 は、空き時間および不在 (OOF) の情報にアクセスするのに EWS を使用します。Mac Outlook 2011 では、すべてのクライアント アクセス機能で EWS を使用します。ユーザーのメールボックスにアクティブに接続している Outlook クライアントの数によっては、ユーザーが利用できる同時接続の数が制限される可能性があります。また、アプリケーションが 1 つのセキュリティ コンテキストを使用しているときに同時に複数のメールボックスに接続する必要がある場合、**EWSMaxConcurrency** ポリシーの値を考慮することが重要です。同時接続で 1 つのセキュリティ コンテキストを使用する方法の詳細については、この記事で前述した「[EWS の偽装を使用するアプリケーションの調整の考慮事項](#throttling-considerations-for-applications-that-use-ews-impersonation)」をご覧ください。

同時に複数のメールボックスに接続するアプリケーションは、クライアント側でリソースの使用状況を追跡できる必要があります。EWS の操作は要求/応答ベースのため、要求の開始から応答の受信までの間に発生する接続数を追跡し、同時に発生する開かれた要求を 10 以内に収めれば、アプリケーションを **EWSMaxConcurrency** のしきい値内で適切に動作させることができます。

**EWSFindCountLimit** ポリシー パラメーターは、**FindItem** または **FindFolder** の操作がクライアント アクセス サーバー上で 1 人のユーザーに対して同時に使用できる結果の最大サイズを指定します。 1 つのアプリケーション (複数のアプリケーションの可能性もあります) が特定のユーザーのためにそれぞれ 100 項目を返す 2 つの同時 EWS **FindItem** 要求を行う場合、その特定のユーザーの予算に対する **EWSFindCountLimit** の使用分は 200 になります。 最初の要求を返すときに予算は 100 まで下がり、2 番目の要求を返すときに予算はゼロまで下がります。 同じアプリケーションが 1000 項目の 2 つの同時要求を行う場合、予算の値は 2000 項目になり、**EWSFindCountLimit** の値を超えます。 項目に対するユーザーの予算がゼロを下回る場合、ユーザーの予算が 1 以上に回復するまで、次の要求がエラーになります。

## <a name="throttling-considerations-for-ews-notification-applications"></a>EWS 通知アプリケーションに関する調整の考慮事項

プッシュ、プル、またはストリーミング通知を利用する EWS 通知アプリケーションを作成する場合、**EWSMaxSubscriptions** および **EWSMaxConcurrency** 調整ポリシーと **HangingConnectionLimit** の影響をご考慮ください。

**EWSMaxSubscriptions** ポリシー パラメーターは、ユーザーが特定のクライアント アクセス サーバーに対して同時に保持できるアクティブなプッシュ、プル、ストリーミング サブスクリプションの最大数を指定します。 このパラメーターの既定値は Exchange のバージョンごとに異なります。 ユーザーは **SubscribeToAllFolders** プロパティを使用して、メールボックス内のすべてのフォルダーをサブスクライブできます。これは **EWSMaxSubscriptions** の予算に対して 1 つのサブスクリプションを使用します。 ユーザーは個別のフォルダーをサブスクライブできます。各フォルダーのサブスクリプションが **EWSMaxSubscriptions** の予算に対してカウントされていき、最大で **EWSMaxSubscriptions** パラメーターの値で設定された制限にまで至ります (たとえば、**EWSMaxSubscriptions** が 20 に設定されている場合、ユーザーは様々なメールボックスの 20 の予定表フォルダーをサブスクライブできます)。

偽装と **EWSMaxSubscriptions** パラメーターの詳細については、この記事で前述した「[EWS の偽装を使用するアプリケーションの調整の考慮事項](#throttling-considerations-for-applications-that-use-ews-impersonation)」をご覧ください。

**EWSMaxConcurrency** ポリシー パラメーターが EWS 通知で問題になる可能性があります。例を挙げます。

- EWS がサブスクリプションの所有者の接続数を増分させる一方で、プッシュ サブスクリプションによって通知が生成される場合。

- アプリケーションが複数のユーザーのメールボックスをリッスンするように設計されており、配布リストに送信されたメッセージのインスタンスに関する同時の通知をユーザーたちが受信する場合。

通知アプリケーションがマルチスレッドで、同時に接続要求を行って、ユーザーアカウントによって受信された特定のメッセージに関する詳細情報を取得する場合は、 **Ewsmaxconcurrency**ポリシーの制限を超えることができます。 これに対処するには、サーバーが使用するものも含めて同時接続をアプリケーションで監視し、クライアントに要求のキューを実装することをご検討ください。

**HangingConnectionLimit** は、ストリーミング通知にのみ適用されます。この制限は web.config ファイルで設定されます。つまり、オンプレミスの Exchange サーバーで Exchange 管理者はこの値を設定できますが、Exchange Online のメールボックスはこの制限の既定値を使用する必要があります (Exchange Online と Exchange 2013 のどちらも既定値は 3 です)。詳細については、「[考慮に入れる必要がある調整の値](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)」をご覧ください。

## <a name="throttling-policy-and-application-performance"></a>調整ポリシーとアプリケーションのパフォーマンス

**PercentTimeIn** 調整ポリシーの次の 3 つのパラメーターは、EWS アプリケーションがクライアント アクセス サーバー上で使用できる時間数に影響します。 

- **EWSPercentTimeInAD**

- **EWSPercentTimeInCAS**

- **EWSPercentTimeInMailboxRPC**

**PercentTimeIn** ポリシー パラメーターに指定される値は、1 つの要求を行う 1 つのスレッドに割り当てられる時間数を示します。たとえば、**EWSPercentTimeInCAS** の値を 90 とすると、クライアント アクセス サーバー上でコードを実行するのにそれぞれ 54 秒を費やす 2 つの同時実行要求がプロセスにある場合、プロセスは 60 秒間のウィンドウで 108 秒を使用します。これは、180% の **EWSPercentTimeInCAS** パラメーターの値を表します。

> [!NOTE]
> **EWSPercentTimeInCAS** パラメーターの値は、**EWSPercentTimeInAD** および **EWSPercentTimeInMailboxRPC** パラメーターの値の重複するスーパーセットです。つまり、クライアント アクセス サーバーの処理時間における消費は、**EWSPercentTimeInAD** と **EWSPercentTimeInMailboxRPC** における消費よりも常に大きくなります。これは、Exchange コンポーネントが Active Directory または RPC を呼び出すには、クライアント アクセス サーバー コードを事前に実行しておく必要があるためです。さらに、LDAP または RPC の呼び出し中、**EWSPercentTimeInCAS** の処理時間における消費は止まりません。要求が Active Directory Domain Services (AD DS) または Exchange ストアからの応答を同期して待機している場合も、プロセスはサーバー上のスレッドを消費し続けるため、スレッドはその使用分が引き続き計上されます。

アプリケーションが60秒以内に実行される CPU 時間の量は、これらの調整制限を超える可能性があります。そのため、要求の量と種類を考慮することが重要です。 たとえば、同時に実行される**ResolveNames**操作の大きなバッチは、 **EWSPercentTimeInAD** policy パラメーターの値を超える場合があります。 既定の調整ポリシーに含まれているポリシー値は、ほとんどの EWS アプリケーションが問題なく機能するように設計されています。ただし、マルチスレッドの高ボリュームアプリケーションでは、1つの特定のクライアントアクセスサーバーに大量の要求が配置されると、問題が発生する可能性があります。 これを回避するには、サーバーに対して実行するバッチのサイズを制限することを検討してください。

## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>調整ポリシーと、大量の電子メールを送信するアプリケーション

既定の調整ポリシーには、EWS を使用して大量のメッセージを送信したり、短期間で大量のメッセージを送信したりするアプリケーションに影響を与える可能性がある、3 つのレート制限ポリシー パラメーターがあります。

> [!NOTE]
> 一般に、一括メールの送信には、EWS を使用しないことをお勧めします。頻繁に大量のメール メッセージを送信するには、一括メール サービスに特化した SMTP ホストを使用します。

**MessageRateLimit** ポリシー パラメーターは、EWS を含む Exchange クライアントで送信可能な 1 分あたりのメッセージ数を指定します。既定では、このポリシーが 1 分あたり 30 のメッセージに設定されています。一般的なユーザーは、通常はこれで十分です。ただし、大量のメール メッセージを送信するアプリケーション (請求のプログラムの一部を成すものなど) では、問題が発生する可能性があります。このポリシーの制限を超えた場合、メールボックスのメッセージ配信が遅延します。具体的には、ユーザーまたはアプリケーションが送信するメッセージの数が **MessageRateLimit** パラメーターに指定された値を超えると、メッセージが [送信トレイ] や [下書き] フォルダーに表示される時間が延びます。配信追跡システムを開発する場合 (特に、ユーザーが Outlook を使用して接続するメールボックスをアプリケーションが使用する場合) には、この点を必ずご考慮ください。遅延した項目が [送信トレイ] や [下書き] フォルダーに格納されると、ユーザーがこれをエラーとして解釈する可能性があります。

**RecipientRateLimit** ポリシー パラメーターは、24 時間中にユーザーが宛先として指定できる受信者数の制限を指定します。たとえば、この値が 500 に設定されていると、1 つの Exchange メールボックス アカウントがメッセージを送信できる受信者の数は毎日 500 以内になります。この制限は、組織内と組織外の受信者宛てのメッセージに適用されます。基幹業務アプリケーションで月の最後に請求処理を行い、この既定の制限を超える数の受信者にメッセージを送信する必要がある場合、問題が発生する可能性があります。この制限を回避するには、メッセージのバッチ処理が可能な外部サービスか、別個のオンプレミスの送信中継ソリューションを使用できます。


            **ForwardeeLimit** ポリシー パラメーターは、受信トレイ ルールを使用して、メッセージが転送またはリダイレクトできる受信者の最大数を指定します。このパラメーターは、受信者に転送またはリダイレクト可能なメッセージの数は制限しません。

## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>調整の制限を超過したときに生成されるエラー

調整ポリシーを超過すると、EWS は次の表に記載するエラーのいずれかを生成します。

**表 3. 調整制限のエラー**

|**エラー**|**調整ポリシー パラメーター**|**説明**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |サーバーに対する同時要求が、ユーザーのポリシーで許可されているものより多いことを示します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |ユーザーの調整ポリシーのサブスクリプションの最大数を超過したことを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |検索操作の呼び出しが、返すことのできる項目の合計数を超えたことを示します。  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |サーバーがビジー状態のときに発生します。ErrorServerBusy エラーと共に返される BackOffMilliseconds 値は、このエラー コードを返した応答の原因となった要求を再送信するまでに待機すべき時間数をクライアントに対して示します。  <br/> |

次の表は、調整エラーによって返される HTTP ステータス コードを示します。

**表 4. 調整エラーによって返される HTTP ステータス コード**

|**HTTP ステータス コード**|**説明**|
|:-----|:-----|
|HTTP 503  <br/> |EWS 要求が IIS でキューイングしていることを示します。クライアントは、追加の要求の送信をしばらく遅らせる必要があります。  <br/> |
|HTTP 500  <br/> |内部サーバー エラーと ErrorServerBusy エラー コードを示します。これは、クライアントが追加の要求の送信をしばらく遅延させる必要があることを示します。応答には、BackOffMilliseconds と呼ばれるバックオフのヒントが含まれる可能性があります。これが存在する場合は、クライアントが要求を再送信するまでの期間として BackOffMilliseconds の値を使用する必要があります。  <br/> |
|HTTP 200  <br/> |EWS スキーマ ベースのエラー応答と ErrorInternalServerError のエラー コードが含まれています。内部の ErrorServerBusy エラー コードが存在する可能性があります。これは、クライアントが追加の要求の送信をしばらく遅延させる必要があることを示します。  <br/> |

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
