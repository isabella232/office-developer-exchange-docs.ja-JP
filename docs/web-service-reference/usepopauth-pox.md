---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: UsePOPAuth 要素は、POP3 タイプのアカウントに提供される認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。
ms.openlocfilehash: 354c027bf40ddf30cda472eb4ca0d018dca64f9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542625"
---
# <a name="usepopauth-pox"></a>UsePOPAuth (POX)

**UsePOPAuth** 要素は、POP3 タイプのアカウントに提供される認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[UsePOPAuth (POX)](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている 2007 年Microsoft Exchange Serverコンピューターにクライアントを接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、POP3 タイプのアカウントに提供される認証情報が SMTP にも使用されるかどうかを示します。 指定できる値は **オンと** オフ **です**。
  
## <a name="remarks"></a>注釈

**UsePOPAuth 要素** は、Type [(POX) が SMTP の場合](type-pox.md)にのみ使用されます。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

