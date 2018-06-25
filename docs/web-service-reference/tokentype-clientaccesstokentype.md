---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: TokenType 要素は、GetClientAccessToken の応答で返されるクライアントのアクセス トークンの種類を識別します。
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839725"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

**TokenType**要素は、 **GetClientAccessToken**の応答で返されるクライアントのアクセス トークンの種類を識別します。 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenTypeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[TokenRequest](tokenrequest.md) | [(ClientAccessTokenType) をトークン](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>テキスト値

**CallerIdentity**のテキスト値は、呼び出し元 id のクライアントのアクセス トークンが返されますを意味します。 **ExtensionCallback**のテキスト値は、拡張機能コールバック クライアントのアクセス トークンが返されることを示します。 テキスト値が**ScopedToken**のクライアントのアクセス トークンがスコープのトークンであることを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

