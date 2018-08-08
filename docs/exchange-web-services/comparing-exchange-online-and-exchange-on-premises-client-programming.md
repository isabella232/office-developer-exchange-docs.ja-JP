---
title: Exchange Online と Exchange オンプレミス クライアントでのプログラミングの比較
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Exchange Online および Exchange オンプレミスに対して動作する EWS マネージ API または EWS クライアント アプリケーションを作成するための設計に関する考慮事項について説明します。
ms.openlocfilehash: 87c6ee476e06b50c339901bf61020b0fc98f8486
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758905"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Exchange Online と Exchange オンプレミス クライアントでのプログラミングの比較

Exchange Online および Exchange オンプレミスに対して動作する EWS マネージ API または EWS クライアント アプリケーションを作成するための設計に関する考慮事項について説明します。
  
ほとんどの場合、対象とするクライアントおよび Exchange の Web サービスは、対象が Exchange Online、Office 365 の一部としての Exchange Online、または Exchange オンプレミス サーバーかどうかに関係なく、同様に動作します。 ただし、いくつかの例外があり、アプリケーションがそれらの例外を処理できることを確認する必要があります。 この記事の情報は、Exchange Online および Exchange オンプレミスの両方を対象とするクライアントを設計する際に役立ちます。

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>自動検出クライアント プログラミングに関する考慮事項

[自動検出](autodiscover-for-exchange.md)は、Exchange クライアントの構成情報を提供します。 クライアント アプリケーションは、クライアントが Exchange Online と Exchange オンプレミスのどちらを対象にしているかに応じて、次の 3 つの方法のいずれかで構成情報を検出できます。 
  
**表 1. 自動検出サービスの種類と Exchange の適用性**

|**自動検出サービスの種類**|**適用対象**|
|:-----|:-----|
|[SOAP 自動検出](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online および Exchange 2010 以降のバージョンの Exchange オンプレミス  <br/> |
|[POX 自動検出](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online および Exchange 2007 以降のバージョンの Exchange オンプレミス  <br/> |
|[サービス接続ポイント (SCP) の検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Exchange 2007 以降のバージョンの Exchange オンプレミス  <br/> |
   
クライアント構成情報だけでなく、SOAP および POX の自動検出は Exchange サービス バージョンも返し、そのサービスが Exchange Online によってホストされているかどうかを示します。使用している自動検出の種類に応じて、この情報はさまざまな要素で返されます。
  
**表 2. サービス バージョンを返す自動検出の要素と Exchange Online ホスティング情報**

|**自動検出サービスの種類**|**サービス バージョンを格納する XML 要素**|**ユーザーが Exchange Online アカウントを持っているかどうかを示す XML 要素**|
|:-----|:-----|:-----|
|SOAP 自動検出  <br/> |**CasVersion** テキスト値を持つ [設定 (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) 要素  <br/> |**UserMSOnline** テキスト値を持つ [設定 (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) 要素  <br/> |
|POX 自動検出  <br/> |[ServerVersion (POX)](http://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
クライアントがこの情報を確実に取り込むようにして、Exchange サーバーで利用可能な[機能セット](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)を対象にできるようにします。 これは、ユーザーのメールボックスが Exchange Online にあるか、または Exchange オンプレミス組織にあるかに基づいた別々の動作をクライアントが予期することができるかどうかを判別するのに役立ちます。 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Exchange Online を対象とするアプリケーションのテストおよびログ ファイル

Exchange Online は、EWS のプロトコル ログ ファイル、EWS のパフォーマンス カウンターへのアクセス、およびオンプレミスの Exchange サーバーで利用可能な EWS 関連サービス イベントへのアクセスを提供しません。 ただし、これらへのアクセスは、アプリケーションが EWS と対話するときにどのように実行されるかを判別するのに役立ちます。 テスト用の Exchange オンプレミス サーバーに対してアプリケーションを必ずテストして、そのパフォーマンスを最適化できるようにします。 可能であれば、Exchange Online の調整設定に一致するように、テスト サーバーで[調整設定を変更する](http://technet.microsoft.com/ja-JP/library/bb232205%28v=exchg.150%29.aspx#Policies)ことができます。これにより、Exchange Online に接続したときのアプリケーションの動作を検証できます。 
  
> [!TIP]
> [EWSRelentless](https://ewsrelentless.codeplex.com/) ツールを使用して、EWS の負荷テストを実行できます。 テスト サーバー、EWS プロトコル ログ、EWS パフォーマンス カウンター、サービス イベント、および EWS 調整設定でこのツールを使用すると、負荷がある状態で EWS がどのように動作するかについて理解を深めることができます。 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>調整設定と Exchange Online

Exchange Online での [EWS 調整設定](ews-throttling-in-exchange.md)の既定値は、Exchange オンプレミスでの既定値とは異なります。 また、Exchange Online の調整設定は変更できません。 Exchange 管理シェル コマンドレットを使用すると、Exchange オンプレミスの調整設定を検出できます。ただし、これらのコマンドレットは、Exchange Online では有効ではありません。 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Exchange 管理シェルのコマンドレットと構成設定

コマンドレットの多くは、Exchange Online および Exchange オンプレミスの Web サービス API に直接または間接的に影響を与える可能性があります。コマンドレットは、Exchange Online で以下には利用できません。
  
- 調整設定 
    
- 仮想ディレクトリ設定 
    
- 認証設定
    
Exchange Online で利用可能なコマンドレットの詳細については、「[Exchange Online の PowerShell コマンドレット](http://help.outlook.com/ja-JP/140/dd575549.aspx)」を参照してください。 Exchange オンプレミスで使用可能なコマンドレットの詳細については、「[Exchange 2013 コマンドレット](http://technet.microsoft.com/ja-JP/library/bb124413%28v=exchg.150%29.aspx)」を参照してください。
  
## <a name="client-affinity-and-network-load-balancers"></a>クライアント アフィニティとネットワーク負荷分散装置
<a name="affinity"> </a>

ほとんどの EWS 通信では、Exchange とのアフィニティを維持するためにクライアントが参加する必要はありません。 メールボックス イベントへのサブスクリプションには、クライアントが Cookie およびその他の情報を提供して、ユーザーのメールボックス イベントのキューを維持する Exchange サーバーとのアフィニティを維持する必要があります。 Exchange Server 2010 は、exchangecookie を使用して、ネットワーク負荷分散装置間でクライアント アフィニティを維持します。 Exchange Online および Exchange 2013 以降のバージョンの Exchange オンプレミスは、[X-AnchorMailbox ヘッダー、X-PreferServerAffinity ヘッダー、および X-BackEndOverrideCookie Cookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) を使用して、メールボックスの通知のアフィニティを維持します。 
  
## <a name="authentication"></a>認証
<a name="auth"> </a>

クライアントは、基本認証または OAuth を使用して、Exchange Online で認証を行うことができます。 Exchange 2013 以降のバージョンの Exchange オンプレミスは、既定では NTLM を使用します。ただし、基本認証を使用するように Exchange オンプレミスを構成することもできます。 
  
## <a name="client-latency-diagnostics"></a>クライアントの待機時間診断
<a name="diag"> </a>

Exchange Online は、クライアントの待機時間診断の報告があった場合に、それらの診断を収集します。 これは、Microsoft が Exchange Online での接続の問題のトラブルシューティングをサポートするのに役立ちます。 Exchange オンプレミスは、クライアントの待機時間診断は収集しません。 クライアントが Exchange オンプレミスを対象とする場合は、クライアントはサーバーに待機時間診断を報告することはできません。
  
## <a name="functionality-in-the-ews-managed-api"></a>EWS マネージ API の機能
<a name="ewsma"> </a>

EWS マネージ API は、サービス ポイント接続検索などの Exchange オンプレミスに特有のいくつかの機能や、クライアントの待機時間レポートなどの Exchange Online に特有のいくつかの機能を公開します。 いくつかの機能は、EWS マネージ API で実装される前に Exchange Online で実装される可能性があることに注意してください。 
  
次の EWS マネージ API 機能は、Exchange Online にのみ適用できます。
  
- クライアントの待機時間レポート
    
- 基本事前認証
    
- 応答で RequestId が返されることを要求する機能
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Exchange Online プランと Exchange サーバー エディションの API 機能
<a name="exo"> </a>

Office 365 および Exchange Online の各種プランや Exchange サーバーの標準バージョンおよびエンタープライズ バージョンで、それぞれに異なる機能セットを利用できることが考えられます。 Exchange Online のプラン、またはユーザーのメールボックスをホストする Exchange サーバー エディションによっては、いくつかの API 機能は、お使いのクライアント アプリケーションで利用できない場合がありますのでご注意ください。 
  
**表 3. プランおよびエディションによる API 機能のバリエーション**

|**API 機能**|**プランまたはエディションに関する考慮事項**|
|:-----|:-----|
|Exchange の偽装によるアクセスを除く、アカウントへの EWS アクセス  <br/> |[ビジネス向け Office 365—キオスク プラン](http://office.microsoft.com/ja-JP/business/compare-office-365-kiosk-plans-FX103178917.aspx)では許可されていません。  <br/> |
|ユニファイド メッセージング (UM)  <br/> |Office 365 エンタープライズ (E3) プラン、Exchange Online プラン 2、および Exchange Server 2013 エンタープライズ エディションでのみ利用できます。  <br/> |
|Active Directory Domain Services (AD DS) の統合  <br/> |Office 365 Small Business および Office 365 Small Business Premium プランでは利用できません。  <br/> |
|Information Rights Management、アーカイブ、および訴訟ホールド  <br/> |Office 365 エンタープライズ (E3 および E4) プランでのみ利用できます。  <br/> |
|データ損失防止  <br/> |Office 365 エンタープライズ プラン、Exchange Online プラン 2、および Exchange Server 2013 エンタープライズ エディションでのみ利用できます。  <br/> |
   
機能の可用性は変わる可能性があるため、Exchange Online プランと Exchange サーバー エディションを確認して、機能の可用性がクライアントに及ぼす影響を検証することをお勧めします。 [GetServiceConfiguration 操作](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)を使用して、または機能を実装する操作のためのテスト要求を送信することによって、機能の可用性を確認するようにクライアントを設計することもできます。 その機能が利用できない場合、サーバーからの応答でそのように示されます。 
  
## <a name="other-considerations"></a>その他の考慮事項
<a name="other"> </a>

Exchange Online ではなく、Exchange オンプレミスを対象としている場合は、次を行うことができます。
  
- Exchange サーバーにインストールされているクライアントを作成します。 
    
- EWS およびその他のクライアントで作成および送信したメッセージの配信と内容に影響を与えることのできる[カスタム トランスポート エージェント](../transport-agents/transport-agents-in-exchange-2013.md)をインストールします。 
    
## <a name="see-also"></a>関連項目

- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
- [Exchange Online と Exchange Server 2013 の比較](http://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [ビジネス プラン向けのすべての Office 365 を比較する](http://office.microsoft.com/ja-JP/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - EWS 負荷生成ツール](https://ewsrelentless.codeplex.com/)
- [Exchange および EWS Managed API の Web サービス API 機能の可用性](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Exchange での EWS 調整](ews-throttling-in-exchange.md)
    

