---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: DeleteItems 要素では、フォルダー内のどのアイテムを削除する権限をユーザーが持っていることを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759994"
---
# <a name="deleteitems"></a><span data-ttu-id="4fa7f-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="4fa7f-104">DeleteItems</span></span>

<span data-ttu-id="4fa7f-105">**DeleteItems**要素では、フォルダー内のどのアイテムを削除する権限をユーザーが持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="4fa7f-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="4fa7f-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fa7f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4fa7f-108">Attributes and elements</span></span>

<span data-ttu-id="4fa7f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fa7f-110">属性</span><span class="sxs-lookup"><span data-stu-id="4fa7f-110">Attributes</span></span>

<span data-ttu-id="4fa7f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fa7f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4fa7f-112">Child elements</span></span>

<span data-ttu-id="4fa7f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fa7f-114">親要素</span><span class="sxs-lookup"><span data-stu-id="4fa7f-114">Parent elements</span></span>

|<span data-ttu-id="4fa7f-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-115">**Element**</span></span>|<span data-ttu-id="4fa7f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fa7f-117">Permission</span><span class="sxs-lookup"><span data-stu-id="4fa7f-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="4fa7f-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="4fa7f-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4fa7f-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="4fa7f-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="4fa7f-121">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="4fa7f-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fa7f-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4fa7f-123">Text value</span></span>

<span data-ttu-id="4fa7f-124">次の表は、 **DeleteItems**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="4fa7f-125">**DeleteItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="4fa7f-126">**値**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-126">**Value**</span></span>|<span data-ttu-id="4fa7f-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa7f-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa7f-128">なし</span><span class="sxs-lookup"><span data-stu-id="4fa7f-128">None</span></span>  <br/> |<span data-ttu-id="4fa7f-129">ユーザーに、フォルダー内のアイテムを削除する権限がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="4fa7f-130">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="4fa7f-130">Owned</span></span>  <br/> |<span data-ttu-id="4fa7f-131">ユーザーがフォルダーにユーザーが所有しているアイテムを削除する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="4fa7f-132">All</span><span class="sxs-lookup"><span data-stu-id="4fa7f-132">All</span></span>  <br/> |<span data-ttu-id="4fa7f-133">ユーザーがフォルダー内のすべてのアイテムを削除する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fa7f-134">備考</span><span class="sxs-lookup"><span data-stu-id="4fa7f-134">Remarks</span></span>

<span data-ttu-id="4fa7f-135">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4fa7f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fa7f-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="4fa7f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fa7f-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="4fa7f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fa7f-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4fa7f-138">Schema Name</span></span>  <br/> |<span data-ttu-id="4fa7f-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4fa7f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fa7f-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4fa7f-140">Validation File</span></span>  <br/> |<span data-ttu-id="4fa7f-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fa7f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fa7f-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4fa7f-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fa7f-143">False</span><span class="sxs-lookup"><span data-stu-id="4fa7f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fa7f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="4fa7f-144">See also</span></span>

- [<span data-ttu-id="4fa7f-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4fa7f-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="4fa7f-146">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="4fa7f-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

