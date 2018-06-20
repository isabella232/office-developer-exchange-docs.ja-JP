---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: AppointmentState 要素は、予定の状態を指定します。
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759422"
---
# <a name="appointmentstate"></a><span data-ttu-id="7819a-103">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="7819a-103">AppointmentState</span></span>

<span data-ttu-id="7819a-104">**AppointmentState**要素は、予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="7819a-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="7819a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="7819a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7819a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7819a-106">Attributes and elements</span></span>

<span data-ttu-id="7819a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7819a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7819a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7819a-108">Attributes</span></span>

<span data-ttu-id="7819a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7819a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7819a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7819a-110">Child elements</span></span>

<span data-ttu-id="7819a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7819a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7819a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7819a-112">Parent elements</span></span>

|<span data-ttu-id="7819a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7819a-113">**Element**</span></span>|<span data-ttu-id="7819a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7819a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7819a-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="7819a-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7819a-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7819a-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7819a-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7819a-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7819a-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="7819a-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7819a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7819a-119">Text value</span></span>

<span data-ttu-id="7819a-120">この要素を表しますが、ビットを設定するテキスト値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7819a-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="7819a-121">これは整数です。</span><span class="sxs-lookup"><span data-stu-id="7819a-121">This is in integer form.</span></span> <span data-ttu-id="7819a-122">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7819a-122">This element is read-only.</span></span> <span data-ttu-id="7819a-123">応答でのみ返されます。</span><span class="sxs-lookup"><span data-stu-id="7819a-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7819a-124">備考</span><span class="sxs-lookup"><span data-stu-id="7819a-124">Remarks</span></span>

<span data-ttu-id="7819a-125">返される整数値では、予定の状態ビットマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7819a-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="7819a-126">次の表では、各ビットについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7819a-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="7819a-127">**名前**</span><span class="sxs-lookup"><span data-stu-id="7819a-127">**Name**</span></span>|<span data-ttu-id="7819a-128">**ビット**</span><span class="sxs-lookup"><span data-stu-id="7819a-128">**Bit**</span></span>|<span data-ttu-id="7819a-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="7819a-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7819a-130">なし</span><span class="sxs-lookup"><span data-stu-id="7819a-130">None</span></span>  <br/> |<span data-ttu-id="7819a-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="7819a-131">0x0000</span></span>  <br/> |<span data-ttu-id="7819a-132">フラグが設定されていません。</span><span class="sxs-lookup"><span data-stu-id="7819a-132">No flags have been set.</span></span> <span data-ttu-id="7819a-133">出席者が含まれていない予定の場合にだけ使用します。</span><span class="sxs-lookup"><span data-stu-id="7819a-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="7819a-134">会議</span><span class="sxs-lookup"><span data-stu-id="7819a-134">Meeting</span></span>  <br/> |<span data-ttu-id="7819a-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="7819a-135">0x0001</span></span>  <br/> |<span data-ttu-id="7819a-136">この予定は会議です。</span><span class="sxs-lookup"><span data-stu-id="7819a-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="7819a-137">Received</span><span class="sxs-lookup"><span data-stu-id="7819a-137">Received</span></span>  <br/> |<span data-ttu-id="7819a-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="7819a-138">0x0002</span></span>  <br/> |<span data-ttu-id="7819a-139">この予定を受信しました。</span><span class="sxs-lookup"><span data-stu-id="7819a-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="7819a-140">キャンセル済み</span><span class="sxs-lookup"><span data-stu-id="7819a-140">Canceled</span></span>  <br/> |<span data-ttu-id="7819a-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="7819a-141">0x0004</span></span>  <br/> |<span data-ttu-id="7819a-142">この予定は取り消されました。</span><span class="sxs-lookup"><span data-stu-id="7819a-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="7819a-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7819a-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7819a-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="7819a-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7819a-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="7819a-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7819a-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7819a-146">Schema name</span></span>  <br/> |<span data-ttu-id="7819a-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7819a-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="7819a-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7819a-148">Validation file</span></span>  <br/> |<span data-ttu-id="7819a-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7819a-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7819a-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7819a-150">Can be empty</span></span>  <br/> |<span data-ttu-id="7819a-151">False</span><span class="sxs-lookup"><span data-stu-id="7819a-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7819a-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="7819a-152">See also</span></span>

- [<span data-ttu-id="7819a-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7819a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

