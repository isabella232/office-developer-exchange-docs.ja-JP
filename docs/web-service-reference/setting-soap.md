---
title: Setting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: Setting 要素は、返される構成設定を表します。
ms.openlocfilehash: 2e03bfacaf36676ee4687c148f3b08732a9f17b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539144"
---
# <a name="setting-soap"></a>Setting (SOAP)

**Setting 要素** は、返される構成設定を表します。 
  
```XML
<Setting/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は構成設定です。 次の表に、使用可能な構成設定の一覧を示します。
  
|**構成設定**|**説明**|
|:-----|:-----|
|userDisplayName  <br/> |ユーザーの表示名。  <br/> |
|UserDN  <br/> |ユーザーの従来の識別名。  <br/> |
|UserDeploymentId  <br/> |ユーザーの展開識別子。  <br/> |
|InternalMailboxServer  <br/> |メールボックス サーバーの完全修飾ドメイン名 (FQDN) です。  <br/> |
|InternalRpcClientServer  <br/> |RPC クライアント サーバーの完全修飾ドメイン名。  <br/> |
|InternalMailboxServerDN  <br/> |メールボックス サーバーの従来の識別名。  <br/> |
|InternalEcpUrl  <br/> |コントロール パネルの内部 URL Exchangeします。  <br/> |
|InternalEcpVoicemailUrl  <br/> |VoiceMail カスタマイズ用の Exchangeコントロール パネルの内部 URL。  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |電子メール サブスクリプションのExchangeコントロール パネルの内部 URL。  <br/> |
|InternalEcpTextMessagingUrl  <br/> |テキスト メッセージング用のExchangeコントロール パネルの内部 URL。  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |配信レポートのExchangeの内部 URL。  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |RetentionPolicy タグExchangeコントロール パネルの内部 URL。  <br/> |
|InternalEcpPublishingUrl  <br/> |[発行] コントロール Exchangeの内部 URL。  <br/> |
|InternalEwsUrl  <br/> |Web サービスのExchange URL。  <br/> |
|InternalOABUrl  <br/> |オフライン アドレス帳 (OAB) の内部 URL。  <br/> |
|InternalUMUrl  <br/> |ユニファイド メッセージング サービスの内部 URL。  <br/> |
|InternalWebClientUrls  <br/> |Web クライアントの内部 URL Exchangeします。  <br/> |
|MailboxDN  <br/> |ユーザーのメールボックスのメールボックス データベースの識別名。  <br/> |
|PublicFolderServer  <br/> |パブリック フォルダー サーバーの名前。  <br/> |
|ActiveDirectoryServer  <br/> |Active Directory サーバーの名前。  <br/> |
|ExternalMailboxServer  <br/> |HTTP サーバー上の RPC の名前。  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |RPC over HTTP サーバーが SSL を必要とするかどうかを示すインジケーター。  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |RPC over HTTP サーバーでサポートされる認証方法。  <br/> |
|EcpVoicemailUrlFragment,  <br/> |VoiceMail カスタマイズ用のExchangeコントロール パネルの URL フラグメント。  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |電子メール サブスクリプションのExchangeコントロール パネルの URL フラグメント。  <br/> |
|EcpTextMessagingUrlFragment  <br/> |テキスト メッセージング用の Exchangeコントロール パネルの URL フラグメント。  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |配信レポート用のExchangeコントロール パネルの URL フラグメント。  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |RetentionPolicy タグExchangeコントロール パネルの URL フラグメント。  <br/> |
|EcpPublishingUrlFragment  <br/> |発行のコントロール パネルExchange URL フラグメント。  <br/> |
|ExternalEcpUrl  <br/> |コントロール パネルのExchange URL。  <br/> |
|ExternalEcpVoicemailUrl  <br/> |VoiceMail カスタマイズ用の Exchangeコントロール パネルの外部 URL。  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |電子メール サブスクリプションの Exchangeコントロール パネルの外部 URL。  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |テキスト メッセージング用の Exchangeコントロール パネルの外部 URL。  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |配信レポートのコントロール Exchangeの外部 URL。  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |RetentionPolicy タグExchangeコントロール パネルの外部 URL。  <br/> |
|ExternalEcpPublishingUrl  <br/> |発行用のコントロール Exchangeの外部 URL。  <br/> |
|ExternalEwsUrl  <br/> |Web サービスのExchange URL。  <br/> |
|ExternalOABUrl  <br/> |OAB の外部 URL。  <br/> |
|ExternalUMUrl  <br/> |ユニファイド メッセージング サービスの外部 URL。  <br/> |
|ExternalWebClientUrls  <br/> |Web クライアントのExchange URL。  <br/> |
|CrossOrganizationSharingEnabled  <br/> |組織間の共有が有効になっているかどうかを示します。  <br/> |
|AlternateMailboxes  <br/> |代替メールボックスのコレクション。  <br/> |
|CasVersion  <br/> |要求を処理しているクライアント アクセス サーバーのバージョン (たとえば、14.XX.YYYYY)。ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Web サービスでサポートされるスキーマ のバージョンのコンマExchange一覧。 スキーマ バージョンの値は **、ExchangeServerVersion** 列挙の値と同じです。  <br/> |
|InternalPop3Connections  <br/> |POP3 プロトコル接続の内部接続設定リスト。  <br/> |
|ExternalPop3Connections  <br/> |POP3 プロトコル接続の外部接続設定リスト。  <br/> |
|InternalImap4Connections  <br/> |IMAP4 プロトコル接続の内部接続設定リスト。  <br/> |
|ExternalImap4Connections  <br/> |IMAP4 プロトコル接続の外部接続設定リスト。  <br/> |
|InternalSmtpConnections  <br/> |SMTP 接続の内部接続設定リスト。  <br/> |
|ExternalSmtpConnections  <br/> |SMTP 接続の外部接続設定リスト。  <br/> |
|InternalServerExclusiveConnect  <br/> |内部サーバー排他的接続フラグ。 "Off" に設定されている場合、クライアントは、このプロトコルを介して接続しない必要があります。  <br/> |
|ExternalServerExclusiveConnect  <br/> |外部サーバー排他的接続フラグ。 "On" に設定されている場合、クライアントは、このプロトコルを介して接続する必要があります。  <br/> |
|ExchangeRpcUrl  <br/> |リモート プロシージャ呼び出しに使用される URL。 この URL はサーバーの内部であり、クライアントでは使用されません。  <br/> |
|ShowGalAsDefaultView  <br/> |アドレス帳として GAL を表示するかどうかを示すブール値を指定します。 "true" のテキスト値は、GAL が既定で表示されるかどうかを示します。 "false" のテキスト値は、連絡先リストが表示されるかどうかを示します。  <br/> |
|AutoDiscoverSMTPAddress  <br/> |ユーザーの自動検出プライマリ SMTP アドレス。 これは、プロキシ アドレスが存在する場合、ユーザーの電子メール アドレスの代用のプロキシ アドレスです。  <br/> |
|InteropExternalEwsUrl  <br/> |サーバーの Web サービス エンドポイントの外部 URL。 これは、Web サービスを持つサーバーでホストされているメールボックスにサービスを提供できるサーバーの URL です。  <br/> |
|ExternalEwsVersion  <br/> |指定した要求を配信している Web サービス サーバーのバージョン。  <br/> |
|InteropExternalEwsVersion  <br/> |InteropExternalEwsUrl が指しているサーバーのバージョン。  <br/> |
|MobileMailboxPolicyInterop  <br/> |モバイル メールボックス ポリシーの設定。  <br/> |
|GroupingInformation  <br/> |通知をサブスクライブするときにアフィニティを維持するために複数のメールボックスをグループ化するために ExternalEwsUrl 設定と組み合わせて使用される値。 [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)  <br/> |
|UserMSOnline  <br/> |ユーザーのメールボックスがユーザーのメールボックスでホストされているかどうかを示すブールExchange OnlineまたはExchange Onlineの一部Office 365。  <br/> |
|MapiHttpEnabled  <br/> |MAPI/HTTP プロトコルを介してユーザーのメールボックスにアクセスできるかどうかを示すブール値。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

