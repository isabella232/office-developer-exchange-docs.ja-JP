---
title: Exchange での EWS 調整
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。
ms.openlocfilehash: e7966f67753b3998235e000a022e41c90fa227b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758945"
---
# <a name="ews-throttling-in-exchange"></a>Exchange での EWS 調整

Exchange を使用しているときに EWS に影響を与える調整ポリシーについて説明します。
  
**によって提供される:** 拡張されます。マイケル ・ Mainer、米国 Microsoft Corporation 
  
この記事は、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2010 以降のオンプレミス バージョンの Exchange の EWS の調整に関する情報を提供します。Exchange の調整は、1 人のユーザーまたは 1 つのアプリケーションが使用できるサーバー リソースの量を制限して、サーバーの信頼性と稼働時間を確保するのに役立ちます。調整は、サービスの信頼性と機能に影響を与える可能性があるシステム リソースの過剰使用への事後対応です。Exchange は常に、メールボックス データベースなどの重要なインフラストラクチャ リソースの稼働状態を監視します。これらのリソースのパフォーマンスを低下させる高負荷の要因が検出された場合、EWS の接続は、各呼び出し元がこの高負荷状態に関与する量に比例して調整されます。結果として、あるユーザーが調整制限内に収まっていても、リソースの稼働状態が運用レベルに戻るまで、パフォーマンス低下が発生する可能性があります。
  
EWS を含む、Exchange のクライアント アクセス プロトコルには、それぞれ調整ポリシーがあります。EWS を使用するアプリケーションを設計するときに、アプリケーションの信頼性と Exchange サーバーの正常性を確保できるように、調整ポリシーについて考慮することは重要です。この記事では、Exchange Online と Exchange Server 2010 以降のバージョンの Exchange On-Premises のどちらを対象としているかを問わず、EWS の様々な調整ポリシーやサービスの制限を示します。必要に応じて、この記事では様々なバージョンごとの Exchange の調整ポリシーの違いも示します。
  
> [!IMPORTANT]
> 既定の調整ポリシー、調整ポリシーへのアクセス、調整ポリシーの構成は、Exchange Online と Exchange On-Premises で異なります。特定の調整設定の値は、Exchange の特定のバージョンにのみ該当します。設定値はバージョン間で異なり、オンプレミスの展開では Exchange の管理者が既定の調整ポリシーを変更できるため、この記事では既定の設定値を示しません。より重要なのは、調整の制限内で機能し、調整のシナリオに合わせて適切に対応するアプリケーションを設計するための考慮事項に注意することです。 
  
アプリケーション開発者は、調整をアプリケーションの設計に組み込む必要があります。EWS の調整パラメーターの既定値は Exchange のバージョンごとに異なります。さまざまなバージョンの Exchange にアクセスするよう設計されたクライアントとサービス アプリケーションでは、それらの設定を考慮に入れる必要があります。これは、既定値、Exchange の管理者が設定したカスタム値、あるいは (Exchange Online の場合なら) 既定で設定されて検出できない値のいずれであっても当てはまります。調整パラメーターの値はプログラムで検出できないため、起こり得るさまざまな調整の制限にアプリケーションが適合できるよう、計画をクライアントの設計仕様に組み込む必要があります。多数のメールボックスにアクセスするマルチスレッド アプリケーションを設計するとき、または多数のクライアントが同じメールボックスにアクセスするときは、既定のポリシーによって Exchange に適用される同時実行の制限をご検討ください。  
  
## <a name="throttling-policies-that-affect-ews"></a>EWS に影響を与える調整ポリシー
<a name="bk_PolicyParameters"> </a>

Exchange の調整ポリシーは、EWS だけでなく、Office Outlook、Outlook Web App、Exchange ActiveSync によって使用されるプロトコルを含む、Exchange サーバーへのすべてのクライアント接続にも影響します。  
  
ポリシーを調整する**CPUStartPercent**は、Exchange 2010 を実行している場合、EWS のパフォーマンスを影響します。 Exchange の平均 CPU 使用率がクライアント アクセス サーバー上で実行を処理する場合-に限らず、EWS のプロセスを含む-このポリシーによって指定された値を超える場合、CPU 使用率を減らすために受信要求は遅れます。 このポリシーの値を変更することはできませんが、パフォーマンスの問題のトラブルシューティングに役立ちますのです。 サンプリング ロジックをクライアント アクセス サーバーがこの値に対して実行は、10 秒間のローリング ウィンドウ上での平均です。 これにより、CPU 使用率のスパイクを迅速に適切に応答するプロセスです。 このしきい値を超えた場合、EWS への着信接続が遅延します。 EWS 要求ごとには、理論上 100 %cpu 使用率で、500 ミリ秒 (ミリ秒) にこの遅延が上限です。 100 項目を取得するバッチ EWS 要求が渡されると、サーバーは CPU 使用率が 100 回 (1 回あたりの項目) を確認 50 秒の最大遅延時間です。 遅延時間は、CPU 使用率には直線的に比例します。 **CPUStartPercent**遅延は 0 (スレッドの yield) と、500 まで直線的に増加 CPU 使用率が 100% にミリ秒を超えています。 スロットルのポリシーは、すべての Exchange ユーザーに適用するためには可能性のある CPU 使用率は、 **CPUStartPercent**に対する制限を超えた Exchange クライアント アクセス サーバーでは、個々 のユーザーやアプリケーションに影響を与えるための十分な CPU の使用率を取得できないためサーバー操作です。 
  
次の表は、EWS を使用するアプリケーションに影響を与える調整ポリシー パラメーターをまとめています。
  
**表 1: EWS に影響を与えるポリシーのパラメーターを調整します。**

|**スロットルのポリシー パラメーターの名前**|**適用されます。**|**説明**|
|:-----|:-----|:-----|
|**DiscoveryMaxConcurrency** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが同時に接続できる同時探索検索の数を指定します。   <br/> |
|**DiscoveryMaxKeywords** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが探索検索に含めることができるキーワードの最大数を指定します。   <br/> |
|**DiscoveryMaxKeywordsPerPage** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |統計情報を表示するキーワードの数を指定します。   <br/> |
|**DiscoveryMaxMailboxes** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが探索検索に含めることができるソース メールボックスの最大数を指定します。   <br/> |
|**DiscoveryMaxMailboxesResultsOnly** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |インプレース電子情報開示検索において検索可能 (統計情報の表示は不可) なメールボックスの最大数を指定します。   <br/> |
|**DiscoveryPreviewSearchResultsPageSize** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |電子情報開示検索のプレビューの応答で返されるメッセージの数を指定します。   <br/> |
|**EwsCutoffBalance** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |EWS ユーザーのリソース消費制限を定義し、これを超えたら特定のコンポーネントの操作を実行できないよう、ユーザーを完全にブロックするようにします。   <br/> |
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |増加したリソースを EWS ユーザーが消費できる時間の長さを定義し、これを超えたら調整を行うようにします。これは、ミリ秒単位で測定されます。この値は、コンポーネントごとに個別に設定されます。   <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |予算時間中に EWS ユーザーの予算を回復する速度 (予算の増加単位) を定義します。   <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |ユーザーが特定のクライアント アクセス サーバーに対して同時に保持できるアクティブなプッシュ、プル、ストリーミング通知のサブスクリプションの最大数を定義します。この予算は Exchange のバージョンごとに異なります。   <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |EWS で Exchange の検索を使用して、高速な検索が続行前に秒単位でタイムアウトの時間を定義します。[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)で高度なクエリ構文 (AQS) のクエリ文字列を使用して検索を高速な検索には。  <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |一度に 1 人のユーザーのクライアント アクセス サーバー上のメモリ内の[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)またはことができます[FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)の項目の最大数を定義します。 このプロパティの既定値は 1000 です。 [フォールバック値](http://technet.microsoft.com/en-us/library/dd297964%28v=exchg.141%29.aspx#fallback)この値は 1000 です。  <br/> Exchange オンラインと設置型のバージョンの Exchange が Exchange 2013 で始まるが、このスロットルのポリシーを照会やコマンドレットによって構成されていることはできません。 Exchange Online および設置型バージョンの Exchange が Exchange 2013、 [AQS の検索](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)のための EWSFindCountLimit、任意の交換を開始、制限付きの検索は 250 の結果です。 最高 1000 の結果を制限せず、Exchange 検索に戻ります。  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |特定のユーザーが Active Directory の要求を実行できる時間が 1 分間のうちに占める割合を定義します。   <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |特定のユーザーがクライアント アクセス サーバーのコードを実行できる時間が 1 分間のうちに占める割合を定義します。   <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |特定のユーザーがメールボックス RPC の要求を実行できる時間が 1 分間のうちに占める割合を定義します。  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |EWS を使用している Exchange サーバーに対して特定のユーザーが同時に並列で開くことができる接続の数を定義します。Exchange 2010 の既定値は 10 です。Exchange 2013 および Exchange Online の既定値は 27 です。 <br/> 通知のストリーミング以外のすべての操作に、このポリシーが適用されます。 ストリーミングの通知では、開いているストリーミング イベント利用可能な接続の数を示すために**HangingConnectionLimit**を使用します。 詳細についてを参照してください[考慮に入れるにはスロットル値が必要ですか?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)です。  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |送信可能な 1 分あたりのメッセージ数を定義します。   <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中にユーザーが宛先として指定できる受信者数の制限を定義します。   <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |24 時間中に受信トレイの転送またはリダイレクト操作の対象にできる受信者数の制限を定義します。   <br/> |
   
> [!CAUTION]
> 設定しない**null**にポリシーを調整します。 これにより、スロットルのポリシーが設定されていないことを示す数を無制限に、ポリシーが設定されます。 
  
## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Exchange のメールボックスに適用するポリシーを表示する
<a name="bk_PolicyCmdlets"> </a>

Exchange On-Premises には、調整ポリシーを設定および取得するために使用できる Exchange 管理シェル コマンドレットが用意されています。Exchange Online は、調整ポリシーのコマンドレットを利用できません。
  
次のコマンドレットを使用して、オンプレミスの Exchange Server の展開の調整ポリシーを表示できます。
  
- **Get ThrottlingPolicy** -調整の設定を 1 つまたは複数のクライアント調整ポリシーを取得します。 詳細については、TechNet の[Get ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351264.aspx)を参照してください。 
    
- **Get ThrottlingPolicyAssociation** -オブジェクトとの関連付けられた調整ポリシーとの間の関係を表示できます。 オブジェクトには、メールボックスを持つユーザー、メールボックス、または取引先担当者にユーザーができます。 詳細については、TechNet の「 [Get ThrottlingPolicyAssociation](http://technet.microsoft.com/en-us/library/ff459241.aspx)を参照してください。 
    
Exchange 2010 の既定の調整ポリシーを表示するには、次のコマンドを使用します。
  
**Get ThrottlingPolicy |Where-object {$_ です。IsDefault - eq"True"} |形式リスト**
  
Exchange 2013 のグローバル調整ポリシー (Exchange 2010 の既定の調整ポリシーに等しい) を表示するには、次のコマンドを使用します。
  
**Get ThrottlingPolicy |Where-object {$_ です。ThrottlingPolicyScope - eq「グローバル」} |形式リスト**
  
Exchange 2010 または Exchange 2013 のユーザーに関連付けられた調整ポリシーを表示するには、次のコマンドを使用します。ユーザー名 john@contoso.com を、調整ポリシー情報を取得する対象ユーザーのユーザー名で置き換えます。
  
**Get ThrottlingPolicyAssociation john@contoso.com |形式リスト**
  
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
> **ThrottlingPolicyId**プロパティが空の場合は、既定のポリシーがメールボックスに適用されます。 
  
[セット ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd298094.aspx)と[セット ThrottlingPolicyAssociation](http://technet.microsoft.com/en-us/library/ff459231.aspx)コマンドレットを使用して Exchange サーバー上のポリシーを調整を設定することができます。 作成し、削除以外の[新規 ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351045.aspx)と[削除 ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351178.aspx)コマンドレットを使用してポリシーを調整できます。 
  
> [!TIP]
> 既定の調整ポリシーに従うようにアプリケーションを設計することをお勧めします。クライアント アプリケーションの設計が既定のポリシーに対応できない場合にのみ、既定の調整ポリシーに変更を加えてください。制限の少ない調整ポリシーは、サービスの信頼性に悪影響を及ぼす可能性があることにご注意ください。 
  
## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>EWS の偽装を使用するアプリケーションの調整の考慮事項
<a name="bk_ThrottlingConsiderations"> </a>

[偽装](impersonation-and-ews-in-exchange.md)は、多数のアカウントにアクセスする 1 つのアカウントを有効にする認証方法です。 サービス アカウントは、ユーザーを偽装するときにユーザーとして動作し、したがってそれらのユーザーに割り当てられている権限を想定しています。 ログ ファイルでは、偽装されたユーザーとしてのアクセスを記録します。 管理者は、Exchange 管理シェルを使用して偽装を構成するのには、役割ベースのアクセス制御 (RBAC) を使用します。 
  
偽装を使用すると、調整のしきい値すべての予算は Exchange のバージョンごとに異なって適用されます。予算の計算は、偽装される側のアカウントか、サービス アカウントのいずれかに対して行われます。アプリケーションがマルチスレッド化され、複数のメールボックスに対して同時要求を行う場合は、調整のしきい値がアプリケーションのパフォーマンスに与える影響をご考慮ください。一般に、偽装ですべてのメールボックスにアクセスするサービス ベースのアプリケーションを作成するときには、サービス アカウントの次の制限にご注意ください。  
  
- 偽装を使用する場合、サービス アカウントは、次のポリシー パラメーターに関して別個の予算を持ちます。
    
  - **EWSMaxConcurrency**
    
  - **EWSPercentTimeInAD**
    
  - **EWSPercentTimeInCAS**
    
  - **EWSPercentTimeInMailboxRPC**
    
  - **EWSMaxSubscriptions**
    
  - **EWSFastSearchTimeoutInSeconds**
    
  - **EWSFindCountLimit**
    
- **EWSMaxConcurrency**予算は、サービス アカウントと、Exchange 2010 Service Pack 2 (SP2) の更新プログラムのロールアップ 4 (RU4) より前のバージョンの Exchange への接続すべてに偽装されているアカウントに共有されています。 Exchange 2010 SP2 の RU4 を開始して、Exchange Online を含め、サービス アカウントのアクセスは、ユーザー **EWSMaxConcurrency**の予算からの個別の予算を使用します。 EWS の同時接続のスロットルのポリシーの [Exchange の更新の詳細については、[説明の更新プログラムのロールアップ 4 については、Exchange Server 2010 のサービス パック 2](http://support.microsoft.com/kb/2706690)を参照してください。
    
    EWS のバージョンの Exchange が Exchange 2010 で始まると、Exchange Online を含む通知をストリーミングでは、他のすべての EWS クライアント接続からその他のクローン ・ **EWSMaxConcurrency**予算があります。 ストリーミングの通知の接続は、他のすべての EWS の操作よりも個別の予算に対してカウントされます。 ストリーミングの通知の最大同時実行予算は、実際には 2 つの異なる予算: すべてのサービス アカウントは、1 つの予算と予算は 1 つが偽装されているアカウントには。 通知を Exchange ストリーミング オンラインとのバージョンの Exchange が Exchange 2013 で始まるを使用して、 [HangingConnectionLimit](ews-throttling-in-exchange.md#bk_ThrottlingNotifications)の接続数を制限します。 
    
    たとえば、 **EWSMaxConcurrency**が 5 に等しいと仮定します。 ユーザーは、サービス アカウントは 5 つ同時プル通知に接続できるユーザーのメールボックスに対して、ユーザーと同時に 5 つの開いているプル通知の接続を持つことができます。 
    
- 次の表は、サービス アカウントと、アカウントを偽装する**EWSMaxSubscriptions**スロットルの予算を計算する方法を識別します。 
    
   **表 2: EWSMaxSubscriptions 予算会計**

   |**Exchange のバージョン**|**EWSMaxSubscriptions の予算勘定の調整**|
   |:-----|:-----|
   |Exchange Online  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2013  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP3  <br/> |対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP2  <br/> |呼び出し元のアカウントに対して適用されます。Exchange 2010 SP2 RU4 以降では、予算は対象のメールボックスに対して適用されます。  <br/> |
   |Exchange 2010 SP1  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |
   |Exchange 2010  <br/> |呼び出し元のアカウントに対して適用されます。  <br/> |
   
- 偽装されているアカウントに対して予算を調整する**EWSMaxSubscriptions**が充電されるとため、制限はありません、サービス アカウントを購読して、ストリーミングの通知を受信のメールボックスの数に限り偽装使用されています。 偽装されているアカウントにすることはできません_n_の同時実行の要求より多くの_**EWSMaxSubscriptions**値は_、ターゲット メールボックスあたりです。 偽装を使用していないが、同じサービス アカウントこと_n_同時実行される要求の合計より多くがないです。 論点は、サービス アカウントの偽装を使用して、指数関数的に増加するサービスを提供できるメールボックスの数です。 詳細については、 [Exchange でのサブスクリプションのグループとメールボックス サーバー間のアフィニティを維持](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)を参照してください。
    
- **EWSPercentTimeInMailboxRPC**、 **EWSPercentTimeInCAS**、および**EWSPercentTimeInAD**のポリシーのパラメーターは、1 つのスレッドによって実行されるアクションを参照してください。 アプリケーションは、複数の同時操作を実行するときは、ユーザーのリソースの予算内でこれらの操作の累積的な影響を考慮する必要があります。 
    
## <a name="throttling-implications-for-ews-batch-requests"></a>EWS のバッチ要求の調整の影響
<a name="bk_ThrottlingBatch"> </a>

EWS を使用すると、クライアント アクセス サーバーで実行される 1 つの要求に複数の項目の要求をバッチ処理できます。 これにより、効率性とパフォーマンスが向上。 Exchange サーバーでは、バッチ処理される要求を実行するときは、バッチ内の各項目の実行後にユーザーの予算を確認します。 アプリケーションが予算オーバーの場合は、そのユーザーの予算は、再充電するまで、バッチ内の次のアイテムの処理が遅延します。 バッチ操作を使用するアプリケーションが正常に実行されることを確認するには、1 つのバッチに含めることができるし、結果の信頼性を高めるための複数の小さいバッチの間で大規模なバッチに分割項目要求の数を制限します。 スロットルしきい値を特定のバッチ処理の影響は、要求の種類、項目 (たとえば、 **UploadItems**または**ExportItems**の操作) で処理して、メールボックスの内容のサイズによって異なります。 スロットルのポリシーは、プロセスに時間がかかる要求を発生させることによって、バッチ操作を影響します。 呼び出し元は、しばらくの間、応答の必要したがって、呼び出しがタイムアウトで EWS が 1 つ分のバッチ要求の実行時間を制限するためです。 
  
アプリケーションのバッチの最適なサイズを決定するには、様々な入力セットを使用して単体テストを実行し、運用環境でアプリケーションにエラーが発生しないことを確認します。  
  
## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>EWS の検索操作に影響を与える調整ポリシー パラメーター
<a name="bk_ThrottlingSearch"> </a>

[EWS での検索操作](search-and-ews-in-exchange.md)では、大量の時間とリソースの検索を実行する方法と、どのような情報が必要に応じてを要求できます。 検索中にリソースの使用状況を制御するポリシーの 2 つのパラメーターが有効: **EWSFastSearchTimeoutInSeconds**と**EWSFindCountLimit**。 
  
**EWSFastSearchTimeoutInSeconds**ポリシーのパラメーターは、時間、その EWS の高速検索 (インデックス検索のコンテンツとも呼ばれます) を秒単位でタイムアウトする前に実行を指定します。[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)で高度なクエリ構文 (AQS) のクエリ文字列を使用して検索を高速検索には。
  
Exchange のメールボックス フォルダーを 2 つの方法で検索できます。
  
- Exchange ストアの検索を使用します。これにより、ターゲット検索スコープ内のすべてのメッセージの順次スキャンを実行します。
    
- Exchange Search サービス (コンテンツ インデックス) を使用します。
    
これらの種類の検索は、両方ともタイムアウトになることがあります。これらの検索はメールボックスのインデックスを対象とし、AQS クエリを使用しているため、できれば Exchange Search サービスを使用します。次の例では、EWS および Exchange Search サービスを使用して受信トレイの AQS 検索を実行する方法を示します。
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

AQS 検索を使用できない場合は、過度に複雑な検索フィルターを使用しないようにします。また、クエリに拡張 MAPI プロパティが含まれる場合は、計算された値に基づいて検索フィルターを作成しないようにもご注意ください。AQS 検索は Exchange 2010 で導入されました。
  
> [!NOTE]
> 最初に複雑な Exchange ストア検索クエリを実行するときに時間がかかる実行され、タイム ・ アウトします。その後は、クエリが迅速に対応されます。 バックエンドの Exchange の詳細については、交換の際に発生するサーバー プロセスは検索クエリを保存、TechNet の[パフォーマンスへの影響の高数と制限付きビューを理解する](http://technet.microsoft.com/en-us/library/cc535025%28EXCHG.80%29.aspx)を参照してください。 の**SearchFilter**を使用して、今後、同様のクエリを支援する動的な制限を作成がこれらの制限は本質的に動的であるため、永続的なまたは信頼性の高いではない、最大 3 日後に削除します。 
  
**EWSFindCountLimit**ポリシーのパラメーターは、クライアント アクセス サーバー上のメモリに 1 人のユーザーに同時に存在できる**FindItem**または**FindFolder**操作の結果からのアイテムの最大数を指定します。 すべての項目または EWS が**FindItem**または**FindFolder**要求で処理するフォルダーは、 **EWSFindCountLimit**要素で指定されている予算に対してカウントされます。 応答は、依頼者に返送される、現在の呼び出しの検索数の請求金額が解放されます。 サーバーに返します、依頼者の予算を超えたときの応答は、 **RequestServerVersion**要素の値と、依頼者がページングを指定するかどうかに基づいています。 **RequestServerVersion**要素の値は、Exchange 2010 または Exchange の以前のバージョンを示す、サーバーはエラー コード**ErrorServerBusy**のエラー応答を送信します。 **RequestServerVersion**要素の値は、バージョンを示す場合の Exchange と Exchange 2010 SP1 または Exchange Online では、クライアントの起動を使用してページング、EWS はエラーではなく、部分的な結果を返すことがあります。 EWS がすべての項目を返すことがありますされません、アプリケーションが予想されます。 **IncludesLastItemInRange**要素の値が false の場合、アプリケーションする必要があります新しいオフセットを持つ別の**FindItem**または**FindFolder**要求継続して**IncludesLastItemInRange**要素が true を返すまでします。 
  
**FindItem**または**FindFolder**操作を使用する場合に、ページングを使用して必要があります。 EWS のマネージ API は、ページングの使用を強制しますが、EWS プロキシ オブジェクトや、生の SOAP など、他のメソッドを使用している場合は、ページングを明示的に設定する必要があります。 次の例では、EWS のマネージ API でページングを使用する方法を示します。 
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> Exchange の既定のポリシーでは、ページ サイズを 1000 項目に制限します。この数よりも大きい値にページ サイズを設定しても、実際的な効果はありません。 
  
アプリケーションは、設定、同時実行を要求するアプリケーションに返される結果の一部のパラメーターの値を調整する_EWSFindCountLimit_がありますということを考慮する必要がありますもします。 次の例では、EWS のマネージ API のすべての結果がクエリに含まれていることを確認するのには**MoreAvailable**プロパティを使用する方法を示します。 
  
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
<a name="bk_ThrottlingConcurrency"> </a>

同時実行とは、特定のユーザーからの接続の数を指します。接続は、要求が受信された時点から応答が要求側に送信されるまで保持されます。ユーザーがポリシーの許可数を超える同時要求を試みると、新しい接続試行は失敗します。ただし、既存の接続は有効なまま維持されます。調整ポリシーは、様々な方法で同時実行に影響を与える可能性があります。
  
**EWSMaxConcurrency**スロットルのポリシー パラメーターは、特定のユーザーが Exchange サーバーに対して同時に 1 つの同時接続の数を設定します。 許可する同時接続の最大数を確認するのには、Outlook クライアントを使用する接続を検討してください。 Outlook 2007 および Outlook 2010 は、可用性および Office (OOF) の情報にアクセスするのには EWS を使用します。 Mac Outlook 2011 では、すべてのクライアント アクセス機能の EWS を使用します。 、積極的にユーザーのメールボックスに接続する Outlook クライアントの数によっては、ユーザーの同時接続の数が限られた可能性があります。 アプリケーションに 1 つのセキュリティ コンテキストを使用しているときに同時に複数のメールボックスに接続する場合は、 **EWSMaxConcurrency**ポリシーの値を考慮に入れる必要があります。 同時接続で 1 つのセキュリティ コンテキストを使用する方法の詳細については、この資料の前半の[EWS の偽装を使用するアプリケーション用のスロットルの考慮事項](http://msdn.microsoft.com/library/961f773a-8b8e-4b4f-a4b9-64305e107ca4.aspx#bk_ThrottlingConsiderations)を参照してください。 
  
同時に複数のメールボックスに接続するアプリケーションをクライアント側のリソースの使用状況を追跡する必要があります。 EWS の操作が要求/応答ベースのため行うことができます**EWSMaxConcurrency**のしきい値の範囲内でアプリケーションの動作は、要求と応答の開始の間で発生する接続の数を追跡することによって受信し、同時に発生する要求を開く 10 個を超えないことを確認します。 
  
**EWSFindCountLimit**ポリシーのパラメーターでは、 **FindItem**または**FindFolder**操作ことができますを使用してクライアント アクセス サーバーで同時に 1 人のユーザーの最大数の結果のサイズを指定します。 アプリケーション (または複数のアプリケーション可能性があります) は、100 項目の特定のユーザーを返す 2 つの同時 EWS **FindItem**要求を使用して、その特定のユーザーの予算に対して**EWSFindCountLimit**の費用が 200 になります。 100、予算を削除する最初の要求が返されるとき、予算がゼロに低下して 2 番目の要求が返されるとき。 1000 項目の 2 つの同時要求を作成する同じアプリケーションの場合、予算の値でしょう 2000 アイテム、 **EWSFindCountLimit**の値を超える。 品目に対するユーザーの予算がゼロを下回った場合、次の要求は、1 つまたは複数ユーザーの予算が充電されますまで、エラーになります。 
  
## <a name="throttling-considerations-for-ews-notification-applications"></a>EWS 通知アプリケーションに関する調整の考慮事項
<a name="bk_ThrottlingNotifications"> </a>

EWS 通知プッシュ、プル、または通知をストリーミングを使用するアプリケーションを構築する場合に、 **EWSMaxSubscriptions**と**EWSMaxConcurrency**の制限ポリシー、および、**の影響を検討してください。HangingConnectionLimit**。 
  
**EWSMaxSubscriptions**ポリシーのパラメーターは、アクティブなプッシュ、プル、およびユーザーが特定のクライアント アクセス サーバーで同時に持つことができますストリーミングのサブスクリプションの最大数を指定します。 異なるバージョンの Exchange では、このパラメーターの既定値があります。 ユーザーが**SubscribeToAllFolders**プロパティを使用してメールボックス内のすべてのフォルダーを購読できます - **EWSMaxSubscriptions**の予算に対して 1 つのサブスクリプションを使用します。 ユーザーは、個々 のフォルダーを購読できますは、各フォルダーに**EWSMaxSubscriptions**予算の上限に達するまでにサブスクリプションをカウント**EWSMaxSubscriptions**パラメーターの値 (たとえば、ユーザーが購読できる 20 の予定表フォルダー **EWSMaxSubscriptions**が 20 に設定されている場合、別のメールボックスで)。 
  
偽装と**EWSMaxSubscriptions**パラメーターについては、この資料の前半の[EWS の偽装を使用するアプリケーション用のスロットルの考慮事項](ews-throttling-in-exchange.md#bk_ThrottlingConsiderations)を参照してください。 
  
**EWSMaxConcurrency**ポリシーのパラメーターには、EWS の通知は、問題ことができます。例えば： 
  
- EWS がサブスクリプションの所有者の接続数を増分させる一方で、プッシュ サブスクリプションによって通知が生成される場合。
    
- アプリケーションが複数のユーザーのメールボックスをリッスンするように設計されており、配布リストに送信されたメッセージのインスタンスに関する同時の通知をユーザーたちが受信する場合。
    
通知アプリケーションは、マルチ スレッド、同時接続要求を特定のユーザー アカウントで受信したメッセージの詳細については、 **EWSMaxConcurrency**ポリシーの制限を超えることができます。 これを考慮するのには、アプリケーションの同時接続を監視するサーバーによって使用されるものなど、クライアント上のキューの要求を実装することを検討してください。 
  
**HangingConnectionLimit**は、通知をストリーミングするのには該当する場合のみです。 この制限は、Exchange 管理者は、オンプレミスの Exchange サーバーでこの値を設定できますが、Exchange Online のメールボックスは、オンラインの Exchange および Exchange 2013 の 3 では、この制限の既定値を使用する必要があることを意味する、web.config ファイルで設定されています。 詳細についてを参照してください[考慮に入れるにはスロットル値が必要ですか?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)です。
  
## <a name="throttling-policy-and-application-performance"></a>調整ポリシーとアプリケーションのパフォーマンス
<a name="bk_PercentTimeIn"> </a>

ポリシーを調整する**PercentTimeIn**の次の 3 つのパラメーターは、クライアント アクセス サーバーで、EWS アプリケーションを使用する時間の量に影響します。 
  
- **EWSPercentTimeInAD**
    
- **EWSPercentTimeInCAS**
    
- **EWSPercentTimeInMailboxRPC**
    
**PercentTimeIn**ポリシーのパラメーターで指定された値は、1 つの要求を行っている 1 つのスレッドが割り当てられた時間量を示します。 などのクライアント アクセス サーバーでコードを実行する各プロセスは、54 秒を費やしている 2 つの同時要求を行った場合、90 の**EWSPercentTimeInCAS**値を想定すると、プロセスを使用して、108 秒、60 秒のウィンドウです。 これは、 **EWSPercentTimeInCAS**パラメーターの値が 180% を表します。 
  
> [!NOTE]
> **EWSPercentTimeInCAS**パラメーターの値は、 **EWSPercentTimeInAD**および**EWSPercentTimeInMailboxRPC**パラメーターの値の重複のスーパー セットです。 これは、クライアント アクセス サーバーの処理時間の支出常になるは**EWSPercentTimeInAD**と**EWSPercentTimeInMailboxRPC**のコストよりも大きいことを意味します。 コンポーネントの Active Directory または RPC コールを作成するのにする必要があります既に実行されているクライアント アクセス サーバーのコードがあるためにです。 さらに、LDAP の中に**EWSPercentTimeInCAS**の処理時間の支出を停止しないか、RPC 呼び出しが行われています。 要求は、Active Directory ドメイン サービス (AD DS) または Exchange ストアからの応答を同期的に待機している可能性があります、プロセスがまだサーバー上のスレッドを消費して、スレッドは引き続きその使用法について、請求するためです。 
  
CPU 時間が 60 秒以内にアプリケーションがかかる場合があります。 がこれらの制限の範囲を制限を超える可能性があります。したがって、ボリュームおよび行われる要求の種類を考慮すべき重要なです。 たとえば、 **ResolveNames**操作が同時に行われる大規模なバッチは、 **EWSPercentTimeInAD**ポリシー パラメーターの値を超過できます。 既定の調整ポリシーに含まれているポリシーの値は問題なく動作するほとんどの EWS アプリケーションを許可するように設計されていますただし、大容量のマルチ スレッド アプリケーションでは、1 つの特定のクライアント アクセス サーバーで大量の要求を配置、ときにこれ問題が生じることができます。 これを回避するには、サーバーに対して実行されているバッチのサイズを制限することを検討します。 
  
## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>大量のメールを送信する調整ポリシーとアプリケーション
<a name="bk_RateLimits"> </a>

既定の調整ポリシーには、EWS を使用して大量のメッセージを送信したり、短期間で大量のメッセージを送信したりするアプリケーションに影響を与える可能性がある、3 つのレート制限ポリシー パラメーターがあります。  
  
> [!NOTE]
> 一般に、一括メールの送信には、EWS を使用しないことをお勧めします。頻繁に大量のメール メッセージを送信するには、一括メール サービスに特化した SMTP ホストを使用します。 
  
**MessageRateLimit**ポリシーのパラメーターでは、EWS を含む、すべての Exchange クライアントによって送信可能な 1 分あたりのメッセージ数を指定します。 既定では、1 分あたり 30 のメッセージにこのポリシーを設定します。 通常のユーザーは、だけで十分です。 ただし、請求のプログラムでは、一部として、たとえば、電子メール メッセージのサイズの大きいバッチを送信するアプリケーションは、問題を実行できます。 このポリシーの制限を超えた場合、メールボックスのメッセージ配信が遅延します。 具体的には、メッセージは、ユーザーまたはアプリケーションは、 **MessageRateLimit**パラメーターで指定した値より大きな値のメッセージを送信する時間の長い期間の [送信トレイ] や [下書き] フォルダーに表示されます。 アプリケーションが Outlook を使用して接続のユーザーのメールボックスを使用する場合に特に追跡システムの提供を開発するときは、考慮する必要があります。 遅延のアイテムは [送信トレイ] や [下書き] フォルダーに格納されているユーザーとして解釈されるエラー。 
  
**RecipientRateLimit**ポリシーのパラメーターは、ユーザーが 24 時間以内に対処できる受信者の数に制限を指定します。 たとえば、この値は 500 に設定されている場合ことを意味なし 500 以上の受信者の 1 日に 1 つの Exchange メールボックス アカウントがメッセージを送信できることです。 内および組織外の受信者へのメッセージにこの制限が適用されます。 この既定の制限値か月間の最後の請求書の実行を行うし、この受信者数を超えるメッセージを送信する必要があるいくつかの基幹業務アプリケーションの問題が発生する可能性があります。 この制限を回避するには、メッセージまたは送信中継ソリューションの個別設置型のバッチ処理を有効にする外部のサービスを使用することができます。 
  
**ForwardeeLimit**ポリシーのパラメーターは、受信者がメッセージを転送または受信トレイ ルールを使用するリダイレクトの最大数を指定します。 このパラメーターには、転送または受信者にリダイレクトできるメッセージの数を制限しません。 
  
## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>エラー
<a name="bk_ThrottlingErrors"> </a>

調整ポリシーを超過すると、EWS は次の表に記載するエラーのいずれかを生成します。
  
**表 3: 調整の制限のエラー**

|**Error**|**ポリシー パラメーターの調整**|**説明**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |サーバーに対する同時要求が、ユーザーのポリシーで許可されているものより多いことを示します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |ユーザーの調整ポリシーのサブスクリプションの最大数を超過したことを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |検索操作の呼び出しが、返すことのできる項目の合計数を超えたことを示します。  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |サーバーがビジー状態のときに発生します。ErrorServerBusy エラーと共に返される BackOffMilliseconds 値は、このエラー コードを返した応答の原因となった要求を再送信するまでに待機すべき時間数をクライアントに対して示します。  <br/> |
   
次の表は、調整エラーによって返される HTTP ステータス コードを示します。
  
**表 4: エラーを調整することによって返される HTTP ステータス ・ コード**

|**HTTP ステータス コード**|**説明**|
|:-----|:-----|
|HTTP 503  <br/> |EWS 要求が IIS でキューイングしていることを示します。クライアントは、追加の要求の送信をしばらく遅らせる必要があります。  <br/> |
|HTTP 500  <br/> |内部サーバー エラーと ErrorServerBusy エラー コードを示します。これは、クライアントが追加の要求の送信をしばらく遅延させる必要があることを示します。応答には、BackOffMilliseconds と呼ばれるバックオフのヒントが含まれる可能性があります。これが存在する場合は、クライアントが要求を再送信するまでの期間として BackOffMilliseconds の値を使用する必要があります。  <br/> |
|HTTP 200  <br/> |EWS スキーマ ベースのエラー応答と ErrorInternalServerError のエラー コードが含まれています。内部の ErrorServerBusy エラー コードが存在する可能性があります。これは、クライアントが追加の要求の送信をしばらく遅延させる必要があることを示します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange ワークロード管理](http://technet.microsoft.com/en-us/library/jj150503.aspx)
- [ThrottlingPolicy で新しいコマンドレット](http://technet.microsoft.com/en-us/library/dd351045.aspx)
- [クライアントのポリシーの制限を理解します。](http://technet.microsoft.com/en-us/library/dd297964.aspx)
- [ThrottlingPolicy クラス](http://msdn.microsoft.com/en-us/library/ff342496%28v=EXCHG.140%29.aspx)
- [スロットルのポリシーと、EWSFindCountLimit](http://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [IIS ログに予算のスナップショット](http://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)
- [Exchange 2010 sp1 では、配置の調整の効果](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Exchange 2010 sp1 では、ポリシー関連の調整](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [スロットルのポリシーと CPUStartPercent](http://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Exchange の偽装と EWS](impersonation-and-ews-in-exchange.md)
    

