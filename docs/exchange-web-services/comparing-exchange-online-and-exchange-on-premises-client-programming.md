---
title: Exchange Online と Exchange オンプレミス クライアント プログラミングの比較
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Exchange Online および Exchange オンプレミスに対して動作する EWS マネージ API または EWS クライアント アプリケーションを作成するための設計に関する考慮事項について説明します。
ms.openlocfilehash: 87c6ee476e06b50c339901bf61020b0fc98f8486
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758905"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Exchange Online と Exchange オンプレミス クライアント プログラミングの比較

Exchange Online および Exchange オンプレミスに対して動作する EWS マネージ API または EWS クライアント アプリケーションを作成するための設計に関する考慮事項について説明します。
  
大部分、クライアントおよび web を対象の Exchange のサービスが、ターゲットは、Exchange オンラインで、Office 365 の一部として Exchange のオンラインかどうかに関係なく同様に動作または Exchange の設置型サーバーです。 ある、ただし、いくつかの例外と、アプリケーションがそれらを処理できることを確認します。 両方の Exchange Online を対象とするようにクライアントをデザインするため、この資料の情報を使用し、交換設置します。

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>自動検出クライアント プログラミングの考慮事項

[自動検出](autodiscover-for-exchange.md)では、Exchange クライアントの構成情報を提供します。 クライアント アプリケーションは、クライアントが対象とするオンラインの Exchange または Exchange の設置型かどうかに応じて、次の 3 つの方法のいずれかの構成情報を検出できます。 
  
**表 1 です。自動検出サービスの種類と交換の適用範囲**

|**自動検出サービスの種類**|**適用されます。**|
|:-----|:-----|
|[SOAP の自動検出](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online および Exchange 2010 以降のバージョンの Exchange オンプレミス  <br/> |
|[POX の自動検出](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online および Exchange 2007 以降のバージョンの Exchange オンプレミス  <br/> |
|[サービス接続ポイント (SCP) の検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Exchange 2007 以降のバージョンの Exchange オンプレミス  <br/> |
   
クライアント構成情報だけでなく、SOAP および POX の自動検出は Exchange サービス バージョンも返し、そのサービスが Exchange Online によってホストされているかどうかを示します。使用している自動検出の種類に応じて、この情報はさまざまな要素で返されます。
  
**表 2 になります。サービスのバージョンとの情報をホストしている Exchange Online を返す要素を自動検出**

|**自動検出サービスの種類**|**サービスのバージョンを格納する XML 要素**|**XML 要素をユーザーが Exchange のオンライン アカウントを持っているかどうかを示す**|
|:-----|:-----|:-----|
|SOAP 自動検出  <br/> |**CasVersion**のテキスト値を持つ要素を[設定 (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)です。  <br/> |**UserMSOnline**のテキスト値を持つ要素を[設定 (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)です。  <br/> |
|POX 自動検出  <br/> |[ServerVersion (POX)](http://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Exchange サーバーで使用可能な[機能セット](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)をターゲットにできるように、クライアントがこの情報を取り込みことを確認します。 これは、クライアントがユーザーのメールボックスが Exchange online にあるかどうかに基づくさまざまな動作を期待できるかどうかを調べるのに役立ちます。 または Exchange の設置型の組織。 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Exchange Online を対象とするアプリケーションのテストおよびログ ファイル

Exchange Online は、EWS のプロトコル ログ ファイル、EWS のパフォーマンス カウンター、および、オンプレミスの Exchange サーバーで利用可能なサービスの EWS に関連するイベントへのアクセスは提供されません。 これらへのアクセスでは、EWS と対話するときに、アプリケーションを実行する方法を発見するためのに便利です。 パフォーマンスを最適化することができるように、テスト、オンプレミスの Exchange サーバーに対して、アプリケーションをテストすることを確認します。 可能であれば、Exchange Online に接続する場合、アプリケーションの動作を評価するために Exchange Online では、スロットルの設定を一致するようにテスト サーバーで[制限の設定を変更](http://technet.microsoft.com/en-us/library/bb232205%28v=exchg.150%29.aspx#Policies)することできます。 
  
> [!TIP]
> EWS のロード テストを実行するのに、 [EWSRelentless](https://ewsrelentless.codeplex.com/)ツールを使用することができます。 EWS が負荷の下で実行する方法を理解するために、テスト サーバー、EWS のプロトコル ログ、EWS のパフォーマンス カウンター、サービス ・ イベント、および EWS の調整の設定でこのツールを使用できます。 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>調整設定と Exchange Online

[EWS のスロットル設定](ews-throttling-in-exchange.md)の既定値は、設置型の Exchange よりも、Exchange Online の異なります。 また、Exchange Online の調整の設定は変更できません。 Exchange 管理シェル コマンドレットを使用すると、設置型の Exchange はスロットルの設定を見つけることができます。ただし、これらのコマンドレットは、Exchange Online では無効です。 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Exchange 管理シェルのコマンドレットと構成設定

コマンドレットの多くは、Exchange Online および Exchange オンプレミスの Web サービス API に直接または間接的に影響を与える可能性があります。コマンドレットは、Exchange Online で以下には利用できません。
  
- 調整設定  
    
- 仮想ディレクトリ設定  
    
- 認証設定
    
Exchange のオンラインで利用可能なコマンドレットの詳細については、 [Exchange Online の PowerShell コマンドレット](http://help.outlook.com/en-us/140/dd575549.aspx)を参照してください。 設置型の Exchange で使用可能なコマンドレットの詳細については、 [Exchange 2013 のコマンドレット](http://technet.microsoft.com/en-us/library/bb124413%28v=exchg.150%29.aspx)を参照してください。
  
## <a name="client-affinity-and-network-load-balancers"></a>クライアント アフィニティとネットワーク負荷分散装置
<a name="affinity"> </a>

EWS のほとんどの通信では、Exchange との類似性を維持するためにクライアントが参加する必要はありません。 メールボックス イベントへのサブスクリプションは、cookie およびその他の情報をユーザーのメールボックス イベント キューを管理している Exchange サーバーとのアフィニティを維持するためにクライアントが提供することは必要があります。 Exchange Server 2010 では、ネットワーク負荷分散装置の間でクライアントのアフィニティを維持するために、exchangecookie を使用します。 オンラインの Exchange および Exchange のオンプレミス Exchange 2013 以降のバージョン、メールボックスの通知用の関係を維持するため[X AnchorMailbox ヘッダー、X PreferServerAffinity ヘッダー、および X BackEndOverrideCookie の cookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained)を使用します。 
  
## <a name="authentication"></a>認証
<a name="auth"> </a>

基本認証または OAuth を使用して Exchange Online でクライアントを認証できます。 Exchange のオンプレミス Exchange 2013 以降のバージョンは、既定では NTLM を使用します。ただし、基本認証にも使用するオンプレミスの Exchange を構成することができます。 
  
## <a name="client-latency-diagnostics"></a>クライアントの待機時間診断
<a name="diag"> </a>

Exchange Online に収集報告があった場合のクライアントの遅延の診断をします。 マイクロソフトのサポートを Exchange Online に接続に関する問題のトラブルシューティングに役立ちます。 Exchange の設置型では、クライアントの遅延の診断は収集しません。 クライアントは、Exchange の設置型をターゲットとしている場合、クライアントはサーバーに遅延の診断を報告できません。
  
## <a name="functionality-in-the-ews-managed-api"></a>EWS マネージ API の機能
<a name="ewsma"> </a>

EWS のマネージ API では、Exchange 設置、サービス ポイントの接続の参照、およびいくつかの機能を Exchange Online では、クライアントの遅延の報告などのように固有のいくつかの機能を公開します。 EWS のマネージ API では実装前に、Exchange Online で実装される機能の一部にできることに注意してください。 
  
次の EWS マネージ API 機能は、Exchange Online にのみ適用できます。
  
- クライアントの待機時間レポート
    
- 基本事前認証
    
- 応答で RequestId が返されることを要求する機能
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Exchange Online プランと Exchange サーバー エディションの API 機能
<a name="exo"> </a>

さまざまな機能セットは、さまざまな Office 365 および Exchange Online の計画、または Exchange Server の標準とエンタープライズのバージョンで利用可能な可能性があります。 いくつかの API 機能できない可能性があります Exchange Online の計画や、ユーザーのメールボックスをホストする Exchange Server のエディションによって、クライアント ・ アプリケーションに対応します。 
  
**表 3。計画およびエディション間での API 機能のバリエーション**

|**API の機能**|**計画またはエディションの考慮事項**|
|:-----|:-----|
|Exchange の偽装によるアクセスを除く、アカウントへの EWS アクセス  <br/> |許可されていません、[ビジネスのための Office 365-キオスク プラン](http://office.microsoft.com/en-us/business/compare-office-365-kiosk-plans-FX103178917.aspx)。  <br/> |
|ユニファイド メッセージング (UM)  <br/> |Office 365 エンタープライズ (E3) プラン、Exchange Online プラン 2、および Exchange Server 2013 エンタープライズ エディションでのみ利用できます。  <br/> |
|Active Directory ドメイン サービス (AD DS) の統合  <br/> |Office 365 Small Business および Office 365 Small Business Premium プランでは利用できません。  <br/> |
|Information Rights Management、アーカイブ、および訴訟ホールド  <br/> |Office 365 エンタープライズ (E3 および E4) プランでのみ利用できます。  <br/> |
|データ損失防止  <br/> |Office 365 エンタープライズ プラン、Exchange Online プラン 2、および Exchange Server 2013 エンタープライズ エディションでのみ利用できます。  <br/> |
   
機能の可用性を変更することができますので、使用可能な機能が、クライアントに影響を評価するためには、Exchange のオンラインの計画と Exchange Server のエディションを確認することをお勧めします。 [GetServiceConfiguration 操作](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)を使用するか、機能を実装する操作のためのテスト要求を送信することによって、使用可能な機能をチェックするようにクライアントを作成することもできます。 かどうか、機能を使用できないよう、サーバーからの応答を示します。 
  
## <a name="other-considerations"></a>その他の考慮事項
<a name="other"> </a>

Exchange Online ではなく、Exchange オンプレミスを対象としている場合は、次を行うことができます。
  
- Exchange サーバーにインストールされているクライアントを作成します。  
    
- 配信し、作成および EWS およびその他のクライアントに送信するメッセージの内容に影響を与えることができます[カスタムのトランスポート エージェント](../transport-agents/transport-agents-in-exchange-2013.md)をインストールします。 
    
## <a name="see-also"></a>関連項目

- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
- [オンラインの Exchange および Exchange Server 2013 を比較します。](http://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [ビジネス プランのすべての Office 365 を比較します。](http://office.microsoft.com/en-us/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - EWS 負荷生成ツール](https://ewsrelentless.codeplex.com/)
- [Exchange および EWS のマネージ API の web サービス API 機能の可用性](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [EWS の交換で調整](ews-throttling-in-exchange.md)
    

