---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: da9ff2b73f86bba3003c31dec009ea11a9b26b32
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833030"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="05525-102">ReferenceAttachmentType complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="05525-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="05525-103">型情報</span><span class="sxs-lookup"><span data-stu-id="05525-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05525-104">**名前空間**</span><span class="sxs-lookup"><span data-stu-id="05525-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05525-105">**スキーマ ファイル**</span><span class="sxs-lookup"><span data-stu-id="05525-105">**Schema file**</span></span> <br/> |<span data-ttu-id="05525-106">types.xsd</span><span class="sxs-lookup"><span data-stu-id="05525-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="05525-107">**拡張機能の基本**</span><span class="sxs-lookup"><span data-stu-id="05525-107">**Extension base**</span></span> <br/> |<span data-ttu-id="05525-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="05525-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="05525-109">定義</span><span class="sxs-lookup"><span data-stu-id="05525-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="05525-110">要素と属性</span><span class="sxs-lookup"><span data-stu-id="05525-110">Elements and attributes</span></span>

<span data-ttu-id="05525-111">スキーマは、**シーケンス**、 **minOccurs**、 **maxOccurs**では、**選択**などの特定の要件を定義する場合は、定義のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="05525-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="05525-112">子要素</span><span class="sxs-lookup"><span data-stu-id="05525-112">Child elements</span></span>

|<span data-ttu-id="05525-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="05525-113">**Element**</span></span>|<span data-ttu-id="05525-114">**型**</span><span class="sxs-lookup"><span data-stu-id="05525-114">**Type**</span></span>|<span data-ttu-id="05525-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="05525-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="05525-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="05525-116">AttachLongPathName</span></span>](http://msdn.microsoft.com/library/98464422-2c13-8d33-0fe3-b1978f2d5b4a%28Office.15%29.aspx) <br/> |<span data-ttu-id="05525-117">xs:string</span><span class="sxs-lookup"><span data-stu-id="05525-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="05525-118">属性</span><span class="sxs-lookup"><span data-stu-id="05525-118">Attributes</span></span>

<span data-ttu-id="05525-119">なし。</span><span class="sxs-lookup"><span data-stu-id="05525-119">None.</span></span>
  

