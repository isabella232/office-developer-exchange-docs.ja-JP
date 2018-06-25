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
description: アカウントの要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。
ms.openlocfilehash: 88911aad41816f7cefbffef151e066fe5d4da192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760437"
---
# <a name="account-pox"></a>アカウント (POX)

**アカウント**の要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。 
  
- [(POX) を自動検出](autodiscover-pox.md)
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |アカウントの種類を表します。  <br/> |
|[アクション (POX)](action-pox.md) <br/> |ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Exchange Server を実行しているコンピューターの URL が含まれています。  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |以降の自動検出要求に使用する電子メール アドレスを指定します。  <br/> |
|[イメージ (POX)](image-pox.md) <br/> |構成のエクスペリエンスのブランド化に使用されるイメージのパスが含まれています。  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |インターネット サービス プロバイダー (ISP) のホーム ページの URL が含まれています。  <br/> |
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。  <br/> |
|[エラー (POX)](error-pox.md) <br/> |自動検出エラー応答が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[応答 (POX)](response-pox.md) <br/> |自動検出サービスからの応答が含まれています。  <br/> |
   
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

