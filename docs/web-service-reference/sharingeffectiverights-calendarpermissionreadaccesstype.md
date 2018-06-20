---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: SharingEffectiveRights 要素は、ユーザーが共有されている予定表データを持っているアクセス許可を示します。
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="ef057-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="ef057-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="ef057-104">**SharingEffectiveRights**要素は、ユーザーが共有されている予定表データを持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="ef057-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="ef057-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="ef057-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef057-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ef057-106">Attributes and elements</span></span>

<span data-ttu-id="ef057-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef057-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef057-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef057-108">Attributes</span></span>

<span data-ttu-id="ef057-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ef057-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef057-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ef057-110">Child elements</span></span>

<span data-ttu-id="ef057-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ef057-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef057-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ef057-112">Parent elements</span></span>

|<span data-ttu-id="ef057-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ef057-113">**Element**</span></span>|<span data-ttu-id="ef057-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef057-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef057-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="ef057-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="ef057-116">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ef057-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef057-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ef057-117">Text value</span></span>

<span data-ttu-id="ef057-118">次の表は、 **SharingEffectiveRights**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="ef057-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="ef057-119">**値**</span><span class="sxs-lookup"><span data-stu-id="ef057-119">**Value**</span></span>|<span data-ttu-id="ef057-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef057-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef057-121">なし</span><span class="sxs-lookup"><span data-stu-id="ef057-121">None</span></span>  <br/> |<span data-ttu-id="ef057-122">ユーザーに予定表にアイテムを表示する権限がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ef057-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="ef057-123">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="ef057-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="ef057-124">ユーザーが予定表の空き時間のみを表示する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ef057-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="ef057-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="ef057-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="ef057-126">ユーザーが予定表、件名、予定の場所に空き時間情報を表示するアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ef057-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="ef057-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ef057-127">FullDetails</span></span>  <br/> |<span data-ttu-id="ef057-128">ユーザーが空き時間情報、件名、場所、および予定の詳細情報を含む、予定表のすべての項目を表示する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ef057-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef057-129">備考</span><span class="sxs-lookup"><span data-stu-id="ef057-129">Remarks</span></span>

<span data-ttu-id="ef057-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ef057-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef057-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="ef057-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef057-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="ef057-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef057-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef057-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ef057-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ef057-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef057-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef057-135">Validation File</span></span>  <br/> |<span data-ttu-id="ef057-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef057-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef057-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ef057-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef057-138">False</span><span class="sxs-lookup"><span data-stu-id="ef057-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef057-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef057-139">See also</span></span>



- [<span data-ttu-id="ef057-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ef057-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

