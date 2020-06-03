---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: FreeBusyView 要素には、特定のユーザーの空き時間情報が含まれています。
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456102"
---
# <a name="freebusyview"></a><span data-ttu-id="1ea78-103">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1ea78-103">FreeBusyView</span></span>

<span data-ttu-id="1ea78-104">**FreeBusyView**要素には、特定のユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ea78-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="1ea78-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ea78-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1ea78-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1ea78-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1ea78-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1ea78-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1ea78-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1ea78-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="1ea78-109">**FreeBusyView**</span><span class="sxs-lookup"><span data-stu-id="1ea78-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ea78-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1ea78-110">Attributes and elements</span></span>

<span data-ttu-id="1ea78-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ea78-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ea78-112">属性</span><span class="sxs-lookup"><span data-stu-id="1ea78-112">Attributes</span></span>

<span data-ttu-id="1ea78-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1ea78-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ea78-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1ea78-114">Child elements</span></span>

|<span data-ttu-id="1ea78-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="1ea78-115">**Element**</span></span>|<span data-ttu-id="1ea78-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ea78-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ea78-117">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="1ea78-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="1ea78-118">応答で返される要求された空き時間情報の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="1ea78-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="1ea78-119">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="1ea78-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="1ea78-120">データのマージされた空き時間ストリームを格納します。</span><span class="sxs-lookup"><span data-stu-id="1ea78-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="1ea78-121">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1ea78-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="1ea78-122">要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムの繰り返しを含みます。</span><span class="sxs-lookup"><span data-stu-id="1ea78-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="1ea78-123">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="1ea78-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1ea78-124">要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。</span><span class="sxs-lookup"><span data-stu-id="1ea78-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ea78-125">親要素</span><span class="sxs-lookup"><span data-stu-id="1ea78-125">Parent elements</span></span>

|<span data-ttu-id="1ea78-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ea78-126">**Element**</span></span>|<span data-ttu-id="1ea78-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ea78-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ea78-128">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1ea78-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="1ea78-129">1つのメールボックスユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ea78-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="1ea78-130">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ea78-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ea78-131">注釈</span><span class="sxs-lookup"><span data-stu-id="1ea78-131">Remarks</span></span>

<span data-ttu-id="1ea78-132">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ea78-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="1ea78-133">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="1ea78-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="1ea78-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1ea78-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ea78-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1ea78-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ea78-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ea78-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ea78-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ea78-137">Schema Name</span></span>  <br/> |<span data-ttu-id="1ea78-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1ea78-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ea78-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ea78-139">Validation File</span></span>  <br/> |<span data-ttu-id="1ea78-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1ea78-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ea78-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ea78-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ea78-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="1ea78-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ea78-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ea78-143">See also</span></span>



[<span data-ttu-id="1ea78-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1ea78-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1ea78-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ea78-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1ea78-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="1ea78-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

