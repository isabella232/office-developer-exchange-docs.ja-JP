---
title: Protocol (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: Protocol 要素には、クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Exchange Server接続するための仕様が含まれている。
ms.openlocfilehash: 4f308951c74612936755e6d4c16620e38277aecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516399"
---
# <a name="protocol-pox"></a>Protocol (POX)

**Protocol 要素** には、クライアント アクセス サーバーの役割がインストールされているExchange Serverコンピューターにクライアントを接続するための仕様が含まれている。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
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
|種類  <br/> |この Protocol 要素で記述されるプロトコルの種類 **を示** します。 この属性の有効な値は"mapiHttp"のみです。 この属性は、この応答に対応する自動検出要求に [X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ存在します。 この属性は、ビルド 15.00.0847.032 (Exchange Server 2013 SP1) から、MAPI/HTTP プロトコルとターゲット Exchange Online、Exchange Online を Office 365 の一部として実装するクライアント、または Exchange のオンプレミス バージョンに適用されます。  <br/> |
|バージョン  <br/> |この Protocol 要素で説明されているプロトコルのバージョンを **示** します。 この属性の有効な値は "1" のみです。 この属性は、この応答に対応する自動検出要求に **X-MapiHttpCapability ヘッダーが含まれている場合にのみ存在** します。 この属性は、ビルド 15.00.0847.032 (Exchange Server 2013 SP1) から、MAPI/HTTP プロトコルとターゲット Exchange Online、Exchange Online を Office 365 の一部として実装するクライアント、または Exchange のオンプレミス バージョンに適用されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |構成済みのメール アカウントの種類を識別します。  <br/> |
|[内部 (POX)](internal-pox.md) <br/> |クライアントが組織のネットワーク内からユーザーに接続するために使用Exchange URL のコレクションを格納します。  <br/> |
|[External (POX)](external-pox.md) <br/> |クライアントが組織のネットワークの外部からExchangeに使用できる URL のコレクションを格納します。  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |設定が有効な状態を維持する時間 (時間) を指定します。  <br/> |
|[Server (POX)](server-pox.md) <br/> |メール サーバーの名前を指定します。  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |識別名Exchange Server指定します。  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |バージョン番号のExchange Serverを表します。  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |メールボックス データベースの識別名を表します。  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |ユーザーのパブリック フォルダー サーバーの完全修飾ドメイン名 (FQDN) が含まれる。  <br/> |
|[Port (POX)](port-pox.md) <br/> |ストアへの接続に使用するポートを指定します。  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Name Service Provider Interface (NSPI) プロトコルを使用する場合にディレクトリへの接続に使用するポートを指定します。  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |ディレクトリへの参照を取得するために使用するポートを指定します。  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |メールが有効なユーザーの Web サービスに最適Exchangeインスタンスの URL を指定します。  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |メールが有効なユーザーの Web サービス (EWS) にExchangeエンドポイント インスタンスの URL を指定します。  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |メールが有効なユーザーの Web サービス (EWS) にExchangeエンドポイント インスタンスの URL を指定します。  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |予定表と連絡先の組織間共有に使用される共有サーバーの URL を格納します。  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |メールが有効なユーザー Exchangeコントロール パネルの URL を指定します。  <br/> |
|[EcpUrl-um (POX)](ecpurl-um-pox.md) <br/> |メールが有効なユーザーのボイス メール設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |メールが有効なユーザーの電子メール集約設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |メールが有効なユーザーの電子メール メッセージ追跡設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |メールが有効なユーザーの保持タグ設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |メールが有効なユーザーのショート メッセージ サービス (SMS) 設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-publish (POX)](ecpurl-publish-pox.md) <br/> |メールが有効なユーザーの予定表発行設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |メールが有効なユーザーの現在の写真を表示または変更するために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |メールが有効なユーザーが現在メンバーになっているすべてのサイト メールボックスのリストにアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせ可能な部分 URL を指定します。  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、新しいサイト メールボックスの作成に使用できる URL を生成できる部分 URL を指定します。  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、サイト メールボックスからユーザーの登録を解除するために使用できる URL を生成できる部分的な URL を指定します。  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイト メールボックスの編集に使用できる URL を生成できる部分 URL を指定します。  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーのメールボックスに現在インストールされているメール アプリを表示または変更するために使用できる URL を生成できる部分的な URL を指定します。  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |メールが有効なユーザーの可用性サービスの最適なインスタンスの URL を指定します。  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |オフライン トポロジのオフライン アドレス帳構成サーバーの URL をExchangeします。  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |メールが有効なユーザーのユニファイド メッセージング Web サービスの最適なインスタンスの URL を指定します。  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |メールが有効なユーザーの Web サービス (EWS) にExchangeエンドポイント インスタンスの URL を指定します。  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |ユーザーのログオン名を指定します。  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |ドメインが認証に必要かどうかを示します。  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |ユーザーのドメインを指定します。  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |セキュリティで保護されたパスワード認証が必要かどうかを示します。  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |メールボックス サーバーの役割がインストールされている 2007 Exchangeに対して認証するときに使用する認証スキームを指定します。  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |SSL を使用Secure Sockets Layer Microsoft 組織に接続するために必要な証明書 (SSL) Exchangeを指定します。  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |セキュリティで保護されたログオンが必要かどうかを指定します。  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |認証が必要かどうかを指定します。  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |POP3 タイプのアカウントに提供される認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |SMTP サーバーを使用して電子メールを送信する前に、電子メールをダウンロードする必要があるかどうかを指定します。  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |クライアント コンピューターがインターネット サービス プロバイダーのサーバーへの接続要件を満たすネットワーク上にあるかどうかを判断するために使用される条件が含まれます。  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをアドレス帳サーバーに接続するための仕様が含まれる。 この要素は **、Protocol** 要素の Type属性が存在し、"mapiHttp" に設定されている場合にのみ存在します。 **AddressBook** 要素は、MAPI/HTTP プロトコルを実装し、Exchange Online および Exchange のバージョンを 15.00.0847.032 から実装するクライアントに適用できます。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれる。 この要素は **、Protocol** 要素の Type属性が存在し、"mapiHttp" に設定されている場合にのみ存在します。 **MailStore** 要素は、MAPI/HTTP プロトコルを実装し、Exchange Online および Exchange のバージョンを 15.00.0847.032 から実装するクライアントに適用できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

**Protocol 要素** は、設定と等しいアクション [(POX)](action-pox.md)値を持つ応答に存在 **します**。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

