---
title: IntendedFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IntendedFreeBusyStatus
api_type:
- schema
ms.assetid: 0e0fa898-69a4-4c57-8bb2-52f716b5b478
description: IntendedFreeBusyStatus 要素は、会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。
ms.openlocfilehash: 3254becf8c6885f7d6dc401ecf31da149e7de2d4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831945"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="bd79f-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="bd79f-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="bd79f-104">**IntendedFreeBusyStatus**要素は、会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="bd79f-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="bd79f-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="bd79f-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd79f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bd79f-106">Attributes and elements</span></span>

<span data-ttu-id="bd79f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd79f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd79f-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd79f-108">Attributes</span></span>

<span data-ttu-id="bd79f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd79f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd79f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd79f-110">Child elements</span></span>

<span data-ttu-id="bd79f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bd79f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd79f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bd79f-112">Parent elements</span></span>

|<span data-ttu-id="bd79f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bd79f-113">**Element**</span></span>|<span data-ttu-id="bd79f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd79f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd79f-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="bd79f-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="bd79f-116">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="bd79f-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd79f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bd79f-117">Text value</span></span>

<span data-ttu-id="bd79f-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="bd79f-118">A text value is required.</span></span> <span data-ttu-id="bd79f-119">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="bd79f-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="bd79f-120">Free</span><span class="sxs-lookup"><span data-stu-id="bd79f-120">Free</span></span>
    
- <span data-ttu-id="bd79f-121">Tentative</span><span class="sxs-lookup"><span data-stu-id="bd79f-121">Tentative</span></span>
    
- <span data-ttu-id="bd79f-122">Busy</span><span class="sxs-lookup"><span data-stu-id="bd79f-122">Busy</span></span>
    
- <span data-ttu-id="bd79f-123">不在時</span><span class="sxs-lookup"><span data-stu-id="bd79f-123">OOF</span></span>
    
- <span data-ttu-id="bd79f-124">NoData</span><span class="sxs-lookup"><span data-stu-id="bd79f-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="bd79f-125">備考</span><span class="sxs-lookup"><span data-stu-id="bd79f-125">Remarks</span></span>

<span data-ttu-id="bd79f-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bd79f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd79f-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="bd79f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd79f-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="bd79f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd79f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd79f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bd79f-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bd79f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd79f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd79f-131">Validation File</span></span>  <br/> |<span data-ttu-id="bd79f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd79f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd79f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd79f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd79f-134">False</span><span class="sxs-lookup"><span data-stu-id="bd79f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd79f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd79f-135">See also</span></span>



- [<span data-ttu-id="bd79f-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bd79f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

