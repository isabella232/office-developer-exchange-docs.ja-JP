---
title: Setting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: Setting 要素は、返される構成設定を表します。
ms.openlocfilehash: df3b55fe7ba2c5ae92f8c31ec0643dbe100fa072
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466746"
---
# <a name="setting-soap"></a>Setting (SOAP)

**Setting**要素は、返される構成設定を表します。 
  
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
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、構成設定です。 次の表に、使用可能な構成設定を示します。
  
|**構成設定**|**説明**|
|:-----|:-----|
|userDisplayName  <br/> |ユーザーの表示名。  <br/> |
|UserDN  <br/> |ユーザーの従来の識別名。  <br/> |
|UserDeploymentId  <br/> |ユーザーの展開識別子。  <br/> |
|InternalMailboxServer  <br/> |メールボックスサーバーの完全修飾ドメイン名 (FQDN)。  <br/> |
|InternalRpcClientServer  <br/> |RPC クライアントサーバーの完全修飾ドメイン名。  <br/> |
|InternalMailboxServerDN  <br/> |メールボックスサーバーの従来の識別名。  <br/> |
|InternalEcpUrl  <br/> |Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEcpVoicemailUrl  <br/> |ボイスメールカスタマイズ用の Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |電子メール購読のための Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEcpTextMessagingUrl  <br/> |テキストメッセージング用の Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |配信レポート用の Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |Get-retentionpolicy タグの Exchange コントロールパネルの内部 URL。  <br/> |
|Internalecpはっこう Url  <br/> |発行用の Exchange コントロールパネルの内部 URL。  <br/> |
|InternalEwsUrl  <br/> |Exchange Web サービスの内部 URL。  <br/> |
|インターネットの Url  <br/> |オフラインアドレス帳 (OAB) の内部 URL。  <br/> |
|InternalUMUrl  <br/> |ユニファイドメッセージングサービスの内部 URL。  <br/> |
|InternalWebClientUrls  <br/> |Exchange Web クライアントの内部 Url。  <br/> |
|MailboxDN  <br/> |ユーザーのメールボックスのメールボックスデータベースの識別名。  <br/> |
|PublicFolderServer  <br/> |パブリックフォルダーサーバーの名前。  <br/> |
|ActiveDirectoryServer  <br/> |Active Directory サーバーの名前。  <br/> |
|ExternalMailboxServer  <br/> |RPC over HTTP サーバーの名前。  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |RPC over HTTP サーバーが SSL を必要とするかどうかを示すインジケーター。  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |RPC over HTTP サーバーでサポートされている認証方法。  <br/> |
|EcpVoicemailUrlFragment,  <br/> |ボイスメールカスタマイズ用の Exchange コントロールパネルの URL フラグメント。  <br/> |
|Ecpemailsubscription急増 Lfragment  <br/> |電子メール購読のための Exchange コントロールパネルの URL フラグメント。  <br/> |
|EcpTextMessagingUrlFragment  <br/> |テキストメッセージング用の Exchange コントロールパネルの URL フラグメント。  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |配信レポート用の Exchange コントロールパネルの URL フラグメント。  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Get-retentionpolicy タグの Exchange コントロールパネルの URL フラグメント。  <br/> |
|Ecpはっこう Urlfragment  <br/> |発行用の Exchange コントロールパネルの URL フラグメント。  <br/> |
|ExternalEcpUrl  <br/> |Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEcpVoicemailUrl  <br/> |ボイスメールカスタマイズ用の Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |電子メール購読のための Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |テキストメッセージング用の Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |配信レポート用の Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |Get-retentionpolicy タグの Exchange コントロールパネルの外部 URL。  <br/> |
|Externalecp発行 Url  <br/> |発行用の Exchange コントロールパネルの外部 URL。  <br/> |
|ExternalEwsUrl  <br/> |Exchange Web サービスの外部 URL。  <br/> |
|ExternalOABUrl  <br/> |OAB の外部 URL。  <br/> |
|ExternalUMUrl  <br/> |ユニファイドメッセージングサービスの外部 URL。  <br/> |
|ExternalWebClientUrls  <br/> |Exchange Web クライアントの外部 Url。  <br/> |
|クロス組織の有効化  <br/> |組織間共有が有効になっていることを示します。  <br/> |
|AlternateMailboxes  <br/> |代替メールボックスのコレクション。  <br/> |
|CasVersion  <br/> |要求を処理しているクライアントアクセスサーバーのバージョン (たとえば、14.。YYYY.ZZZ  <br/> |
|EwsSupportedSchemas  <br/> |Exchange Web サービスによってサポートされるスキーマバージョンのコンマ区切りのリスト。 スキーマバージョンの値は、 **ExchangeServerVersion**列挙の値と同じになります。  <br/> |
|InternalPop3Connections  <br/> |POP3 プロトコル接続の内部接続設定リスト。  <br/> |
|ExternalPop3Connections  <br/> |POP3 プロトコル接続の外部接続設定リスト。  <br/> |
|InternalImap4Connections  <br/> |IMAP4 プロトコル接続の内部接続設定リスト。  <br/> |
|ExternalImap4Connections  <br/> |IMAP4 プロトコル接続の外部接続設定リスト。  <br/> |
|InternalSmtpConnections  <br/> |SMTP 接続の内部接続設定リスト。  <br/> |
|ExternalSmtpConnections  <br/> |SMTP 接続の外部接続設定リスト。  <br/> |
|InternalServerExclusiveConnect  <br/> |内部サーバーの排他的接続フラグ。 "Off" に設定すると、クライアントはこのプロトコルを使用して接続しません。  <br/> |
|ExternalServerExclusiveConnect  <br/> |外部サーバーの排他的な接続フラグ。 [オン] に設定されている場合、クライアントはこのプロトコルを使用して接続する必要があります。  <br/> |
|ExchangeRpcUrl  <br/> |リモートプロシージャコールに使用する URL。 この URL はサーバー内部で、クライアントが使用するものではありません。  <br/> |
|ShowGalAsDefaultView  <br/> |GAL をアドレス帳として表示するかどうかを示すブール値を指定します。 テキスト値 "true" は、GAL が既定で表示されることを示します。 テキスト値 "false" は、連絡先リストが表示されることを示します。  <br/> |
|AutoDiscoverSMTPAddress  <br/> |ユーザーの自動検出プライマリ SMTP アドレス。 プロキシアドレスが存在する場合は、ユーザーの電子メールアドレスの代わりにプロキシアドレスを入力します。  <br/> |
|InteropExternalEwsUrl  <br/> |サーバーの Web サービスエンドポイントの外部 URL。 これは、Web サービスを持たないサーバーでホストされているメールボックスを処理できるサーバーへの URL です。  <br/> |
|ExternalEwsVersion  <br/> |指定した要求を配信している Web サービスサーバーのバージョン。  <br/> |
|InteropExternalEwsVersion  <br/> |サーバー InteropExternalEwsUrl のバージョンは、を指しています。  <br/> |
|MobileMailboxPolicyInterop  <br/> |モバイルメールボックスポリシーの設定。  <br/> |
|GroupingInformation  <br/> |複数のメールボックスをグループ化して、通知のサブスクライブ時に[類似性を維持](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するために、ExternalEwsUrl の設定と組み合わせて使用される値。  <br/> |
|UserMSOnline  <br/> |ユーザーのメールボックスが、Office 365 の一部として Exchange Online または Exchange Online でホストされているかどうかを示すブール値。  <br/> |
|MapiHttpEnabled  <br/> |MAPI/HTTP プロトコルを使用してユーザーのメールボックスにアクセスできるかどうかを示すブール値。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

