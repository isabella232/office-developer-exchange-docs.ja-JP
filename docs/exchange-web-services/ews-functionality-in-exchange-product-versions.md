---
title: Exchange 製品バージョン別の EWS 機能
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: 新しい製品リリースでは、EWS により新機能が実装されます。 この資料の内容を読み、対象としている Exchange のバージョンに、アクセスするデータや機能のサポートが含まれているかどうか判断してください。
ms.openlocfilehash: bccd0e84fc28f8a7366f0463e555cceec71aa181
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512283"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Exchange 製品バージョン別の EWS 機能

新しい製品リリースでは、EWS により新機能が実装されます。 この資料の内容を読み、対象としている Exchange のバージョンに、アクセスするデータや機能のサポートが含まれているかどうか判断してください。 
  
次の表は、EWS が組み込まれている Exchange のバージョンと、各バージョンで導入された主な機能を記しています。
  
## <a name="ews-features-by-product-version"></a>製品バージョン別の EWS 機能

|**製品バージョン**|**機能**|
|:-----|:-----|
|Office 365 および Exchange Online |オンライン クライアント用に追加された新機能に加え、現在のバージョンの Exchange のすべての機能が含まれます。  |
|Exchange 2013 SP1 | Exchange 2013 で導入されたすべての機能が含まれます。 次の機能は、Exchange 2013 SP1 で導入されました。<ul><li>更新および削除のため、開封確認を中断することができます。</li><li>[モデレート トランスポート](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx)の承認情報を取得することができます。</li><li>返信応答を表示することができます。</li><li>[SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) メソッドと [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) 操作は、単一オブジェクト内のすべてのパラメーターを受け付けます。</li><li>電子情報開示の検索では、検索クエリの言語と、日付範囲のカルチャ固有の書式を指定できます。</li><li>[StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) オブジェクトが、[StreamingSubscription](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) オブジェクトにアクセスできるようになりました。</li><li>会話には、IRM で保護された電子メール メッセージが含まれているかどうかを表示させる設定があります。</li><li>会議出席者は、会議の新しい開始と終了日時を提案し、会議の応答に含めることができます。</li><li>SOAP 自動検出 [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) メソッドが、複数のメールボックス イベント サブスクリプションのアフィニティ維持に使用する [GroupingInformation](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) 設定を返すようになりました。</li></ul> |
|Exchange 2013  | Exchange 2010 SP2 で導入されたすべての機能が含まれます。 次の機能は、Exchange 2013 で導入されました。  <ul><li>  アーカイブ</li><li>電子情報開示</li><li>ペルソナ</li><li>アイテム保持ポリシー</li><li>統合連絡先ストア</li><li>ユーザーの写真</li></ul> |
|Exchange 2010 SP2  | Exchange 2010 SP1 で導入されたすべての機能が含まれます。次の機能は、Exchange 2010 SP2 で導入されました。  <ul><li>  パスワードの有効期限の取得</li><li>DateTime の精度</li><li>連絡先のプロパティ識別子の更新</li><li>新しい偽装シナリオ</li></ul> |
|Exchange 2010 SP1  | Exchange 2010 で導入されたすべての機能が含まれます。次の機能は、Exchange 2010 SP1 で導入されました。  <ul><li>  受信トレイ ルールの作成、取得、変更</li><li>プログラムによるアーカイブ メールボックスへのアクセス</li><li>会話アクション</li><li>ファイアウォールを通過する通知</li><li>管理機能の向上</li><li>混在バージョンのサポートの向上</li><li>保護サポートの調整</li><li>EWS へのアプリケーション アクセスの制御</li><li>クライアント証明書認証サポート</li></ul> |
|Exchange 2010  | Exchange 2007 SP1 で導入されたすべての機能が含まれます。次の機能は、Exchange 2010 の初期リリース バージョンで導入されました。 <ul> <li>  個人用完全配布リスト</li><li>ユーザー構成オブジェクト</li><li>フォルダーに関連付けられたアイテム</li><li>メッセージ追跡</li><li>ユニファイド メッセージング</li><li>SOAP 自動検出  </li><li>タイム ゾーン サポートの強化</li><li>会議室リソースの空き時間情報</li><li>インデックス検索</li><li>ごみ箱へのアクセス</li><li>メールヒント情報</li></ul> |
|Exchange 2007 SP1  | Exchange 2007 で導入されたすべての機能が含まれます。次の機能は、Exchange 2007 SP1 で導入されました。  <ul><li>  管理の委任</li><li>フォルダーのアクセス許可</li><li>パブリック フォルダー</li><li>アイテムの投稿</li><li>ID 変換</li></ul> |
|Exchange 2007  | 次の機能は、Exchange 2007 の最初のリリース バージョンで導入されました。  <ul><li>  アイテム、フォルダー、添付ファイルへのフル アクセス (作成、取得、更新、削除)</li><li>可用性</li><li>不在設定</li><li>通知</li><li>同期</li><li>名前の解決</li><li>配布リスト (DL) の展開</li><li>検索</li></ul> |
   
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
- [Exchange テクノロジへの移行](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

