---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: DomainName 要素は、ユーザーのドメインを指定します。
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458426"
---
# <a name="domainname-pox"></a>DomainName (POX)

**DomainName**要素は、ユーザーのドメインを指定します。 
  
- [自動検出 (POX)](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md)  
- [アカウント (POX)](account-pox.md) 
- [プロトコル (POX)](protocol-pox.md) 
- [DomainName (POX)](domainname-pox.md)
  
```xml
<DomainName/>
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーのドメインを指定します。
  
## <a name="remarks"></a>注釈

値が指定されていない場合、既定の認証では電子メールアドレスがユーザープリンシパル名 (UPN) 形式として使用されます。 次に例を示します \<Username\> @ \<Domain\> 。
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

