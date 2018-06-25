---
title: 修飾子の一覧
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
description: RequestType 要素では、プロキシ要求がサイト間またはフォレスト間の要求であるかどうかを識別します。
ms.openlocfilehash: 96a4d57432b15aa54fff2618df458fc75cb227f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833139"
---
# <a name="requesttype"></a>修飾子の一覧

**RequestType**要素では、プロキシ要求がサイト間またはフォレスト間の要求であるかどうかを識別します。 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 **AvailabilityProxyRequestType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

この要素には、スキーマ内の親がありません。 この要素は、SOAP ヘッダーで使用されます。 この要素の使用方法の詳細については、WSDL ファイルを参照してください。
  
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の必要があります。 指定可能な値は次のいずれかです。
  
- CrossSite
    
- CrossForest
    
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

