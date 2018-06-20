---
title: 要求 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: 要求要素には、自動検出サービスへの要求が含まれています。
ms.openlocfilehash: ed6b0a80e83e160287f382a881dc5405bfb47a37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833124"
---
# <a name="request-pox"></a>要求 (POX)

**要求**要素には、自動検出サービスへの要求が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[要求 (POX)](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |自動検出応答スキーマを識別します。  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |ユーザーの電子メール アドレスを識別します。  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |従来の識別名によって、ユーザーのメールボックスを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(POX) を自動検出](autodiscover-pox.md) <br/> |自動検出要求のルート要素です。  <br/> |
   
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

