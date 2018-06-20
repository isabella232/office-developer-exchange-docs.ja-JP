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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832993"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="d9601-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="d9601-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="d9601-104">**RecipientTrackingEvents**要素は、メッセージの 1 つまたは複数のイベントのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d9601-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="d9601-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="d9601-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9601-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d9601-106">Attributes and elements</span></span>

<span data-ttu-id="d9601-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9601-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9601-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9601-108">Attributes</span></span>

<span data-ttu-id="d9601-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d9601-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9601-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d9601-110">Child elements</span></span>

|<span data-ttu-id="d9601-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9601-111">**Element**</span></span>|<span data-ttu-id="d9601-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9601-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9601-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="d9601-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="d9601-114">追跡レポートで特定のイベントの詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9601-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9601-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d9601-115">Parent elements</span></span>

|<span data-ttu-id="d9601-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9601-116">**Element**</span></span>|<span data-ttu-id="d9601-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9601-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9601-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d9601-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="d9601-119">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9601-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9601-120">備考</span><span class="sxs-lookup"><span data-stu-id="d9601-120">Remarks</span></span>

<span data-ttu-id="d9601-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9601-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9601-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d9601-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9601-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d9601-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9601-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9601-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d9601-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9601-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9601-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9601-126">Validation File</span></span>  <br/> |<span data-ttu-id="d9601-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9601-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9601-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9601-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9601-129">False</span><span class="sxs-lookup"><span data-stu-id="d9601-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9601-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9601-130">See also</span></span>



[<span data-ttu-id="d9601-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="d9601-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="d9601-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9601-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

