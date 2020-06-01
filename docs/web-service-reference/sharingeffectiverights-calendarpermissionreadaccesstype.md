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
description: SharingEffectiveRights 要素は、共有されている予定表データに対してユーザーが持っているアクセス許可を示します。
ms.openlocfilehash: 5581e9cc001608a124ae94e69eba836f6fd98520
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458580"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="b2dab-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="b2dab-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="b2dab-104">**SharingEffectiveRights**要素は、共有されている予定表データに対してユーザーが持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="b2dab-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="b2dab-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2dab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b2dab-106">Attributes and elements</span></span>

<span data-ttu-id="b2dab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2dab-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2dab-108">Attributes</span></span>

<span data-ttu-id="b2dab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2dab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2dab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2dab-110">Child elements</span></span>

<span data-ttu-id="b2dab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b2dab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2dab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2dab-112">Parent elements</span></span>

|<span data-ttu-id="b2dab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b2dab-113">**Element**</span></span>|<span data-ttu-id="b2dab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2dab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2dab-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="b2dab-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="b2dab-116">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2dab-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b2dab-117">Text value</span></span>

<span data-ttu-id="b2dab-118">次の表に、 **SharingEffectiveRights**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="b2dab-119">**値**</span><span class="sxs-lookup"><span data-stu-id="b2dab-119">**Value**</span></span>|<span data-ttu-id="b2dab-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2dab-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b2dab-121">なし</span><span class="sxs-lookup"><span data-stu-id="b2dab-121">None</span></span>  <br/> |<span data-ttu-id="b2dab-122">ユーザーが予定表のアイテムを表示する権限を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="b2dab-123">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="b2dab-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="b2dab-124">ユーザーが予定表の空き時間情報のみを表示するアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="b2dab-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="b2dab-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="b2dab-126">ユーザーが予定表の空き時間情報を表示するためのアクセス許可と、予定の件名と場所を表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="b2dab-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="b2dab-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2dab-127">FullDetails</span></span>  <br/> |<span data-ttu-id="b2dab-128">ユーザーが予定表のすべてのアイテムを表示するためのアクセス許可を持っていることを示します。空き時間情報、件名、場所、および予定の詳細が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b2dab-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b2dab-129">注釈</span><span class="sxs-lookup"><span data-stu-id="b2dab-129">Remarks</span></span>

<span data-ttu-id="b2dab-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2dab-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2dab-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b2dab-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2dab-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2dab-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2dab-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2dab-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b2dab-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b2dab-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2dab-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2dab-135">Validation File</span></span>  <br/> |<span data-ttu-id="b2dab-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b2dab-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2dab-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b2dab-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2dab-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="b2dab-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2dab-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2dab-139">See also</span></span>



- [<span data-ttu-id="b2dab-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b2dab-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

