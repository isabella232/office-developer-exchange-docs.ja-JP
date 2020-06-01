---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: ReadItems 要素は、ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e040b643016781f9f890050f189191356f8d4f0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468300"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="51de7-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="51de7-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="51de7-105">**ReadItems**要素は、ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="51de7-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="51de7-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="51de7-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="51de7-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="51de7-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51de7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51de7-108">Attributes and elements</span></span>

<span data-ttu-id="51de7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51de7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51de7-110">属性</span><span class="sxs-lookup"><span data-stu-id="51de7-110">Attributes</span></span>

<span data-ttu-id="51de7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="51de7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51de7-112">子要素</span><span class="sxs-lookup"><span data-stu-id="51de7-112">Child elements</span></span>

<span data-ttu-id="51de7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="51de7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51de7-114">親要素</span><span class="sxs-lookup"><span data-stu-id="51de7-114">Parent elements</span></span>

|<span data-ttu-id="51de7-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="51de7-115">**Element**</span></span>|<span data-ttu-id="51de7-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="51de7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51de7-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="51de7-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="51de7-118">ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="51de7-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="51de7-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="51de7-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51de7-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="51de7-120">Text value</span></span>

<span data-ttu-id="51de7-121">次の表に、 **ReadItems**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="51de7-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="51de7-122">**ReadItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="51de7-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="51de7-123">**値**</span><span class="sxs-lookup"><span data-stu-id="51de7-123">**Value**</span></span>|<span data-ttu-id="51de7-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="51de7-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51de7-125">なし</span><span class="sxs-lookup"><span data-stu-id="51de7-125">None</span></span>  <br/> |<span data-ttu-id="51de7-126">ユーザーが予定表のアイテムを表示する権限を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="51de7-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="51de7-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="51de7-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="51de7-128">ユーザーが予定表の空き時間情報のみを表示するアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="51de7-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="51de7-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="51de7-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="51de7-130">ユーザーが予定表の空き時間情報を表示するためのアクセス許可と、予定の件名と場所を表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="51de7-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="51de7-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="51de7-131">FullDetails</span></span>  <br/> |<span data-ttu-id="51de7-132">ユーザーが予定表のすべてのアイテムを表示するためのアクセス許可を持っていることを示します。空き時間情報、件名、場所、および予定の詳細が含まれます。</span><span class="sxs-lookup"><span data-stu-id="51de7-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51de7-133">注釈</span><span class="sxs-lookup"><span data-stu-id="51de7-133">Remarks</span></span>

<span data-ttu-id="51de7-134">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="51de7-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51de7-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51de7-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51de7-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="51de7-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51de7-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51de7-137">Schema Name</span></span>  <br/> |<span data-ttu-id="51de7-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="51de7-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="51de7-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51de7-139">Validation File</span></span>  <br/> |<span data-ttu-id="51de7-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="51de7-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51de7-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51de7-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="51de7-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="51de7-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51de7-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="51de7-143">See also</span></span>



- [<span data-ttu-id="51de7-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="51de7-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="51de7-145">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="51de7-145">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

