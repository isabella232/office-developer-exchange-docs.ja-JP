---
title: RecipientTrackingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvents
api_type:
- schema
ms.assetid: c4f729aa-674e-43b2-97f2-bf49740b0a34
description: RecipientTrackingEvents 要素は、メッセージの 1 つまたは複数のイベントのコレクションを表します。
ms.openlocfilehash: 5fa5df422eff533891d021b77d5443b314d36244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832993"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="db496-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="db496-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="db496-104">**RecipientTrackingEvents**要素は、メッセージの 1 つまたは複数のイベントのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="db496-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="db496-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="db496-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db496-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="db496-106">Attributes and elements</span></span>

<span data-ttu-id="db496-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db496-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db496-108">属性</span><span class="sxs-lookup"><span data-stu-id="db496-108">Attributes</span></span>

<span data-ttu-id="db496-109">なし。</span><span class="sxs-lookup"><span data-stu-id="db496-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db496-110">子要素</span><span class="sxs-lookup"><span data-stu-id="db496-110">Child elements</span></span>

|<span data-ttu-id="db496-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="db496-111">**Element**</span></span>|<span data-ttu-id="db496-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="db496-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db496-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="db496-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="db496-114">追跡レポートで特定のイベントの詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="db496-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db496-115">親要素</span><span class="sxs-lookup"><span data-stu-id="db496-115">Parent elements</span></span>

|<span data-ttu-id="db496-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="db496-116">**Element**</span></span>|<span data-ttu-id="db496-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="db496-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db496-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="db496-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="db496-119">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="db496-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="db496-120">備考</span><span class="sxs-lookup"><span data-stu-id="db496-120">Remarks</span></span>

<span data-ttu-id="db496-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="db496-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db496-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="db496-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db496-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="db496-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db496-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db496-124">Schema Name</span></span>  <br/> |<span data-ttu-id="db496-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="db496-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="db496-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db496-126">Validation File</span></span>  <br/> |<span data-ttu-id="db496-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db496-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db496-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db496-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="db496-129">False</span><span class="sxs-lookup"><span data-stu-id="db496-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db496-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="db496-130">See also</span></span>



[<span data-ttu-id="db496-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="db496-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="db496-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="db496-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

