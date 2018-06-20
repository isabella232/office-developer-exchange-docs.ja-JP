---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: MeetingRequestType 要素は、会議出席依頼の種類について説明します。
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832432"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="90ad6-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="90ad6-103">MeetingRequestType</span></span>

<span data-ttu-id="90ad6-104">**MeetingRequestType**要素は、会議出席依頼の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="90ad6-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="90ad6-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90ad6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="90ad6-106">Attributes and elements</span></span>

<span data-ttu-id="90ad6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90ad6-108">属性</span><span class="sxs-lookup"><span data-stu-id="90ad6-108">Attributes</span></span>

<span data-ttu-id="90ad6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90ad6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90ad6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90ad6-110">Child elements</span></span>

<span data-ttu-id="90ad6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="90ad6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90ad6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="90ad6-112">Parent elements</span></span>

|<span data-ttu-id="90ad6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="90ad6-113">**Element**</span></span>|<span data-ttu-id="90ad6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="90ad6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90ad6-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="90ad6-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="90ad6-116">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90ad6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="90ad6-117">Text value</span></span>

<span data-ttu-id="90ad6-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="90ad6-118">A text value is required.</span></span> <span data-ttu-id="90ad6-119">次の表は、この要素の使用可能なテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="90ad6-120">**値**</span><span class="sxs-lookup"><span data-stu-id="90ad6-120">**Value**</span></span>|<span data-ttu-id="90ad6-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="90ad6-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90ad6-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="90ad6-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="90ad6-123">会議出席依頼が既存の要求に完全な更新であることを識別します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="90ad6-124">フル更新には、時間と情報が更新されました。</span><span class="sxs-lookup"><span data-stu-id="90ad6-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="90ad6-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="90ad6-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="90ad6-126">情報コンテンツの更新のみを含む会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="90ad6-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="90ad6-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="90ad6-128">新しい会議出席依頼と会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="90ad6-129">なし</span><span class="sxs-lookup"><span data-stu-id="90ad6-129">None</span></span>  <br/> |<span data-ttu-id="90ad6-130">会議出席依頼の種類にすることを示しますが定義されていません。</span><span class="sxs-lookup"><span data-stu-id="90ad6-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="90ad6-131">古い</span><span class="sxs-lookup"><span data-stu-id="90ad6-131">Outdated</span></span>  <br/> |<span data-ttu-id="90ad6-132">として古い会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="90ad6-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="90ad6-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="90ad6-134">会議出席依頼が代理人に会議のメッセージを転送するには情報とマークされている彼のコピーのあるプリンシパルに属していることを示します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="90ad6-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="90ad6-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="90ad6-136">会議出席依頼を既存の会議に更新プログラムがサイレントとして識別します。</span><span class="sxs-lookup"><span data-stu-id="90ad6-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90ad6-137">備考</span><span class="sxs-lookup"><span data-stu-id="90ad6-137">Remarks</span></span>

<span data-ttu-id="90ad6-138">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="90ad6-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90ad6-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="90ad6-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90ad6-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="90ad6-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90ad6-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90ad6-141">Schema Name</span></span>  <br/> |<span data-ttu-id="90ad6-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="90ad6-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="90ad6-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90ad6-143">Validation File</span></span>  <br/> |<span data-ttu-id="90ad6-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90ad6-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90ad6-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="90ad6-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="90ad6-146">False</span><span class="sxs-lookup"><span data-stu-id="90ad6-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90ad6-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="90ad6-147">See also</span></span>



- [<span data-ttu-id="90ad6-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="90ad6-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

