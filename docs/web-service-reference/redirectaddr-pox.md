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
description: RedirectAddr 要素は、後の自動検出要求に使用する電子メール アドレスを指定します。
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833020"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

**RedirectAddr**要素は、後の自動検出要求に使用する電子メール アドレスを指定します。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、後続の自動検出要求に使用する電子メール アドレスを表します。
  
## <a name="remarks"></a>備考

自動検出応答でこの要素がある場合は、 **RedirectAddr**要素のテキスト値を使用して、別の要求を確認します。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

