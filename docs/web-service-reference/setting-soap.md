---
title: (SOAP) の設定
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: 設定要素は、返される構成設定を表します。
ms.openlocfilehash: cb5b1d6ab2109b48810b96221b76c6b8fc9803ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833472"
---
# <a name="setting-soap"></a>(SOAP) の設定

**設定**要素は、返される構成設定を表します。 
  
```XML
<Setting/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、構成設定です。 次の表は、可能な構成の設定をします。
  
|**構成の設定**|**説明**|
|:-----|:-----|
|UserDisplayName  <br/> |ユーザーの表示名。  <br/> |
|UserDN  <br/> |ユーザーの従来の識別名です。  <br/> |
|UserDeploymentId  <br/> |ユーザーの展開の識別子です。  <br/> |
|InternalMailboxServer  <br/> |メールボックス サーバーの完全修飾ドメイン名 (FQDN) です。  <br/> |
|InternalRpcClientServer  <br/> |RPC クライアント サーバーの完全修飾ドメイン名です。  <br/> |
|InternalMailboxServerDN  <br/> |メールボックス サーバーの従来の識別名です。  <br/> |
|InternalEcpUrl  <br/> |Exchange の [コントロール パネル] の内部 URL です。  <br/> |
|InternalEcpVoicemailUrl  <br/> |ボイスメールのカスタマイズ用の Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |電子メール購読の Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEcpTextMessagingUrl  <br/> |テキスト メッセージングの Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |配信レポートの場合、Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |RetentionPolicy タグの Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEcpPublishingUrl  <br/> |公開の Exchange コントロール パネルの内部の URL です。  <br/> |
|InternalEwsUrl  <br/> |内部 URL の Exchange Web サービスです。  <br/> |
|InternalOABUrl  <br/> |オフライン アドレス帳 (OAB) の内部の URL です。  <br/> |
|InternalUMUrl  <br/> |ユニファイド メッセージング サービスの内部 URL です。  <br/> |
|InternalWebClientUrls  <br/> |Exchange Web クライアントの内部 Url です。  <br/> |
|MailboxDN  <br/> |ユーザーのメールボックスのメールボックス データベースの識別名です。  <br/> |
|PublicFolderServer  <br/> |パブリック フォルダー サーバーの名前です。  <br/> |
|ActiveDirectoryServer  <br/> |Active Directory サーバーの名前。  <br/> |
|ExternalMailboxServer  <br/> |RPC over HTTP サーバーの名前。  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |RPC over HTTP サーバーが SSL を要求するかどうかを示すインジケーターです。  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |HTTP サーバー上で RPC がサポートされている認証方法です。  <br/> |
|EcpVoicemailUrlFragment、  <br/> |ボイスメールのカスタマイズ用の Exchange コントロール パネルの URL フラグメントです。  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |電子メール購読の Exchange コントロール パネルの URL フラグメントです。  <br/> |
|EcpTextMessagingUrlFragment  <br/> |テキスト メッセージングの Exchange コントロール パネルの URL フラグメントです。  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |配信レポートの場合、Exchange コントロール パネルの URL フラグメントです。  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |RetentionPolicy タグの Exchange コントロール パネルの URL フラグメントです。  <br/> |
|EcpPublishingUrlFragment  <br/> |公開の Exchange コントロール パネルの URL フラグメントです。  <br/> |
|ExternalEcpUrl  <br/> |コントロール パネルの [Exchange の外部の URL です。  <br/> |
|ExternalEcpVoicemailUrl  <br/> |ボイスメールのカスタマイズ用の Exchange コントロール パネルの外部の URL です。  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |電子メール購読の Exchange コントロール パネルの外部の URL です。  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |Exchange コントロール パネルで、テキスト メッセージングの外部 URL です。  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |Exchange コントロール パネルの配信レポートの外部の URL です。  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |RetentionPolicy タグの Exchange コントロール パネルの外部の URL です。  <br/> |
|ExternalEcpPublishingUrl  <br/> |公開の Exchange コントロール パネルの外部の URL です。  <br/> |
|ExternalEwsUrl  <br/> |Exchange Web サービスの外部 URL です。  <br/> |
|ExternalOABUrl  <br/> |OAB の外部の URL です。  <br/> |
|ExternalUMUrl  <br/> |ユニファイド メッセージング サービスの外部 URL です。  <br/> |
|ExternalWebClientUrls  <br/> |Exchange Web クライアントの外部の Url です。  <br/> |
|CrossOrganizationSharingEnabled  <br/> |組織間の共有が有効になっていることを示します。  <br/> |
|AlternateMailboxes  <br/> |メールボックスを別のコレクションです。  <br/> |
|CasVersion  <br/> |バージョンのクライアント アクセス サーバーがサービス要求 (たとえば、14.XX です。YYYY。ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Exchange Web サービスでサポートされているスキーマ バージョンのコンマ区切りのリスト。 スキーマ バージョンの値は、 **ExchangeServerVersion**列挙型の値と同じになります。  <br/> |
|InternalPop3Connections  <br/> |POP3 プロトコル接続の内部接続の設定の一覧です。  <br/> |
|ExternalPop3Connections  <br/> |POP3 プロトコル接続の外部接続の設定の一覧です。  <br/> |
|InternalImap4Connections  <br/> |IMAP4 プロトコル接続の内部接続の設定の一覧です。  <br/> |
|ExternalImap4Connections  <br/> |IMAP4 プロトコル接続の外部接続の設定の一覧です。  <br/> |
|InternalSmtpConnections  <br/> |SMTP 接続の内部接続の設定の一覧です。  <br/> |
|ExternalSmtpConnections  <br/> |SMTP 接続の外部接続の設定の一覧です。  <br/> |
|InternalServerExclusiveConnect  <br/> |フラグを排他的な内部サーバーに接続します。 かどうかに設定し、クライアントを「オフ」に接続しないでくださいこのプロトコルを使用しています。  <br/> |
|ExternalServerExclusiveConnect  <br/> |フラグを排他的な外部のサーバーに接続します。 場合は [オン]、[クライアントに設定するにする必要がありますこのプロトコル経由で接続します。  <br/> |
|ExchangeRpcUrl  <br/> |リモート プロシージャ コールに使用する URL です。 この URL は、サーバーの内部クライアントが使用するのには。  <br/> |
|ShowGalAsDefaultView  <br/> |アドレス帳とグローバル アドレス一覧を表示するかどうかを示すブール値を指定します。 文字列値"true"は、グローバル アドレス一覧が既定で表示することを示します。 "False"のテキスト値は、その連絡先リストが表示されることを示します。  <br/> |
|AutoDiscoverSMTPAddress  <br/> |ユーザーの自動検出プライマリ SMTP アドレスです。 これは、プロキシ アドレスが存在する場合に、ユーザーの電子メール アドレスの代わりにプロキシのアドレスです。  <br/> |
|InteropExternalEwsUrl  <br/> |外部の Web サービス エンドポイントの URL です。 これは、Web サービスがないサーバーでホストされているメールボックスを使用できるサーバーの URL です。  <br/> |
|ExternalEwsVersion  <br/> |指定された要求を配信する Web サービスのサーバーのバージョンです。  <br/> |
|InteropExternalEwsVersion  <br/> |InteropExternalEwsUrl サーバーのバージョンを指します。  <br/> |
|MobileMailboxPolicyInterop  <br/> |モバイル メールボックス ポリシーの設定。  <br/> |
|GroupingInformation  <br/> |通知を購読する場合は、[アフィニティを維持](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するために複数のメールボックスをグループ化する ExternalEwsUrl の設定と組み合わせて使用する値です。  <br/> |
|UserMSOnline  <br/> |Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示すブール値です。  <br/> |
|MapiHttpEnabled  <br/> |ユーザーのメールボックスに MAPI または HTTP プロトコル経由でアクセスできるかどうかを示すブール値です。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

