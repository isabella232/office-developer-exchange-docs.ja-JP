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
description: FreeBusyView 要素には、特定のユーザーの利用可能時間情報が含まれています。
ms.openlocfilehash: d0d603f18642a94e841a1a6bb8e8849aa6b5b273
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760602"
---
# <a name="freebusyview"></a><span data-ttu-id="eb572-103">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="eb572-103">FreeBusyView</span></span>

<span data-ttu-id="eb572-104">**FreeBusyView**要素には、特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb572-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="eb572-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eb572-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="eb572-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="eb572-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="eb572-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="eb572-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="eb572-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="eb572-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="eb572-109">**FreeBusyView**</span><span class="sxs-lookup"><span data-stu-id="eb572-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb572-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eb572-110">Attributes and elements</span></span>

<span data-ttu-id="eb572-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eb572-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb572-112">属性</span><span class="sxs-lookup"><span data-stu-id="eb572-112">Attributes</span></span>

<span data-ttu-id="eb572-113">なし。</span><span class="sxs-lookup"><span data-stu-id="eb572-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb572-114">子要素</span><span class="sxs-lookup"><span data-stu-id="eb572-114">Child elements</span></span>

|<span data-ttu-id="eb572-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb572-115">**Element**</span></span>|<span data-ttu-id="eb572-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb572-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb572-117">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="eb572-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="eb572-118">要求された空き時間情報が応答で返されるの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="eb572-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="eb572-119">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="eb572-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="eb572-120">結合された空き時間情報データ ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb572-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="eb572-121">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="eb572-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="eb572-122">要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb572-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="eb572-123">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="eb572-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="eb572-124">要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="eb572-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb572-125">親要素</span><span class="sxs-lookup"><span data-stu-id="eb572-125">Parent elements</span></span>

|<span data-ttu-id="eb572-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb572-126">**Element**</span></span>|<span data-ttu-id="eb572-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb572-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb572-128">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="eb572-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="eb572-129">1 つのメールボックスのユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb572-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="eb572-130">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="eb572-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb572-131">備考</span><span class="sxs-lookup"><span data-stu-id="eb572-131">Remarks</span></span>

<span data-ttu-id="eb572-132">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="eb572-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="eb572-133">この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。</span><span class="sxs-lookup"><span data-stu-id="eb572-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="eb572-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="eb572-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb572-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="eb572-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb572-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="eb572-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb572-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb572-137">Schema Name</span></span>  <br/> |<span data-ttu-id="eb572-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="eb572-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb572-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb572-139">Validation File</span></span>  <br/> |<span data-ttu-id="eb572-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb572-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb572-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eb572-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb572-142">False</span><span class="sxs-lookup"><span data-stu-id="eb572-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb572-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb572-143">See also</span></span>



[<span data-ttu-id="eb572-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="eb572-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="eb572-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eb572-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="eb572-146">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="eb572-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

