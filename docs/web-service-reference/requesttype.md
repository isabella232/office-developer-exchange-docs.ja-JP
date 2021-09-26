---
title: RequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestType
api_type:
- schema
ms.assetid: 4e657e57-528f-4250-a99c-f9850bbbcec5
description: RequestType 要素は、プロキシ要求がクロスサイト要求かフォレスト間要求かを識別します。
ms.openlocfilehash: 3390381b903c7a39a1d2ea6cae80b3fbc07eba43
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541855"
---
# <a name="requesttype"></a>RequestType

**RequestType** 要素は、プロキシ要求がクロスサイト要求かフォレスト間要求かを識別します。 
  
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

この要素は、スキーマに親を持つ必要があります。 この要素は、SOAP ヘッダーで使用されます。 この要素の使用方法の詳細については、WSDL ファイルを参照してください。
  
## <a name="text-value"></a>テキスト値

この要素には、テキスト値が必要です。 指定可能な値は次のいずれかです。
  
- CrossSite
    
- CrossForest
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

