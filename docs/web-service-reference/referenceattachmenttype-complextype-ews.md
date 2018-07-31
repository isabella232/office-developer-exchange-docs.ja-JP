---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: c53686ccd032cabcc3f64a3a6684f29afe63a9b1
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354177"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="25722-102">ReferenceAttachmentType complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="25722-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="25722-103">型情報</span><span class="sxs-lookup"><span data-stu-id="25722-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25722-104">**名前空間**</span><span class="sxs-lookup"><span data-stu-id="25722-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25722-105">**スキーマ ファイル**</span><span class="sxs-lookup"><span data-stu-id="25722-105">**Schema file**</span></span> <br/> |<span data-ttu-id="25722-106">types.xsd</span><span class="sxs-lookup"><span data-stu-id="25722-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="25722-107">**拡張ベース**</span><span class="sxs-lookup"><span data-stu-id="25722-107">**Extension base**</span></span> <br/> |<span data-ttu-id="25722-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="25722-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="25722-109">定義</span><span class="sxs-lookup"><span data-stu-id="25722-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="25722-110">要素と属性</span><span class="sxs-lookup"><span data-stu-id="25722-110">Elements and attributes</span></span>

<span data-ttu-id="25722-111">スキーマは、**シーケンス**、 **minOccurs**、 **maxOccurs**では、**選択**などの特定の要件を定義する場合は、定義のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="25722-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="25722-112">子要素</span><span class="sxs-lookup"><span data-stu-id="25722-112">Child elements</span></span>

|<span data-ttu-id="25722-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="25722-113">**Element**</span></span>|<span data-ttu-id="25722-114">**型**</span><span class="sxs-lookup"><span data-stu-id="25722-114">**Type**</span></span>|<span data-ttu-id="25722-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="25722-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="25722-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="25722-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="25722-117">xs:string</span><span class="sxs-lookup"><span data-stu-id="25722-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="25722-118">属性</span><span class="sxs-lookup"><span data-stu-id="25722-118">Attributes</span></span>

<span data-ttu-id="25722-119">なし。</span><span class="sxs-lookup"><span data-stu-id="25722-119">None.</span></span>
  

