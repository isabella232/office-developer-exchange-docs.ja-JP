---
title: RequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestType
api_type:
- schema
ms.assetid: 4e657e57-528f-4250-a99c-f9850bbbcec5
description: RequestType 要素は、プロキシ要求がクロスサイト要求であるかフォレスト間要求であるかを識別します。
ms.openlocfilehash: 278a65a1f2ce4cb433ae8099703d70d0a2cafa3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455969"
---
# <a name="requesttype"></a>RequestType

**RequestType**要素は、プロキシ要求がクロスサイト要求であるかフォレスト間要求であるかを識別します。 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 **AvailabilityProxyRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

この要素には、スキーマの親がありません。 この要素は、SOAP ヘッダーで使用されます。 この要素の使用方法の詳細については、「WSDL ファイル」を参照してください。
  
## <a name="text-value"></a>テキスト値

この要素にはテキスト値が必要です。 指定可能な値は次のいずれかです。
  
- クロスサイト
    
- クロスフォレスト
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

