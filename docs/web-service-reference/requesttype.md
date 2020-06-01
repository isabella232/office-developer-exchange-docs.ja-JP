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
# <a name="requesttype"></a><span data-ttu-id="bb5f5-103">RequestType</span><span class="sxs-lookup"><span data-stu-id="bb5f5-103">RequestType</span></span>

<span data-ttu-id="bb5f5-104">**RequestType**要素は、プロキシ要求がクロスサイト要求であるかフォレスト間要求であるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-104">The **RequestType** element identifies whether a proxy request is a cross-site or a cross-forest request.</span></span> 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 <span data-ttu-id="bb5f5-105">**AvailabilityProxyRequestType**</span><span class="sxs-lookup"><span data-stu-id="bb5f5-105">**AvailabilityProxyRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb5f5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bb5f5-106">Attributes and elements</span></span>

<span data-ttu-id="bb5f5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb5f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb5f5-108">Attributes</span></span>

<span data-ttu-id="bb5f5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb5f5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb5f5-110">Child elements</span></span>

<span data-ttu-id="bb5f5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb5f5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bb5f5-112">Parent elements</span></span>

<span data-ttu-id="bb5f5-113">この要素には、スキーマの親がありません。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-113">This element does not have a parent in the schema.</span></span> <span data-ttu-id="bb5f5-114">この要素は、SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-114">This element is used in the SOAP header.</span></span> <span data-ttu-id="bb5f5-115">この要素の使用方法の詳細については、「WSDL ファイル」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-115">For more information about how this element is used, see the WSDL file.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bb5f5-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bb5f5-116">Text value</span></span>

<span data-ttu-id="bb5f5-117">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-117">A text value is required for this element.</span></span> <span data-ttu-id="bb5f5-118">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-118">The following are the possible values:</span></span>
  
- <span data-ttu-id="bb5f5-119">クロスサイト</span><span class="sxs-lookup"><span data-stu-id="bb5f5-119">CrossSite</span></span>
    
- <span data-ttu-id="bb5f5-120">クロスフォレスト</span><span class="sxs-lookup"><span data-stu-id="bb5f5-120">CrossForest</span></span>
    
## <a name="element-information"></a><span data-ttu-id="bb5f5-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bb5f5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb5f5-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb5f5-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb5f5-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb5f5-123">Schema name</span></span>  <br/> |<span data-ttu-id="bb5f5-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="bb5f5-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb5f5-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb5f5-125">Validation file</span></span>  <br/> |<span data-ttu-id="bb5f5-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="bb5f5-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb5f5-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bb5f5-127">Can be empty</span></span>  <br/> |<span data-ttu-id="bb5f5-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="bb5f5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb5f5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb5f5-129">See also</span></span>



- [<span data-ttu-id="bb5f5-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bb5f5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

