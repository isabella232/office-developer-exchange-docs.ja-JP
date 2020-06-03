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
ms.openlocfilehash: ef5da21a3300a6939c60d62584b46ca48b071853
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526180"
---
# <a name="eventdata"></a><span data-ttu-id="6bc6c-103">EventData</span><span class="sxs-lookup"><span data-stu-id="6bc6c-103">EventData</span></span>

<span data-ttu-id="6bc6c-104">**EventData**要素は、イベントの処理手順に関連付けられているデータを表します。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-104">The **EventData** element represents data that is associated with the processing step for the event.</span></span> 
  
```XML
<EventData>
   <String/>
</EventData>
```

 <span data-ttu-id="6bc6c-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="6bc6c-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bc6c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6bc6c-106">Attributes and elements</span></span>

<span data-ttu-id="6bc6c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bc6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bc6c-108">Attributes</span></span>

<span data-ttu-id="6bc6c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bc6c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6bc6c-110">Child elements</span></span>

|<span data-ttu-id="6bc6c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6bc6c-111">**Element**</span></span>|<span data-ttu-id="6bc6c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6bc6c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bc6c-113">String</span><span class="sxs-lookup"><span data-stu-id="6bc6c-113">String</span></span>](string.md) <br/> |<span data-ttu-id="6bc6c-114">イベントを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-114">Contains a string that identifies an event.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6bc6c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6bc6c-115">Parent elements</span></span>

|<span data-ttu-id="6bc6c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6bc6c-116">**Element**</span></span>|<span data-ttu-id="6bc6c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6bc6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bc6c-118">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="6bc6c-118">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="6bc6c-119">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-119">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bc6c-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6bc6c-120">Text value</span></span>

<span data-ttu-id="6bc6c-121">なし。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6bc6c-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6bc6c-122">Remarks</span></span>

<span data-ttu-id="6bc6c-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6bc6c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bc6c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6bc6c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bc6c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6bc6c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6bc6c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6bc6c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6bc6c-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6bc6c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="6bc6c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6bc6c-128">Validation File</span></span>  <br/> |<span data-ttu-id="6bc6c-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6bc6c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6bc6c-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6bc6c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bc6c-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="6bc6c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bc6c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="6bc6c-132">See also</span></span>



- [<span data-ttu-id="6bc6c-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6bc6c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

