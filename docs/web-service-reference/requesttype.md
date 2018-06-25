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
# <a name="requesttype"></a><span data-ttu-id="68ff6-103">修飾子の一覧</span><span class="sxs-lookup"><span data-stu-id="68ff6-103">RequestType</span></span>

<span data-ttu-id="68ff6-104">**RequestType**要素では、プロキシ要求がサイト間またはフォレスト間の要求であるかどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="68ff6-104">The **RequestType** element identifies whether a proxy request is a cross-site or a cross-forest request.</span></span> 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 <span data-ttu-id="68ff6-105">**AvailabilityProxyRequestType**</span><span class="sxs-lookup"><span data-stu-id="68ff6-105">**AvailabilityProxyRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68ff6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="68ff6-106">Attributes and elements</span></span>

<span data-ttu-id="68ff6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="68ff6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68ff6-108">属性</span><span class="sxs-lookup"><span data-stu-id="68ff6-108">Attributes</span></span>

<span data-ttu-id="68ff6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="68ff6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68ff6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="68ff6-110">Child elements</span></span>

<span data-ttu-id="68ff6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="68ff6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="68ff6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="68ff6-112">Parent elements</span></span>

<span data-ttu-id="68ff6-113">この要素には、スキーマ内の親がありません。</span><span class="sxs-lookup"><span data-stu-id="68ff6-113">This element does not have a parent in the schema.</span></span> <span data-ttu-id="68ff6-114">この要素は、SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="68ff6-114">This element is used in the SOAP header.</span></span> <span data-ttu-id="68ff6-115">この要素の使用方法の詳細については、WSDL ファイルを参照してください。</span><span class="sxs-lookup"><span data-stu-id="68ff6-115">For more information about how this element is used, see the WSDL file.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="68ff6-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="68ff6-116">Text value</span></span>

<span data-ttu-id="68ff6-117">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="68ff6-117">A text value is required for this element.</span></span> <span data-ttu-id="68ff6-118">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="68ff6-118">The following are the possible values:</span></span>
  
- <span data-ttu-id="68ff6-119">CrossSite</span><span class="sxs-lookup"><span data-stu-id="68ff6-119">CrossSite</span></span>
    
- <span data-ttu-id="68ff6-120">CrossForest</span><span class="sxs-lookup"><span data-stu-id="68ff6-120">CrossForest</span></span>
    
## <a name="element-information"></a><span data-ttu-id="68ff6-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="68ff6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68ff6-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="68ff6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68ff6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="68ff6-123">Schema name</span></span>  <br/> |<span data-ttu-id="68ff6-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="68ff6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="68ff6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="68ff6-125">Validation file</span></span>  <br/> |<span data-ttu-id="68ff6-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="68ff6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="68ff6-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="68ff6-127">Can be empty</span></span>  <br/> |<span data-ttu-id="68ff6-128">False</span><span class="sxs-lookup"><span data-stu-id="68ff6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68ff6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="68ff6-129">See also</span></span>



- [<span data-ttu-id="68ff6-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="68ff6-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

