---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: 24f5a62eadd490b5b0000dfe048850c44540f266
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528735"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="d1c80-102">ReferenceAttachmentType complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="d1c80-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="d1c80-103">型情報</span><span class="sxs-lookup"><span data-stu-id="d1c80-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1c80-104">**Namespace**</span><span class="sxs-lookup"><span data-stu-id="d1c80-104">**Namespace**</span></span> <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1c80-105">**スキーマ ファイル**</span><span class="sxs-lookup"><span data-stu-id="d1c80-105">**Schema file**</span></span> <br/> |<span data-ttu-id="d1c80-106">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d1c80-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1c80-107">**拡張ベース**</span><span class="sxs-lookup"><span data-stu-id="d1c80-107">**Extension base**</span></span> <br/> |<span data-ttu-id="d1c80-108">\ Attachmenttype</span><span class="sxs-lookup"><span data-stu-id="d1c80-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="d1c80-109">定義</span><span class="sxs-lookup"><span data-stu-id="d1c80-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="d1c80-110">要素と属性</span><span class="sxs-lookup"><span data-stu-id="d1c80-110">Elements and attributes</span></span>

<span data-ttu-id="d1c80-111">スキーマで **sequence**、**minOccurs**、**maxOccurs**、**choice** などの具体的な要件が定義されている場合は、定義のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1c80-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="d1c80-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d1c80-112">Child elements</span></span>

|<span data-ttu-id="d1c80-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="d1c80-113">**Element**</span></span>|<span data-ttu-id="d1c80-114">**型**</span><span class="sxs-lookup"><span data-stu-id="d1c80-114">**Type**</span></span>|<span data-ttu-id="d1c80-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1c80-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="d1c80-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="d1c80-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="d1c80-117">xs: 文字列</span><span class="sxs-lookup"><span data-stu-id="d1c80-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="d1c80-118">属性</span><span class="sxs-lookup"><span data-stu-id="d1c80-118">Attributes</span></span>

<span data-ttu-id="d1c80-119">なし。</span><span class="sxs-lookup"><span data-stu-id="d1c80-119">None.</span></span>
  

