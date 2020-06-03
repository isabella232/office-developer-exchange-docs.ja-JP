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
description: DeleteItems 要素は、ユーザーが削除のアクセス許可を持っているフォルダー内のアイテムを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: a0bbefc8b021d047bb2e001669c3e92a6e2536ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454408"
---
# <a name="deleteitems"></a><span data-ttu-id="6c060-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="6c060-104">DeleteItems</span></span>

<span data-ttu-id="6c060-105">**Deleteitems**要素は、ユーザーが削除のアクセス許可を持っているフォルダー内のアイテムを示します。</span><span class="sxs-lookup"><span data-stu-id="6c060-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="6c060-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c060-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="6c060-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="6c060-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c060-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c060-108">Attributes and elements</span></span>

<span data-ttu-id="6c060-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c060-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c060-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c060-110">Attributes</span></span>

<span data-ttu-id="6c060-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c060-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c060-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c060-112">Child elements</span></span>

<span data-ttu-id="6c060-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6c060-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c060-114">親要素</span><span class="sxs-lookup"><span data-stu-id="6c060-114">Parent elements</span></span>

|<span data-ttu-id="6c060-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c060-115">**Element**</span></span>|<span data-ttu-id="6c060-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c060-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c060-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c060-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="6c060-118">ユーザーがフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c060-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="6c060-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c060-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6c060-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="6c060-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="6c060-121">ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c060-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="6c060-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c060-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c060-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c060-123">Text value</span></span>

<span data-ttu-id="6c060-124">次の表に、 **Deleteitems**要素に使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="6c060-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="6c060-125">**DeleteItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="6c060-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="6c060-126">**値**</span><span class="sxs-lookup"><span data-stu-id="6c060-126">**Value**</span></span>|<span data-ttu-id="6c060-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c060-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c060-128">なし</span><span class="sxs-lookup"><span data-stu-id="6c060-128">None</span></span>  <br/> |<span data-ttu-id="6c060-129">ユーザーがフォルダー内のアイテムを削除する権限を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6c060-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="6c060-130">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="6c060-130">Owned</span></span>  <br/> |<span data-ttu-id="6c060-131">ユーザーがフォルダー内で所有するアイテムを削除する権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="6c060-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="6c060-132">すべて</span><span class="sxs-lookup"><span data-stu-id="6c060-132">All</span></span>  <br/> |<span data-ttu-id="6c060-133">ユーザーにフォルダー内のすべてのアイテムを削除する権限があることを示します。</span><span class="sxs-lookup"><span data-stu-id="6c060-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c060-134">注釈</span><span class="sxs-lookup"><span data-stu-id="6c060-134">Remarks</span></span>

<span data-ttu-id="6c060-135">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6c060-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c060-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c060-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c060-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c060-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c060-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c060-138">Schema Name</span></span>  <br/> |<span data-ttu-id="6c060-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c060-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c060-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c060-140">Validation File</span></span>  <br/> |<span data-ttu-id="6c060-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c060-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c060-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c060-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c060-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c060-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c060-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c060-144">See also</span></span>

- [<span data-ttu-id="6c060-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c060-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6c060-146">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="6c060-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

