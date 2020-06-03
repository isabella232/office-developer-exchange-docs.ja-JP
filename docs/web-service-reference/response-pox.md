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
ms.openlocfilehash: 30f6a5c2c6e3034fde8849ab1fced3519029b1f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448976"
---
# <a name="response-pox"></a>応答 (POX)


  
**Response**要素には、自動検出サービスからの応答が含まれます。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
```xml
<Response>
   <User/>
   <Account/>
</Response>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。 この要素は省略できます。  <br/> |
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[自動検出 (POX)](autodiscover-pox.md) <br/> |自動検出応答のルート要素。  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

