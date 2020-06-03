---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: CalendarPermission 要素は、ユーザーが予定表フォルダーに対して持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: c43f75e6cf5abc2dce9af6c04122ec9a589dcd58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529477"
---
# <a name="calendarpermission"></a><span data-ttu-id="295d5-104">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="295d5-104">CalendarPermission</span></span>

<span data-ttu-id="295d5-105">**Calendarpermission**要素は、ユーザーが予定表フォルダーに対して持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="295d5-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="295d5-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="295d5-107">**CalendarPermissionType**</span><span class="sxs-lookup"><span data-stu-id="295d5-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="295d5-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="295d5-108">Attributes and elements</span></span>

<span data-ttu-id="295d5-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="295d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="295d5-110">属性</span><span class="sxs-lookup"><span data-stu-id="295d5-110">Attributes</span></span>

<span data-ttu-id="295d5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="295d5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="295d5-112">子要素</span><span class="sxs-lookup"><span data-stu-id="295d5-112">Child elements</span></span>

|<span data-ttu-id="295d5-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="295d5-113">**Element**</span></span>|<span data-ttu-id="295d5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="295d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="295d5-115">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="295d5-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="295d5-116">ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="295d5-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="295d5-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-118">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="295d5-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="295d5-119">ユーザーがフォルダーにアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="295d5-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-121">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="295d5-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="295d5-122">ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="295d5-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-124">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="295d5-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="295d5-125">ユーザーにフォルダー内のアイテムを削除する権限があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="295d5-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-127">EditItems</span><span class="sxs-lookup"><span data-stu-id="295d5-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="295d5-128">ユーザーにフォルダー内のアイテムを編集する権限があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="295d5-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-130">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="295d5-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="295d5-131">ユーザーがフォルダーの連絡先であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="295d5-132">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-133">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="295d5-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="295d5-134">ユーザーがフォルダーの所有者であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="295d5-135">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-136">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="295d5-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="295d5-137">ユーザーがフォルダーを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="295d5-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-139">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="295d5-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="295d5-140">ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="295d5-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="295d5-141">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="295d5-142">UserId</span><span class="sxs-lookup"><span data-stu-id="295d5-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="295d5-143">代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="295d5-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="295d5-144">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="295d5-145">親要素</span><span class="sxs-lookup"><span data-stu-id="295d5-145">Parent elements</span></span>

|<span data-ttu-id="295d5-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="295d5-146">**Element**</span></span>|<span data-ttu-id="295d5-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="295d5-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="295d5-148">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="295d5-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="295d5-149">フォルダーに対する予定表のアクセス許可の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="295d5-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="295d5-150">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="295d5-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="295d5-151">注釈</span><span class="sxs-lookup"><span data-stu-id="295d5-151">Remarks</span></span>

<span data-ttu-id="295d5-152">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="295d5-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="295d5-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="295d5-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="295d5-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="295d5-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="295d5-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="295d5-155">Schema Name</span></span>  <br/> |<span data-ttu-id="295d5-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="295d5-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="295d5-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="295d5-157">Validation File</span></span>  <br/> |<span data-ttu-id="295d5-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="295d5-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="295d5-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="295d5-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="295d5-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="295d5-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="295d5-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="295d5-161">See also</span></span>



- [<span data-ttu-id="295d5-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="295d5-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="295d5-163">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="295d5-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

