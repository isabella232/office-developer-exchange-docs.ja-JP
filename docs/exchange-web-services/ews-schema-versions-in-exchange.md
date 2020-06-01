---
title: Exchange の EWS スキーマのバージョン
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d1ab6f9c-ea91-4022-830d-7f7b759e3935
description: EWS スキーマ、それと連動するアプリケーションの設計方法、ならびに各スキーマ バージョンで使用できる機能、およびスキーマと Exchange サービスのバージョンとの関係について説明します。
localization_priority: Priority
ms.openlocfilehash: 6afef658e747b11d9aa5fb7d7a88ba8f5c57ac82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456015"
---
# <a name="ews-schema-versions-in-exchange"></a>Exchange の EWS スキーマのバージョン

EWS スキーマ、それと連動するアプリケーションの設計方法、ならびに各スキーマ バージョンで使用できる機能、およびスキーマと Exchange サービスのバージョンとの関係について説明します。
  
EWS スキーマは、Exchange に送信でき、Exchange が返すことのできるデータ構造体を定義したものです。 EWS 機能の大幅な変更を含む新しいバージョンの Exchange にはそれぞれ、新しいスキーマがあります。 EWS と EWS スキーマは両方とも下位互換ですが、上位互換の場合もあります。以前のバージョンの EWS に基づいて設計されたアプリケーションは、ほとんどの場合に、その後のバージョンの EWS とも連動します。後のバージョンの EWS を対象とするアプリケーションは、以前のバージョンに同じ機能が組み込まれていた場合に動作します。 この記事は、EWS スキーマの役割、スキーマのバージョン管理の仕組み、スキーマ バージョンとサービス バージョンの関係、EWS スキーマと連動するアプリケーションの設計方法を理解するうえで役立ちます。 
  
## <a name="role-of-the-ews-schema"></a>EWS スキーマの役割

EWS スキーマには、次の役割があります。
  
- クライアントが使用できる機能セットを定義する。クライアントは、SOAP [自動検出サービス](autodiscover-for-exchange.md)を使用して、サポートされるスキーマ バージョンの一覧を取得できます。こうすることで、クライアントはアクセスできる機能を判別できるようになります。各スキーマ バージョンは [EWS 機能セット](ews-schema-versions-in-exchange.md#bk_features)を表すからです。EWS 用にリリースされた新しいスキーマにはそれぞれ、前のバージョンのスキーマ エンティティに加えて、新機能のためのスキーマ定義が含まれます。このように、EWS は、以前のバージョンの EWS を対象とするアプリケーションをサポートします。
    
- API コントラクトの概要を提供する。このコントラクトを使用して、Exchange との間で送受信できるデータ構造体を判断できます。
    
- 要求を送信するためのバージョン管理メカニズムを提供する。Exchange サーバーの仮想ディレクトリには、サポートされるすべての EWS スキーマ バージョンが含まれます。  
    
## <a name="designing-your-application-with-schema-version-in-mind"></a>スキーマ バージョンを考慮したアプリケーションの設計

それぞれ異なるバージョンの EWS スキーマと連動するアプリケーションを設計するときは、次の点を念頭に置いてください。
  
- スキーマ バージョンに基づいて機能をオン/オフにしてください。 クライアント機能をスキーマ バージョンにマップすること、場合によってはサービスのバージョンにマップすることが必要になります。 次の例は、スキーマおよびサービスのバージョンに基づいて [PropertySet](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) を返します。 
    
  ```cs
  private static PropertySet InitPropertySetByVersion(ExchangeService service)
  {
      PropertySet props;
      // The schema version to target to access the NormalizedBody property 
      // is Exchange2013 or later. The server version to target to access the 
      // NormalizedBody property on an email is 15 or later, which 
      // equates to Exchange 2013.
      if (service.RequestedServerVersion >= ExchangeVersion.Exchange2013 &amp;&amp;
          service.ServerInfo.MajorVersion >= 15)
      {
          props = new PropertySet(EmailMessageSchema.NormalizedBody);
      }
      else
      {
          props = new PropertySet(EmailMessageSchema.Body);
      }
      return props;
  }
  ```

- 使用する機能をサポートする最も古いバージョンの EWS スキーマを使用して、要求をバージョン管理してください。 こうすることで、より多くの潜在的 Exchange サーバーにクライアントを適用できるようになります。 組織のサーバーのみを対象とする基幹業務アプリケーションを開発する場合、これはそれほど重要ではありません。しかし、より広範囲の Exchange ユーザー向けのアプリケーションを構築する場合、これは非常に重要です。
    
## <a name="features-by-schema-version"></a>スキーマ バージョン別の機能
<a name="bk_features"> </a>

クライアントが使用できるスキーマ バージョンは、types.xsd スキーマにある **ExchangeVersionType** 単純型で識別できます。 **ExchangeVersionType** は、[RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 要素によって実装されます。 **RequestServerVersion** 要素はすべての EWS 要求で送信されて、クライアントが対象とするスキーマ バージョンをサーバーに示します。 これは、クライアントが使用できる機能セットを示していることになります。 
  
**表 1: 製品バージョンおよびスキーマ バージョン別の EWS 機能**

|**製品バージョン**|**関連スキーマ バージョン**|**機能**|
|:-----|:-----|:-----|
|Exchange Online  |最新のスキーマ バージョン。  |オンライン クライアント用に追加された新機能に加え、現在のバージョンの Exchange のすべての機能が含まれます。 |
|Exchange 2013 SP1 |Exchange2013_SP1 | Exchange 2013 のすべての機能が含まれます。<br/><br/>次の機能は、Exchange 2013 SP1 で導入されました。 <ul><li>[メールボックス保留ポリシー](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) </li><li> [別の時間を指定](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) </li><li>  アイテムの[更新](https://msdn.microsoft.com/library/office/dn600559%28v=exchg.80%29.aspx)および[削除](https://msdn.microsoft.com/library/office/dn600557%28v=exchg.80%29.aspx)のための開封確認メッセージの更新  </li><li> 会話のための [IRM 情報](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.conversation.hasirm%28v=exchg.80%29.aspx)の更新  </li></ul> |
|Exchange 2013   |Exchange2013   | Exchange 2007 および Exchange 2010 で導入されたすべての機能が含まれます。 <br/><br/>次の機能は、Exchange 2013 で導入されました。<ul><li>アーカイブ  </li><li>  電子情報開示  </li><li>  ペルソナ  </li><li>  アイテム保持ポリシー  </li><li>  統合連絡先ストア  </li><li>  ユーザーの写真  </li></ul> |
|Exchange 2010 SP2   |Exchange2010_SP2 | Exchange 2010 SP1 で導入されたすべての機能が含まれます。 <br/><br/>次の機能は、Exchange 2010 SP2 で導入されました。<ul><li>パスワードの有効期限の取得  </li><li>  DateTime の精度  </li><li>  連絡先のプロパティ識別子の更新  </li><li>  新しい偽装シナリオ  </li></ul> |
|Exchange 2010 SP1  |Exchange2010_SP1   | Exchange 2010 で導入されたすべての機能が含まれます。 <br/><br/>次の機能は、Exchange 2010 SP1 で導入されました。<ul><li>受信トレイ ルールの作成、取得、変更  </li><li>  プログラムによるアーカイブ メールボックスへのアクセス  </li><li>  会話アクション  </li><li>  ファイアウォールを通過する通知  </li><li>  管理機能の向上  </li><li>  混在バージョンのサポートの向上  </li><li>  保護サポートの調整  </li><li>  EWS へのアプリケーション アクセスの制御  </li><li>  クライアント証明書認証サポート  </li></ul> |
|Exchange 2010  |Exchange2010   | Exchange 2007 SP1 で導入されたすべての機能が含まれます。 <br/><br/>次の機能は、Exchange 2010 の最初のリリース バージョンで導入されました。<ul><li>個人用完全配布リスト  </li><li>  ユーザー構成オブジェクト  </li><li>  フォルダーに関連付けられたアイテム  </li><li>  メッセージ追跡  </li><li>  ユニファイド メッセージング  </li><li>  SOAP 自動検出  </li><li>  タイム ゾーン サポートの強化  </li><li>  会議室リソースの空き時間情報  </li><li>  インデックス検索  </li><li>  ごみ箱へのアクセス  </li><li>  メールヒント情報  </li></ul> |
|Exchange 2007 SP1   |Exchange2007_SP1  | Exchange 2007 で導入されたすべての機能が含まれます。 <br/><br/>次の機能は、Exchange 2007 SP1 で導入されました。<ul><li>管理の委任  </li><li>  フォルダーのアクセス許可  </li><li>  パブリック フォルダー  </li><li>  アイテムの投稿  </li><li>  ID 変換  </li></ul>|
|Exchange 2007  |Exchange2007 | 次の機能は、Exchange 2007 の最初のリリース バージョンで導入されました。<ul><li>アイテム、フォルダー、添付ファイルへのフル アクセス (作成、取得、更新、削除)  </li><li>  可用性  </li><li>  不在設定  </li><li>  通知  </li><li>  同期  </li><li>  名前の解決  </li><li>  配布リスト (DL) の展開  </li><li>  検索  </li></ul> |
   
## <a name="relationship-between-the-ews-schema-and-the-service-version"></a>EWS スキーマとサービスのバージョンの関係
<a name="bk_features"> </a>

EWS スキーマ バージョンは、サーバーが実行されている EWS サービスのバージョンに関連しています。 EWS スキーマの名前付けパターンは、オンプレミスの Exchange バージョンに関連しています。 たとえば、Exchange 2013 の最初のリリースでは、サービス バージョンは 15.00.0516.032 で、スキーマ名は **Exchange2013** です。 Exchange 2013 のスキーマが更新されたため、サービス バージョンが 15.00.0516.032 以降の Exchange 2013 と Exchange Online は両方とも、最新スキーマを表す同じバージョン名を持ちます。 以前のバージョンの Exchange では、EWS スキーマは累積的な更新 (旧称ロールアップ) で更新されませんでした。 しかし、Exchange Online をサポートするために Exchange がより頻繁に更新されるため、累積的な更新に EWS のスキーマ更新が含まれるようになりました。 スキーマ ファイル名とそれに関連するスキーマ バージョン名は、オンプレミス Exchange のサービス パックまたはメジャー リリースでのみ更新されます。
  
EWS スキーマはコントラクトを定義しますが、シナリオによっては、サービス バージョンは、クライアントがサービスとどのように対話することになるかを判断するための唯一の手段です。 スキーマに反映されていないサービスの動作の変更は、すべての EWS 応答で返されるサービス バージョンによってのみ確認できます。 たとえば、Exchange 2013 で[パブリック フォルダー](public-folder-access-with-ews-in-exchange.md)が再設計されたとき、パブリック フォルダーの移動とコピーに使用される操作も変わりました。 Exchange 2010 でパブリック フォルダーをコピーするためのクライアントを設計した場合、Exchange 2013 で同じ結果を得るには、異なる操作を使用するようにクライアントを更新することが必要になります。 
  
## <a name="how-the-ews-schema-is-updated"></a>EWS スキーマの更新のされ方
<a name="bk_features"> </a>

Exchange 2007 以降のバージョンの Exchange を実行する Exchange サーバーでは、EWS サービスをホストする仮想ディレクトリに EWS スキーマがあります。現在のスキーマ バージョンは常に、types.xsd ファイルと messages.xsd ファイルによって表されます。図 1 は、新しいバージョンのスキーマを開発するときに messages.xsd スキーマがどのようにフォークされるかを示しています。新機能が追加される前に、元の messages.xsd スキーマのコピーが取り込まれ、前のバージョンのスキーマを表す名前に変更されます。次に messages.xsd ファイルが、新しいバージョンのサービスの説明を使用して更新されます。
  
**図 1. EWS スキーマの更新のされ方**

![EWS スキーマが更新される方法を示した図。最新のスキーマ バージョンはフォークされて 1 つ前のバージョンを示す名前が付けられ、最新のファイル名が現行バージョンを表します。](media/Ex15_EWS_Schema_Update1.png)
  
EWS スキーマが新しいバージョン用に更新される前に、現在のバージョンのスキーマがフォークされ、次の規則に従って名前が変更されます。
  
`<schemaname>-<majorserverversion><servicepack>.xsd`
  
元のファイル名が最新スキーマを表すようになります。以前のバージョンのスキーマの更新と修正を除いて、すべての新機能が最新スキーマに追加されます。  
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS スキーマのバージョン](ews-schema-versions-in-exchange.md) 
- [Exchange の自動検出](autodiscover-for-exchange.md) 
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

