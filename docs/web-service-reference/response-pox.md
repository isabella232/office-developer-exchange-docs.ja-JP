---
title: Response (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 002b72f2-f94d-467c-8e6c-b3818f7e51dc
description: '適用対象:'
ms.openlocfilehash: d613bbb1d8573c1eb60c053ddc064f564676a7c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523483"
---
# <a name="response-pox"></a>Response (POX)


  
**Response 要素** には、自動検出サービスからの応答が含まれる。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
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
|[User (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。 この要素は省略できます。  <br/> |
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AutoDiscover (POX)](autodiscover-pox.md) <br/> |自動検出応答のルート要素。  <br/> |
   
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

