---
title: 応答 (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 002b72f2-f94d-467c-8e6c-b3818f7e51dc
description: '適用対象:'
ms.openlocfilehash: 0e8775c895f1b6d674b9a0141d55c64f57d236b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833177"
---
# <a name="response-pox"></a>応答 (POX)


  
**応答**要素には、自動検出サービスからの応答が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
```xml
<Response>
   <User/>
   <Account/>
</Response>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。 この要素はオプションです。  <br/> |
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(POX) を自動検出](autodiscover-pox.md) <br/> |自動検出の応答のルート要素です。  <br/> |
   
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

