---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: BlockStatus 要素は、項目のブロックの状態を指定します。
ms.openlocfilehash: 5733738d733578c47b849b9d7c62c9b66cd8922e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759515"
---
# <a name="blockstatus"></a><span data-ttu-id="c817e-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="c817e-103">BlockStatus</span></span>

<span data-ttu-id="c817e-104">**BlockStatus**要素は、項目のブロックの状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="c817e-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="c817e-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c817e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c817e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c817e-106">Attributes and elements</span></span>

<span data-ttu-id="c817e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c817e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c817e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c817e-108">Attributes</span></span>

<span data-ttu-id="c817e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c817e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c817e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c817e-110">Child elements</span></span>

<span data-ttu-id="c817e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c817e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c817e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c817e-112">Parent elements</span></span>

|<span data-ttu-id="c817e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c817e-113">**Element**</span></span>|<span data-ttu-id="c817e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c817e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c817e-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c817e-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c817e-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c817e-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c817e-117">Contact</span><span class="sxs-lookup"><span data-stu-id="c817e-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c817e-118">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c817e-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c817e-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c817e-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c817e-120">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c817e-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c817e-121">アイテム</span><span class="sxs-lookup"><span data-stu-id="c817e-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="c817e-122">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="c817e-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c817e-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c817e-123">Text value</span></span>

<span data-ttu-id="c817e-124">の**場合は true** 、 **BlockStatus**要素のテキスト値は、項目がブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="c817e-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="c817e-125">**False**の値は、項目がブロックされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c817e-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c817e-126">備考</span><span class="sxs-lookup"><span data-stu-id="c817e-126">Remarks</span></span>

<span data-ttu-id="c817e-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c817e-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c817e-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c817e-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c817e-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="c817e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c817e-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="c817e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c817e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c817e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c817e-132">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="c817e-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="c817e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c817e-133">Validation File</span></span>  <br/> |<span data-ttu-id="c817e-134">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c817e-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c817e-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c817e-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c817e-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="c817e-136">See also</span></span>



- [<span data-ttu-id="c817e-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c817e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

