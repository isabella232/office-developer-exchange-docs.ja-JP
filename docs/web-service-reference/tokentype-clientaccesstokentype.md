---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: TokenType 要素は、GetClientAccessToken 応答で返されるクライアントアクセストークンの種類を識別します。
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466053"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

**TokenType**要素は、 **GetClientAccessToken**応答で返されるクライアントアクセストークンの種類を識別します。 
  
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

[Tokenrequest](tokenrequest.md)  | [トークン (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>テキスト値

**Calleridentity**のテキスト値は、呼び出し id クライアントアクセストークンが返されることを意味します。 **Extensioncallback**というテキスト値は、拡張コールバッククライアントアクセストークンが返されることを示します。 **ScopedToken**のテキスト値は、クライアントアクセストークンがスコープ付きのトークンであることを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

