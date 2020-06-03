---
title: 会議の Requesttype
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
description: 会議の Requesttype 要素は、会議出席依頼の種類を表します。
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465787"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="3be87-103">会議の Requesttype</span><span class="sxs-lookup"><span data-stu-id="3be87-103">MeetingRequestType</span></span>

<span data-ttu-id="3be87-104">会議の**requesttype**要素は、会議出席依頼の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="3be87-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="3be87-105">**会議の Requesttypetype**</span><span class="sxs-lookup"><span data-stu-id="3be87-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3be87-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3be87-106">Attributes and elements</span></span>

<span data-ttu-id="3be87-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3be87-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3be87-108">属性</span><span class="sxs-lookup"><span data-stu-id="3be87-108">Attributes</span></span>

<span data-ttu-id="3be87-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3be87-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3be87-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3be87-110">Child elements</span></span>

<span data-ttu-id="3be87-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3be87-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3be87-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3be87-112">Parent elements</span></span>

|<span data-ttu-id="3be87-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3be87-113">**Element**</span></span>|<span data-ttu-id="3be87-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3be87-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3be87-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3be87-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3be87-116">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="3be87-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3be87-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3be87-117">Text value</span></span>

<span data-ttu-id="3be87-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="3be87-118">A text value is required.</span></span> <span data-ttu-id="3be87-119">次の表に、この要素に使用できるテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="3be87-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="3be87-120">**値**</span><span class="sxs-lookup"><span data-stu-id="3be87-120">**Value**</span></span>|<span data-ttu-id="3be87-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3be87-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3be87-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="3be87-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="3be87-123">既存の要求に対する完全な更新として会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="3be87-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="3be87-124">完全更新により、時間と情報のコンテンツが更新されました。</span><span class="sxs-lookup"><span data-stu-id="3be87-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="3be87-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="3be87-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="3be87-126">更新された情報コンテンツのみが含まれている会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="3be87-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="3be87-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3be87-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="3be87-128">会議出席依頼を新しい会議出席依頼として識別します。</span><span class="sxs-lookup"><span data-stu-id="3be87-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="3be87-129">なし</span><span class="sxs-lookup"><span data-stu-id="3be87-129">None</span></span>  <br/> |<span data-ttu-id="3be87-130">会議出席依頼の種類が定義されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="3be87-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="3be87-131">最新</span><span class="sxs-lookup"><span data-stu-id="3be87-131">Outdated</span></span>  <br/> |<span data-ttu-id="3be87-132">会議出席依頼を古いものとして識別します。</span><span class="sxs-lookup"><span data-stu-id="3be87-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="3be87-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="3be87-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="3be87-134">会議出席依頼が代理人に会議メッセージを転送しており、そのコピーが情報としてマークされているプリンシパルに属していることを示します。</span><span class="sxs-lookup"><span data-stu-id="3be87-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="3be87-135">孤立した更新</span><span class="sxs-lookup"><span data-stu-id="3be87-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="3be87-136">既存の会議へのサイレント更新として会議出席依頼を識別します。</span><span class="sxs-lookup"><span data-stu-id="3be87-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3be87-137">注釈</span><span class="sxs-lookup"><span data-stu-id="3be87-137">Remarks</span></span>

<span data-ttu-id="3be87-138">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="3be87-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3be87-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3be87-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3be87-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="3be87-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3be87-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3be87-141">Schema Name</span></span>  <br/> |<span data-ttu-id="3be87-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3be87-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="3be87-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3be87-143">Validation File</span></span>  <br/> |<span data-ttu-id="3be87-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3be87-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3be87-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3be87-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="3be87-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="3be87-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3be87-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="3be87-147">See also</span></span>



- [<span data-ttu-id="3be87-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3be87-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

