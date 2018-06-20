---
title: ドメイン名 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: ドメイン名の要素は、ユーザーのドメインを指定します。
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760150"
---
# <a name="domainname-pox"></a>ドメイン名 (POX)

**ドメイン名**の要素は、ユーザーのドメインを指定します。 
  
- [(POX) を自動検出](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md)  
- [アカウント (POX)](account-pox.md) 
- [プロトコル (POX)](protocol-pox.md) 
- [ドメイン名 (POX)](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーのドメインを指定します。
  
## <a name="remarks"></a>備考

値が指定されていない場合は、ユーザー プリンシパル名 (UPN) 形式で電子メール アドレスを使用する既定の認証。 例:\<ユーザー名\>@\<ドメイン\>。
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

