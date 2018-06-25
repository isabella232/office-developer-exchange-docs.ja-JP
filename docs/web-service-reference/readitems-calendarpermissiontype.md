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
description: ReadItems 要素は、ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832964"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="8e3ca-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="8e3ca-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="8e3ca-105">**ReadItems**要素は、ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="8e3ca-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="8e3ca-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e3ca-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8e3ca-108">Attributes and elements</span></span>

<span data-ttu-id="8e3ca-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e3ca-110">属性</span><span class="sxs-lookup"><span data-stu-id="8e3ca-110">Attributes</span></span>

<span data-ttu-id="8e3ca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e3ca-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8e3ca-112">Child elements</span></span>

<span data-ttu-id="8e3ca-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e3ca-114">親要素</span><span class="sxs-lookup"><span data-stu-id="8e3ca-114">Parent elements</span></span>

|<span data-ttu-id="8e3ca-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-115">**Element**</span></span>|<span data-ttu-id="8e3ca-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e3ca-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="8e3ca-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="8e3ca-118">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="8e3ca-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e3ca-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e3ca-120">Text value</span></span>

<span data-ttu-id="8e3ca-121">**ReadItems**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="8e3ca-122">**ReadItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="8e3ca-123">**値**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-123">**Value**</span></span>|<span data-ttu-id="8e3ca-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e3ca-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e3ca-125">なし</span><span class="sxs-lookup"><span data-stu-id="8e3ca-125">None</span></span>  <br/> |<span data-ttu-id="8e3ca-126">ユーザーに予定表にアイテムを表示する権限がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="8e3ca-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="8e3ca-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="8e3ca-128">ユーザーが予定表の空き時間のみを表示する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="8e3ca-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="8e3ca-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="8e3ca-130">ユーザーが予定表、件名、予定の場所に空き時間情報を表示するアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="8e3ca-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="8e3ca-131">FullDetails</span></span>  <br/> |<span data-ttu-id="8e3ca-132">ユーザーが空き時間情報、件名、場所、および予定の詳細情報を含む、予定表のすべての項目を表示する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e3ca-133">備考</span><span class="sxs-lookup"><span data-stu-id="8e3ca-133">Remarks</span></span>

<span data-ttu-id="8e3ca-134">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8e3ca-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e3ca-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="8e3ca-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e3ca-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="8e3ca-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e3ca-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e3ca-137">Schema Name</span></span>  <br/> |<span data-ttu-id="8e3ca-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8e3ca-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e3ca-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e3ca-139">Validation File</span></span>  <br/> |<span data-ttu-id="8e3ca-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e3ca-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e3ca-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8e3ca-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e3ca-142">False</span><span class="sxs-lookup"><span data-stu-id="8e3ca-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e3ca-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e3ca-143">See also</span></span>



- [<span data-ttu-id="8e3ca-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e3ca-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8e3ca-145">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="8e3ca-145">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

