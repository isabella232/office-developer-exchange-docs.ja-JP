---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: RedirectAddr 要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529876"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

**Redirectaddr**要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、以降の自動検出要求に使用される電子メールアドレスを表します。
  
## <a name="remarks"></a>注釈

この要素が自動検出応答に存在する場合は、 **Redirectaddr**要素のテキスト値を使用して、別の要求を行います。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

