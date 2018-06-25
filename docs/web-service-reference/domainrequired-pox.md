---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: DomainRequired 要素は、ドメインが認証に必要かどうかを示します。
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760146"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

**DomainRequired**要素は、ドメインが認証に必要かどうかを示します。 
  
- [(POX) を自動検出](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md) 
- [アカウント (POX)](account-pox.md)  
- [プロトコル (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

テキスト値は、ドメインが認証に必要なかどうかを示します。 使用可能な値は、**オン**と**オフを**します。 **** 値がある場合、後続の要求では、ユーザーのアカウントのドメインを含める必要があります。
  
## <a name="remarks"></a>備考

[LoginName (POX)](loginname-pox.md)要素では、ドメインが指定されていない、または**ログイン名が表示**要素が指定されていません、ユーザーは認証が成功する前にドメインを入力する必要があります。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

