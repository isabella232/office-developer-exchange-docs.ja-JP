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
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461325"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

**Domainrequired**要素は、ドメインが認証に必要かどうかを示します。 
  
- [自動検出 (POX)](autodiscover-pox.md)  
- [応答 (POX)](response-pox.md) 
- [アカウント (POX)](account-pox.md)  
- [プロトコル (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

Text 値は、ドメインが認証に必要かどうかを示します。 有効な値は、 **[オン**] または [**オフ**] です。 値が**on**の場合、以降の要求にはユーザーのアカウントのドメインが含まれている必要があります。
  
## <a name="remarks"></a>注釈

ドメインが[POX (ログイン)](loginname-pox.md)要素で指定されていない場合、または要素が指定さ**れてい**ない場合は、認証が成功する前に、ユーザーはドメインを入力する必要があります。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

