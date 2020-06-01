---
title: アカウント (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Account 要素は、ユーザーのアカウント設定を指定するか、エラー応答を含みます。
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462319"
---
# <a name="account-pox"></a>アカウント (POX)

**Account**要素は、ユーザーのアカウント設定を指定するか、エラー応答を含みます。 
  
- [自動検出 (POX)](autodiscover-pox.md)
- [応答 (POX)](response-pox.md)
- [アカウント (POX)](account-pox.md)
  
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
|[アクション (POX)](action-pox.md) <br/> |ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。  <br/> |
|[Microsoft Online (POX)](microsoftonline-pox.md) <br/> |ユーザーのメールボックスが、Office 365 の一部として Exchange Online または Exchange Online でホストされているかどうかを示す値を格納します。  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |自動検出設定を取得するために使用する必要がある、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターの URL が含まれています。  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |以降の自動検出要求に使用する電子メールアドレスを指定します。  <br/> |
|[Image (POX)](image-pox.md) <br/> |構成環境をブランド化するために使用されるイメージのパスを含みます。  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |インターネットサービスプロバイダー (ISP) のホームページの URL が含まれています。  <br/> |
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアントが、ユーザーのパブリックフォルダー情報を検出するために自動検出要求を送信するために使用できる情報が含まれています。  <br/> |
|[エラー (POX)](error-pox.md) <br/> |自動検出エラー応答を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[応答 (POX)](response-pox.md) <br/> |自動検出サービスからの応答を含みます。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

