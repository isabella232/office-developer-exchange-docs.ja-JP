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
description: ResponseType 要素は、会議に対して受信される受信者応答の種類を表します。
ms.openlocfilehash: ef8183b71e267a20427873ca44b269b828686cbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465395"
---
# <a name="responsetype"></a><span data-ttu-id="eff13-103">ResponseType</span><span class="sxs-lookup"><span data-stu-id="eff13-103">ResponseType</span></span>

<span data-ttu-id="eff13-104">**Responsetype**要素は、会議に対して受信される受信者応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-104">The **ResponseType** element represents the type of recipient response that is received for a meeting.</span></span> 
  
```xml
<ResponseType/>
```

 <span data-ttu-id="eff13-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="eff13-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eff13-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eff13-106">Attributes and elements</span></span>

<span data-ttu-id="eff13-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eff13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eff13-108">属性</span><span class="sxs-lookup"><span data-stu-id="eff13-108">Attributes</span></span>

<span data-ttu-id="eff13-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eff13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eff13-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eff13-110">Child elements</span></span>

<span data-ttu-id="eff13-111">なし。</span><span class="sxs-lookup"><span data-stu-id="eff13-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eff13-112">親要素</span><span class="sxs-lookup"><span data-stu-id="eff13-112">Parent elements</span></span>

|<span data-ttu-id="eff13-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="eff13-113">**Element**</span></span>|<span data-ttu-id="eff13-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="eff13-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eff13-115">出席者</span><span class="sxs-lookup"><span data-stu-id="eff13-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="eff13-116">会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="eff13-117">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="eff13-117">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="eff13-118">Exchange ストアの会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-118">Represents a meeting cancellation in the Exchange store</span></span>  <br/> |
|[<span data-ttu-id="eff13-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="eff13-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="eff13-120">Exchange ストア内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-120">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="eff13-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="eff13-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="eff13-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="eff13-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="eff13-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="eff13-124">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="eff13-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eff13-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eff13-125">Text value</span></span>

<span data-ttu-id="eff13-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="eff13-126">A text value is required.</span></span> <span data-ttu-id="eff13-127">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="eff13-127">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="eff13-128">不明</span><span class="sxs-lookup"><span data-stu-id="eff13-128">Unknown</span></span>
    
- <span data-ttu-id="eff13-129">開催者</span><span class="sxs-lookup"><span data-stu-id="eff13-129">Organizer</span></span>
    
- <span data-ttu-id="eff13-130">仮の予定</span><span class="sxs-lookup"><span data-stu-id="eff13-130">Tentative</span></span>
    
- <span data-ttu-id="eff13-131">承諾</span><span class="sxs-lookup"><span data-stu-id="eff13-131">Accept</span></span>
    
- <span data-ttu-id="eff13-132">同意</span><span class="sxs-lookup"><span data-stu-id="eff13-132">Decline</span></span>
    
- <span data-ttu-id="eff13-133">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="eff13-133">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="eff13-134">注釈</span><span class="sxs-lookup"><span data-stu-id="eff13-134">Remarks</span></span>

<span data-ttu-id="eff13-135">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="eff13-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eff13-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eff13-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eff13-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="eff13-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eff13-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eff13-138">Schema Name</span></span>  <br/> |<span data-ttu-id="eff13-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="eff13-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="eff13-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eff13-140">Validation File</span></span>  <br/> |<span data-ttu-id="eff13-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="eff13-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eff13-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eff13-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="eff13-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="eff13-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eff13-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="eff13-144">See also</span></span>



- [<span data-ttu-id="eff13-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="eff13-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

