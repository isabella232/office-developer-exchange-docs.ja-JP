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
description: プロトコル要素には、クライアント アクセス サーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: e58ae82ea5ec9d39db0f9219f6019df7da24a343
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832926"
---
# <a name="protocol-pox"></a>プロトコル (POX)

**プロトコル**要素には、クライアント アクセス サーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|種類  <br/> |この**プロトコル**要素で記述されたプロトコルの種類を示します。 この属性の唯一の有効値は、"mapiHttp"です。 この属性は、唯一の現在の自動検出を要求する場合に対応するこの応答は[、X-MapiHttpCapability ヘッダーが含まれています](pox-autodiscover-request-for-exchange.md)。 この属性は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに適用または設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。  <br/> |
|バージョン  <br/> |この**プロトコル**要素で記述されたプロトコルのバージョンを示します。 この属性の唯一の有効値は、「1」です。 この属性は、この応答に対応する自動検出要求には、 **X-MapiHttpCapability**ヘッダーが含まれている場合のみです。 この属性は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに適用または設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[(POX) の種類](type-pox.md) <br/> |設定したメール アカウントの種類を識別します。  <br/> |
|[内部 (POX)](internal-pox.md) <br/> |組織のネットワーク内から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。  <br/> |
|[外部 (POX)](external-pox.md) <br/> |組織のネットワーク外部から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |時間、期間の設定が有効なままで、Live までの時間を指定します。  <br/> |
|[サーバー (POX)](server-pox.md) <br/> |メール サーバーの名前を指定します。  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Exchange Server の識別名を指定します。  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Exchange Server のバージョン番号を表します。  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |メールボックス データベースの識別名を表します。  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |ユーザーのパブリック フォルダー サーバーの完全修飾ドメイン名 (FQDN) が含まれています。  <br/> |
|[ポート (POX)](port-pox.md) <br/> |ストアへの接続に使用されるポートを指定します。  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |ネーム サービス プロバイダー インターフェイス (NSPI) プロトコルを使用すると、ディレクトリへの接続に使用されるポートを指定します。  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |ディレクトリへの参照を取得するために使用されるポートを指定します。  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |メールが有効なユーザーの Exchange Web サービスの最適なインスタンスの URL を指定します。  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |組織間の予定表と連絡先の共有に使用する共有サーバーの URL が含まれています。  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |メールが有効なユーザーの Exchange コントロール パネルの URL を指定します。  <br/> |
|[EcpUrl-um (POX)](ecpurl-um-pox.md) <br/> |メールが有効なユーザーのボイス メールの設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |メールが有効なユーザーの e メールの集計の設定へのアクセスに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |メールが有効なユーザーの設定を追跡する電子メール メッセージにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |メールが有効なユーザーの保持タグの設定にアクセスするために使用する URL を生成するのには[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl sms (POX)](ecpurl-sms-pox.md) <br/> |メールが有効なユーザーのショート メッセージ サービス (SMS) の設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[(POX) を EcpUrl 発行](ecpurl-publish-pox.md) <br/> |メールが有効なユーザーの予定表の公開設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[(POX) の EcpUrl の写真](ecpurl-photo-pox.md) <br/> |表示またはメールが有効なユーザーの現在の写真を変更するために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |先のすべてのサイトのメールボックスのメールが有効なユーザーは、現在メンバー リストにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |サイトの新しいメールボックスを作成するのに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |サイトのメールボックスからユーザーの購読を解除するために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |サイトの既存のメールボックスの編集に使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |表示または変更するユーザーのメールボックスに現在インストールされているメール ・ アプリケーションに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |メールが有効なユーザーの可用性サービスの最適なインスタンスの URL を指定します。  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Exchange トポロジの場合、オフライン アドレス帳の構成サーバーの URL を指定します。  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |メールが有効なユーザーのユニファイド メッセージングの Web サービスの最適なインスタンスの URL を指定します。  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |ユーザーのログオン名を指定します。  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |ドメインが認証に必要かどうかを示します。  <br/> |
|[ドメイン名 (POX)](domainname-pox.md) <br/> |ユーザーのドメインを指定します。  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |セキュリティで保護されたパスワード認証が必要かどうかを示します。  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |メールボックス サーバーの役割がインストールされている Exchange 2007 コンピューターに対して認証するときに使用される認証スキームを指定します。  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |SSL を使用して Microsoft Exchange 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |セキュリティで保護されたログオンが必要かどうかを指定します。  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |認証が必要かどうかを指定します。  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |POP3 アカウントの種類の指定された認証情報は、簡易メール転送プロトコル (SMTP) を使用してもかどうかを示します。  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |SMTP サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |使用してクライアント コンピューターがネットワーク サーバーに接続するインターネット サービス プロバイダーの要件を満たしているかどうかを決定する基準が含まれています。  <br/> |
|[アドレス帳 (POX)](addressbook-pox.md) <br/> |MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。 **プロトコル**要素の**Type**属性が存在し、設定の場合でこの要素があるだけに"mapiHttp"です。 **アドレス帳**の要素は、MAPI または HTTP プロトコルと Exchange Online のターゲットと 15.00.0847.032 以降の Exchange のバージョンを実装するクライアントに適用されます。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。 **プロトコル**要素の**Type**属性が存在し、設定の場合でこの要素があるだけに"mapiHttp"です。 **MailStore**要素は、MAPI または HTTP プロトコルと Exchange Online のターゲットと 15.00.0847.032 以降の Exchange のバージョンを実装するクライアントに適用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
## <a name="remarks"></a>備考

**プロトコル**要素は、**設定**と同じである[アクション (POX)](action-pox.md)の値を持つ応答に存在します。
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

