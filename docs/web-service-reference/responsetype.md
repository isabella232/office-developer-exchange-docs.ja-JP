---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: ResponseType 要素は、受信した会議の受信者の応答の種類を表します。
ms.openlocfilehash: fcfd47cb988ee00303b2c4205cb3d058cb6599b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833200"
---
# <a name="responsetype"></a><span data-ttu-id="a8919-103">ResponseType</span><span class="sxs-lookup"><span data-stu-id="a8919-103">ResponseType</span></span>

<span data-ttu-id="a8919-104">**ResponseType**要素は、受信した会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-104">The **ResponseType** element represents the type of recipient response that is received for a meeting.</span></span> 
  
```xml
<ResponseType/>
```

 <span data-ttu-id="a8919-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="a8919-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8919-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a8919-106">Attributes and elements</span></span>

<span data-ttu-id="a8919-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8919-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8919-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8919-108">Attributes</span></span>

<span data-ttu-id="a8919-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a8919-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8919-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a8919-110">Child elements</span></span>

<span data-ttu-id="a8919-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a8919-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8919-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a8919-112">Parent elements</span></span>

|<span data-ttu-id="a8919-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8919-113">**Element**</span></span>|<span data-ttu-id="a8919-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8919-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8919-115">Attendee</span><span class="sxs-lookup"><span data-stu-id="a8919-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="a8919-116">出席者および会議のためのリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="a8919-117">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="a8919-117">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="a8919-118">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-118">Represents a meeting cancellation in the Exchange store</span></span>  <br/> |
|[<span data-ttu-id="a8919-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="a8919-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="a8919-120">Exchange ストア内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-120">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8919-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a8919-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a8919-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8919-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a8919-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="a8919-124">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="a8919-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8919-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8919-125">Text value</span></span>

<span data-ttu-id="a8919-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="a8919-126">A text value is required.</span></span> <span data-ttu-id="a8919-127">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="a8919-127">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="a8919-128">Unknown</span><span class="sxs-lookup"><span data-stu-id="a8919-128">Unknown</span></span>
    
- <span data-ttu-id="a8919-129">Organizer</span><span class="sxs-lookup"><span data-stu-id="a8919-129">Organizer</span></span>
    
- <span data-ttu-id="a8919-130">Tentative</span><span class="sxs-lookup"><span data-stu-id="a8919-130">Tentative</span></span>
    
- <span data-ttu-id="a8919-131">承諾</span><span class="sxs-lookup"><span data-stu-id="a8919-131">Accept</span></span>
    
- <span data-ttu-id="a8919-132">辞退</span><span class="sxs-lookup"><span data-stu-id="a8919-132">Decline</span></span>
    
- <span data-ttu-id="a8919-133">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="a8919-133">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a8919-134">備考</span><span class="sxs-lookup"><span data-stu-id="a8919-134">Remarks</span></span>

<span data-ttu-id="a8919-135">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a8919-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8919-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="a8919-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8919-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="a8919-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8919-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8919-138">Schema Name</span></span>  <br/> |<span data-ttu-id="a8919-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a8919-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8919-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8919-140">Validation File</span></span>  <br/> |<span data-ttu-id="a8919-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8919-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8919-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8919-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8919-143">False</span><span class="sxs-lookup"><span data-stu-id="a8919-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8919-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8919-144">See also</span></span>



- [<span data-ttu-id="a8919-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8919-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

