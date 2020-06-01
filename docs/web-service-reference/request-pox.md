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
description: Request 要素には、自動検出サービスへの要求が含まれています。
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459547"
---
# <a name="request-pox"></a>要求 (POX)

**Request**要素には、自動検出サービスへの要求が含まれています。 
  
- [自動検出 (POX)](autodiscover-pox.md) 
- [要求 (POX)](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |自動検出応答のスキーマを識別します。  <br/> |
|[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md) <br/> |ユーザーの電子メールアドレスを識別します。  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |従来の識別名でユーザーのメールボックスを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[自動検出 (POX)](autodiscover-pox.md) <br/> |自動検出要求のルート要素。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

