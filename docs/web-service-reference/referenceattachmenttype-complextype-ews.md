---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: d0e425d5493f9155aff7e16c306a785663f5b89f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522664"
---
# <a name="referenceattachmenttype-complextype-ews"></a>ReferenceAttachmentType complexType (EWS)

## <a name="type-information"></a>型情報

|||
|:-----|:-----|
|**Namespace** <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|**スキーマ ファイル** <br/> |types.xsd  <br/> |
|**拡張ベース** <br/> |t:AttachmentType  <br/> |
   
## <a name="definition"></a>定義

```XML
<xs:complexType name="ReferenceAttachmentType">
    <xs:complexContent>
        <xs:extension base="t:AttachmentType">
            <xs:sequence>
                <xs:element name="AttachLongPathName" type="xs:string" maxOccurs="1" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>

```

## <a name="elements-and-attributes"></a>要素と属性

スキーマで **sequence**、**minOccurs**、**maxOccurs**、**choice** などの具体的な要件が定義されている場合は、定義のセクションを参照してください。 
  
### <a name="child-elements"></a>子要素

|**Element**|**型**|**説明**|
|:-----|:-----|:-----|
|[AttachLongPathName](attachlongpathname.md) <br/> |xs:string  <br/> ||
   
### <a name="attributes"></a>属性

なし。
  

