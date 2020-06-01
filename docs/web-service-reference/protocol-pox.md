---
title: プロトコル (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: Protocol 要素には、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: 6fca347f49e27958ecb16cce345387b6a2146979
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467761"
---
# <a name="protocol-pox"></a>プロトコル (POX)

**Protocol**要素には、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
```xml
<Protocol>
   <Type/>
   <Internal/>
   <External/>
   <TTL/>
   <Server/>
   <ServerDN/>
   <ServerVersion/>
   <MdbDN/>
   <PublicFolderServer/>
   <Port/>
   <DirectoryPort/>
   <ReferralPort/>
   <ASUrl/>
   <EwsUrl/>
   <EmwsUrl/>
   <SharingUrl/>
   <EcpUrl/>
   <EcpUrl-um/>
   <EcpUrl-aggr/>
   <EcpUrl-mt/>
   <EcpUrl-ret/>
   <EcpUrl-sms/>
   <EcpUrl-publish/>
   <EcpUrl-photo/>
   <EcpUrl-tm/>
   <EcpUrl-tmCreating/>
   <EcpUrl-tmHiding/>
   <EcpUrl-tmEditing/>
   <EcpUrl-extinstall/>
   <OOFUrl/>
   <OABUrl/>
   <UMUrl/>
   <EwsPartnerUrl/>
   <LoginName/>
   <DomainRequired/>
   <DomainName/>
   <SPA/>
   <AuthPackage/>
   <CertPrincipalName/>
   <SSL/>
   <AuthRequired/>
   <UsePOPAuth/>
   <SMTPLast/>
   <NetworkRequirements/>
   <AddressBook/>
   <MailStore/>
</Protocol>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|種類  <br/> |この**プロトコル**要素で記述されているプロトコルの種類を示します。 この属性の有効な値は "Http" だけです。 この属性は、この応答に対応する自動検出要求に[MapiHttpCapability ヘッダーが含まれて](pox-autodiscover-request-for-exchange.md)いた場合にのみ存在します。 この属性は、MAPI/HTTP プロトコルおよびターゲット Exchange Online の一部としての Exchange Online、Office 365 の一部としての Exchange Online、または、build 15.00.0847.032 (Exchange Server 2013 SP1) 以降の Exchange のオンプレミスバージョンを実装するクライアントに適用されます。  <br/> |
|バージョン  <br/> |この**プロトコル**要素で記述されているプロトコルのバージョンを示します。 この属性の有効な値は "1" だけです。 この属性は、この応答に対応する自動検出要求に**MapiHttpCapability**ヘッダーが含まれていた場合にのみ存在します。 この属性は、MAPI/HTTP プロトコルおよびターゲット Exchange Online の一部としての Exchange Online、Office 365 の一部としての Exchange Online、または、build 15.00.0847.032 (Exchange Server 2013 SP1) 以降の Exchange のオンプレミスバージョンを実装するクライアントに適用されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[種類 (POX)](type-pox.md) <br/> |構成されているメールアカウントの種類を識別します。  <br/> |
|[Internal (POX)](internal-pox.md) <br/> |組織のネットワーク内から Exchange に接続するためにクライアントが使用できる Url のコレクションが含まれています。  <br/> |
|[外部 (POX)](external-pox.md) <br/> |組織のネットワーク外から Exchange に接続するためにクライアントが使用できる Url のコレクションが含まれています。  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |設定が有効なままになる時間を時間単位で指定します。  <br/> |
|[サーバー (POX)](server-pox.md) <br/> |メールサーバーの名前を指定します。  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Exchange サーバーの識別名を指定します。  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Exchange サーバーのバージョン番号を表します。  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |メールボックスデータベースの識別名を表します。  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |ユーザーのパブリックフォルダーサーバーの完全修飾ドメイン名 (FQDN) が含まれています。  <br/> |
|[ポート (POX)](port-pox.md) <br/> |ストアへの接続に使用するポートを指定します。  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用するポートを指定します。  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |ディレクトリへの参照を取得するために使用されるポートを指定します。  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |メールが有効なユーザーの Exchange Web サービスの最適なインスタンスの URL を指定します。  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |予定表と連絡先を組織間で共有するために使用される共有サーバーの URL が含まれています。  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |メールが有効なユーザーの Exchange コントロールパネルの URL を指定します。  <br/> |
|[EcpUrl (POX)](ecpurl-um-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのボイスメール設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メール集計の設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メールメッセージ追跡設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの保持タグの設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのショートメッセージサービス (SMS) の設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl (POX)](ecpurl-publish-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの予定表の発行設定にアクセスするために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl (POX)](ecpurl-photo-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの現在の写真を表示または変更するために使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |メールが有効なユーザーが現在メンバーであるすべてのサイトメールボックスのリストにアクセスするために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて指定できる url の一部を指定します。  <br/> |
|[EcpUrl-tmCreating 作成 (POX)](ecpurl-tmcreating-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、新しいサイトメールボックスの作成に使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-tmHiding 表示 (POX)](ecpurl-tmhiding-pox.md) <br/> |サイトメールボックスからのユーザーの登録を解除するために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できる url の部分を指定します。  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイトメールボックスの編集に使用できる url を生成できる url の部分を指定します。  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |ユーザーのメールボックスに現在インストールされているメールアプリを表示または変更するために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できる url の部分を指定します。  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |メールが有効なユーザーの空き時間情報サービスの最適なインスタンスの URL を指定します。  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Exchange トポロジのオフラインアドレス帳構成サーバーの URL を指定します。  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |メールが有効なユーザーに対して、ユニファイドメッセージング Web サービスの最適なインスタンスの URL を指定します。  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。  <br/> |
|[ログイン (POX)](loginname-pox.md) <br/> |ユーザーのログオン名を指定します。  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |ドメインが認証に必要かどうかを示します。  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |ユーザーのドメインを指定します。  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |セキュリティで保護されたパスワード認証が必要かどうかを示します。  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |メールボックスサーバーの役割がインストールされている Exchange 2007 コンピューターに対して認証を行うときに使用する認証方式を指定します。  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL (Secure Sockets Layer) 証明書プリンシパル名を指定します。  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |セキュリティで保護されたログオンが必要かどうかを指定します。  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |認証が必要かどうかを指定します。  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |POP3 の種類のアカウントに対して提供された認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Smtp サーバーを使用して電子メールを送信する前に、SMTP サーバーで電子メールをダウンロードする必要があるかどうかを指定します。  <br/> |
|[NetworkRequirements 要件 (POX)](networkrequirements-pox.md) <br/> |サーバーに接続するためのインターネットサービスプロバイダーの要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |MAPI/HTTP プロトコルを使用して、アドレス帳サーバーにクライアントを接続するための仕様が含まれています。 この要素は、 **Protocol**要素の**Type**属性が存在し、"http" に設定されている場合にのみ存在します。 **AddressBook**要素は、MAPI/HTTP プロトコルと、ターゲットの exchange Online と、15.00.0847.032 以降のバージョンの exchange を実装するクライアントに適用されます。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。 この要素は、 **Protocol**要素の**Type**属性が存在し、"http" に設定されている場合にのみ存在します。 **Mailstore**要素は、MAPI/HTTP プロトコルと、15.00.0847.032 から始まる exchange のバージョンを実装するクライアントに適用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

**Protocol**要素は、**設定**と同じ[処理 (POX)](action-pox.md)値を持つ応答内に存在します。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

