---
title: EventData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventData
api_type:
- schema
ms.assetid: 74acdbad-d6ee-47e6-82fb-e45ecaaa0500
description: EventData 要素は、イベントの処理手順に関連付けられているデータを表します。
ms.openlocfilehash: 2bf38cd4fd956580b31b6e455b947066f07f5593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760337"
---
# <a name="eventdata"></a><span data-ttu-id="500a9-103">EventData</span><span class="sxs-lookup"><span data-stu-id="500a9-103">EventData</span></span>

<span data-ttu-id="500a9-104">**EventData**要素は、イベントの処理手順に関連付けられているデータを表します。</span><span class="sxs-lookup"><span data-stu-id="500a9-104">The **EventData** element represents data that is associated with the processing step for the event.</span></span> 
  
```XML
<EventData>
   <String/>
</EventData>
```

 <span data-ttu-id="500a9-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="500a9-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="500a9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="500a9-106">Attributes and elements</span></span>

<span data-ttu-id="500a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="500a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="500a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="500a9-108">Attributes</span></span>

<span data-ttu-id="500a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="500a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="500a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="500a9-110">Child elements</span></span>

|<span data-ttu-id="500a9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="500a9-111">**Element**</span></span>|<span data-ttu-id="500a9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="500a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="500a9-113">String</span><span class="sxs-lookup"><span data-stu-id="500a9-113">String</span></span>](string.md) <br/> |<span data-ttu-id="500a9-114">イベントを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="500a9-114">Contains a string that identifies an event.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="500a9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="500a9-115">Parent elements</span></span>

|<span data-ttu-id="500a9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="500a9-116">**Element**</span></span>|<span data-ttu-id="500a9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="500a9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="500a9-118">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="500a9-118">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="500a9-119">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="500a9-119">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="500a9-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="500a9-120">Text value</span></span>

<span data-ttu-id="500a9-121">なし。</span><span class="sxs-lookup"><span data-stu-id="500a9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="500a9-122">備考</span><span class="sxs-lookup"><span data-stu-id="500a9-122">Remarks</span></span>

<span data-ttu-id="500a9-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="500a9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="500a9-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="500a9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="500a9-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="500a9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="500a9-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="500a9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="500a9-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="500a9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="500a9-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="500a9-128">Validation File</span></span>  <br/> |<span data-ttu-id="500a9-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="500a9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="500a9-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="500a9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="500a9-131">False</span><span class="sxs-lookup"><span data-stu-id="500a9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="500a9-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="500a9-132">See also</span></span>



- [<span data-ttu-id="500a9-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="500a9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

