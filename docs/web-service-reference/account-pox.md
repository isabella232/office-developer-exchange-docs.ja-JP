---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Account 要素は、ユーザーのアカウント設定を指定するか、エラー応答を含む。
ms.openlocfilehash: 89799ab62a2aa4945b0e8f3209ab1fbc7d2fa2e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534054"
---
# <a name="account-pox"></a>Account (POX)

**Account 要素** は、ユーザーのアカウント設定を指定するか、エラー応答を含む。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |アカウントの種類を表します。  <br/> |
|[Action (POX)](action-pox.md) <br/> |ユーザー構成情報を返す際に別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |ユーザーのメールボックスがユーザーのメールボックスでホストされるかどうかを示す値をExchange Online、Exchange Onlineの一部としてOffice 365。  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |自動検出設定を取得するために使用Exchange Serverクライアント アクセス サーバーの役割がインストールされているコンピューターを実行しているコンピューターの URL が含まれる。  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |後続の自動検出要求に使用する電子メール アドレスを指定します。  <br/> |
|[イメージ (POX)](image-pox.md) <br/> |構成エクスペリエンスのブランド化に使用されるイメージのパスが含まれる。  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |インターネット サービス プロバイダー (ISP) のホーム ページの URL が含まれる。  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをクライアント アクセス サーバーに接続するための仕様が含まれる。  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアントが自動検出要求を送信して、ユーザーのパブリック フォルダー情報を検出するために使用できる情報が含まれる。  <br/> |
|[Error (POX)](error-pox.md) <br/> |自動検出エラー応答が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |自動検出サービスからの応答を格納します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

