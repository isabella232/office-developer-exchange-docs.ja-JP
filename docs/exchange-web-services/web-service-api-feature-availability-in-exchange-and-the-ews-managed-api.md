---
title: Exchange および EWS Managed API の Web サービス API 機能の可用性
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: EWS および Web サービス API のどの機能が Exchange および EWS マネージ API の各バージョンで使用できるかについて説明します。
ms.openlocfilehash: d19ab062c8d418e373e8268b1ab039e5436e71bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759192"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Exchange および EWS Managed API の Web サービス API 機能の可用性

EWS および Web サービス API のどの機能が Exchange および EWS マネージ API の各バージョンで使用できるかについて説明します。
  
Exchange クライアント アプリケーションは、Exchange のバージョンの多くを多くの場合対象します。 このため、アプリケーションを設計することができます[EWS クライアントの機能](ews-client-design-overview-for-exchange.md#EWSFeatures)の有効と無効、ユーザーのメールボックスをホストする Exchange のバージョンに基づくようにする場合があります。 この資料では、サービス API の機能については、別のバージョンの Exchange および EWS のマネージ API で使用可能な情報を提供します。 この情報を使用すると、複数のバージョンの Exchange を実行しているお客様に広範に適用するのにようにアプリケーションをデザインできます。 
  
Exchange のバージョンの違いの詳細については、EWS のスキーマ ファイルおよび関連する[リファレンス ドキュメント](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)を確認します。
  
## <a name="api-features-by-exchange-version"></a>Exchange バージョンごとの API 機能
<a name="bk_apifeatures"> </a>

EWS および Autodiscover を含む Exchange Web サービス API は、複数バージョンの互換性を念頭に置いて開発されています。したがって、Exchange 2007 を対象とするアプリケーションは、Exchange Online および Office 365 の一部としての Exchange Online を含め、Exchange 2013 以降のバージョンの Exchange でも有効です。  
  
次の表では、どの API 機能が Exchange の各バージョン、および 2.0 以降の EWS マネージ API バージョンで使用できるかを示します。アプリケーションは Exchange の複数のバージョンを対象としていることがあるため、クライアントが実装する機能をどのバージョンがサポートしているかを把握するのに役立ちます。自動検出サービスを使用すると、クライアントがユーザー向けに対象としている Exchange のバージョンを検出できるため、ユーザーが利用できるかどうかに応じてこの機能をオンまたはオフに設定することができます。
  
**表 1 です。バージョンの Exchange および EWS のマネージ API で使用できる web サービス機能**

|API の機能|Exchange Online (Office 365)|EWS Managed API|Exchange 2013|Exchange 2010 SP2|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|あいまいな名前の解決  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Outlook 管理用のアプリ  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[アーカイブ メールボックスへのアクセス](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[(POX) を自動検出](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[(SOAP) を自動検出](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|自動応答 (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|可用性  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|可用性 (会議室)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|一括転送  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|連絡先グループ  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|会話の管理  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|DateTime の精度  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|管理の委任  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|配布リストの展開  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[ごみ箱をあさるアクセス](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[電子的証拠開示](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|強化されたタイム ゾーン  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|フォルダーのアクセス許可  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[識別子変換](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[受信トレイの管理](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[アイテムおよびフォルダーのアクセス](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[メールボックスのイベント (プル サブスクリプションおよびプッシュ)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[メールボックス イベント)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|メール ヒント  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|パスワードの期限切れ  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[ペルソナ](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|アイテムの投稿  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[パブリック フォルダーへのアクセス](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|アイテム保持ポリシー  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[(インデックス) を検索](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[検索 (ストア)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[同期](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[統合連絡先ストア](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[ユニファイド メッセージング Web サービス](http://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|ユニファイド メッセージング (EWS ベース)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[ユーザー設定オブジェクト](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[ユーザーの写真](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Web の詳細については、サービスの機能については、 [EWS の操作](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)、[自動検出サービス](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)、および[ExchangeService メソッド](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx)の異なるバージョンの Exchange で使用できる検索ことができます。
  
## <a name="to-learn-more"></a>詳細情報
<a name="bk_apifeatures"> </a>

Exchange の各バージョンに固有の違いについては、次のいずれかで理解できます。
  
- 詳細内の各バージョンの違いを調査するのには、 [EWS のスキーマ](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)について説明します。 
    
- [EWSEditor](http://ewseditor.codeplex.com/)をダウンロードします。 EWSEditor を使用するには別のターゲット スキーマ バージョンを指定し、ターゲット スキーマのバージョンに基づいて、クエリを送信します。
    
## <a name="see-also"></a>関連項目

- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)   
- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md) 
- [Exchange は何です新しい EWS およびその他の web サービス](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

