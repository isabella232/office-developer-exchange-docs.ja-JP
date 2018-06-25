---
title: UniquePathId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniquePathId
api_type:
- schema
ms.assetid: 3c917100-907a-4aa1-a7d4-01c65f9a42e4
description: UniquePathId 要素は、追跡レポートのパスごとに異なる文字列を表します。
ms.openlocfilehash: db238c6ebbe25d4089465f43df6bac79007bc952
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839805"
---
# <a name="uniquepathid"></a><span data-ttu-id="dd355-103">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="dd355-103">UniquePathId</span></span>

<span data-ttu-id="dd355-104">**UniquePathId**要素は、追跡レポートのパスごとに異なる文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="dd355-104">The **UniquePathId** element represents a string that is different for each path in a tracking report.</span></span> 
  
```XML
<UniquePathId/>
```

 <span data-ttu-id="dd355-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="dd355-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd355-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd355-106">Attributes and elements</span></span>

<span data-ttu-id="dd355-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd355-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd355-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd355-108">Attributes</span></span>

<span data-ttu-id="dd355-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd355-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd355-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd355-110">Child elements</span></span>

<span data-ttu-id="dd355-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dd355-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd355-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd355-112">Parent elements</span></span>

|<span data-ttu-id="dd355-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd355-113">**Element**</span></span>|<span data-ttu-id="dd355-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd355-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd355-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="dd355-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="dd355-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd355-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd355-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dd355-117">Text value</span></span>

<span data-ttu-id="dd355-118">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="dd355-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd355-119">備考</span><span class="sxs-lookup"><span data-stu-id="dd355-119">Remarks</span></span>

<span data-ttu-id="dd355-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dd355-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd355-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd355-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd355-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd355-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd355-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd355-123">Schema Name</span></span>  <br/> |<span data-ttu-id="dd355-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dd355-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd355-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd355-125">Validation File</span></span>  <br/> |<span data-ttu-id="dd355-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd355-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd355-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dd355-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd355-128">False</span><span class="sxs-lookup"><span data-stu-id="dd355-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd355-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd355-129">See also</span></span>



- [<span data-ttu-id="dd355-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd355-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

