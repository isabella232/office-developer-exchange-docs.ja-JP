---
title: 受信者 Trackingevents
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
description: 受信者 Trackingevents 要素は、メッセージの1つまたは複数のイベントのコレクションを表します。
ms.openlocfilehash: c0b25a0e22d13bc1f26768b9b7089d96eb2e8cfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468482"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="69b6c-103">受信者 Trackingevents</span><span class="sxs-lookup"><span data-stu-id="69b6c-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="69b6c-104">**受信者 trackingevents**要素は、メッセージの1つまたは複数のイベントのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="69b6c-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="69b6c-105">**Arrayof受信者 Trackingeventtype**</span><span class="sxs-lookup"><span data-stu-id="69b6c-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69b6c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="69b6c-106">Attributes and elements</span></span>

<span data-ttu-id="69b6c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69b6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69b6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="69b6c-108">Attributes</span></span>

<span data-ttu-id="69b6c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="69b6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69b6c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="69b6c-110">Child elements</span></span>

|<span data-ttu-id="69b6c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="69b6c-111">**Element**</span></span>|<span data-ttu-id="69b6c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="69b6c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69b6c-113">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="69b6c-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="69b6c-114">追跡レポートの特定のイベントの詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="69b6c-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69b6c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="69b6c-115">Parent elements</span></span>

|<span data-ttu-id="69b6c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="69b6c-116">**Element**</span></span>|<span data-ttu-id="69b6c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="69b6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69b6c-118">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="69b6c-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="69b6c-119">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="69b6c-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69b6c-120">注釈</span><span class="sxs-lookup"><span data-stu-id="69b6c-120">Remarks</span></span>

<span data-ttu-id="69b6c-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="69b6c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69b6c-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="69b6c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69b6c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="69b6c-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69b6c-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69b6c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="69b6c-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="69b6c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="69b6c-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69b6c-126">Validation File</span></span>  <br/> |<span data-ttu-id="69b6c-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="69b6c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69b6c-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69b6c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="69b6c-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="69b6c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69b6c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="69b6c-130">See also</span></span>



[<span data-ttu-id="69b6c-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="69b6c-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="69b6c-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="69b6c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

