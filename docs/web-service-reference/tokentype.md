---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: TokenType 要素は、トークンの種類を指定します。
ms.openlocfilehash: a51ddfdd097a94370168077b9eca8be2e0581603
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523322"
---
# <a name="tokentype"></a>TokenType

**TokenType 要素** は、トークンの種類を指定します。 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[TokenRequest](tokenrequest.md)  | [トークン](token.md)
  
## <a name="text-value"></a>テキスト値

TokenType 要素の **テキスト値** は、トークンの種類です。 **CallerIdentity のテキスト値は**、トークンが発信者 ID トークンを示します。 **ExtensionCallback のテキスト値は**、トークンが拡張コールバック用の値を示します。 **ScopedToken のテキスト値は**、クライアント アクセス トークンがスコープ 付きトークンを示します。 
  
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
   

