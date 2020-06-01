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
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463476"
---
# <a name="appointmentstate"></a><span data-ttu-id="c090e-103">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="c090e-103">AppointmentState</span></span>

<span data-ttu-id="c090e-104">**AppointmentState**要素は、予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="c090e-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="c090e-105">**int**</span><span class="sxs-lookup"><span data-stu-id="c090e-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c090e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c090e-106">Attributes and elements</span></span>

<span data-ttu-id="c090e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c090e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c090e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c090e-108">Attributes</span></span>

<span data-ttu-id="c090e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c090e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c090e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c090e-110">Child elements</span></span>

<span data-ttu-id="c090e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c090e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c090e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c090e-112">Parent elements</span></span>

|<span data-ttu-id="c090e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c090e-113">**Element**</span></span>|<span data-ttu-id="c090e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c090e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c090e-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c090e-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c090e-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c090e-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c090e-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c090e-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c090e-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="c090e-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c090e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c090e-119">Text value</span></span>

<span data-ttu-id="c090e-120">この要素には、セットビットを表すテキスト値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c090e-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="c090e-121">これは整数形式です。</span><span class="sxs-lookup"><span data-stu-id="c090e-121">This is in integer form.</span></span> <span data-ttu-id="c090e-122">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c090e-122">This element is read-only.</span></span> <span data-ttu-id="c090e-123">応答でのみ返されます。</span><span class="sxs-lookup"><span data-stu-id="c090e-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c090e-124">注釈</span><span class="sxs-lookup"><span data-stu-id="c090e-124">Remarks</span></span>

<span data-ttu-id="c090e-125">返される整数値は、予定の状態ビットマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="c090e-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="c090e-126">次の表で、各ビットについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c090e-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="c090e-127">**名前**</span><span class="sxs-lookup"><span data-stu-id="c090e-127">**Name**</span></span>|<span data-ttu-id="c090e-128">**若干**</span><span class="sxs-lookup"><span data-stu-id="c090e-128">**Bit**</span></span>|<span data-ttu-id="c090e-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="c090e-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c090e-130">なし</span><span class="sxs-lookup"><span data-stu-id="c090e-130">None</span></span>  <br/> |<span data-ttu-id="c090e-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="c090e-131">0x0000</span></span>  <br/> |<span data-ttu-id="c090e-132">フラグが設定されていません。</span><span class="sxs-lookup"><span data-stu-id="c090e-132">No flags have been set.</span></span> <span data-ttu-id="c090e-133">これは、出席者が含まれていない予定に対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="c090e-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="c090e-134">会議</span><span class="sxs-lookup"><span data-stu-id="c090e-134">Meeting</span></span>  <br/> |<span data-ttu-id="c090e-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="c090e-135">0x0001</span></span>  <br/> |<span data-ttu-id="c090e-136">この予定は会議です。</span><span class="sxs-lookup"><span data-stu-id="c090e-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="c090e-137">受信済み</span><span class="sxs-lookup"><span data-stu-id="c090e-137">Received</span></span>  <br/> |<span data-ttu-id="c090e-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="c090e-138">0x0002</span></span>  <br/> |<span data-ttu-id="c090e-139">この予定を受信しました。</span><span class="sxs-lookup"><span data-stu-id="c090e-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="c090e-140">キャンセル済み</span><span class="sxs-lookup"><span data-stu-id="c090e-140">Canceled</span></span>  <br/> |<span data-ttu-id="c090e-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="c090e-141">0x0004</span></span>  <br/> |<span data-ttu-id="c090e-142">この予定はキャンセルされました。</span><span class="sxs-lookup"><span data-stu-id="c090e-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="c090e-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c090e-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c090e-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c090e-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c090e-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="c090e-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c090e-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c090e-146">Schema name</span></span>  <br/> |<span data-ttu-id="c090e-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c090e-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="c090e-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c090e-148">Validation file</span></span>  <br/> |<span data-ttu-id="c090e-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c090e-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c090e-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c090e-150">Can be empty</span></span>  <br/> |<span data-ttu-id="c090e-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="c090e-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c090e-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="c090e-152">See also</span></span>

- [<span data-ttu-id="c090e-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c090e-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

