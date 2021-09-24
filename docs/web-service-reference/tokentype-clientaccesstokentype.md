---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: TokenType 要素は、GetClientAccessToken 応答で返されるクライアント アクセス トークンの種類を識別します。
ms.openlocfilehash: 967d64796799147876ef6443b40b16154b55c01a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523357"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

**TokenType** 要素は **、GetClientAccessToken** 応答で返されるクライアント アクセス トークンの種類を識別します。 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[TokenRequest](tokenrequest.md)  | [トークン (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>テキスト値

**CallerIdentity のテキスト値は、** 発信者 ID クライアント アクセス トークンが返されます。 **ExtensionCallback のテキスト値は**、拡張コールバック クライアント アクセス トークンが返されます。 **ScopedToken** のテキスト値は、クライアント アクセス トークンがスコープ 付きトークンを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

