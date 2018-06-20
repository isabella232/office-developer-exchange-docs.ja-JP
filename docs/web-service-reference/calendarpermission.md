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
description: CalendarPermission 要素は、予定表フォルダーにユーザーが持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759591"
---
# <a name="calendarpermission"></a><span data-ttu-id="f5b04-104">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="f5b04-104">CalendarPermission</span></span>

<span data-ttu-id="f5b04-105">**CalendarPermission**要素は、予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="f5b04-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="f5b04-107">**CalendarPermissionType**</span><span class="sxs-lookup"><span data-stu-id="f5b04-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5b04-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f5b04-108">Attributes and elements</span></span>

<span data-ttu-id="f5b04-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5b04-110">属性</span><span class="sxs-lookup"><span data-stu-id="f5b04-110">Attributes</span></span>

<span data-ttu-id="f5b04-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f5b04-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5b04-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f5b04-112">Child elements</span></span>

|<span data-ttu-id="f5b04-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5b04-113">**Element**</span></span>|<span data-ttu-id="f5b04-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5b04-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5b04-115">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="f5b04-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="f5b04-116">ユーザーが予定表フォルダーに必要なアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="f5b04-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-118">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="f5b04-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="f5b04-119">ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="f5b04-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-121">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="f5b04-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="f5b04-122">ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="f5b04-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-124">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="f5b04-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="f5b04-125">ユーザーがフォルダー内のアイテムを削除する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="f5b04-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-127">EditItems</span><span class="sxs-lookup"><span data-stu-id="f5b04-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="f5b04-128">ユーザーがフォルダー内のアイテムを編集する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="f5b04-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-130">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="f5b04-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="f5b04-131">ユーザーがフォルダーの連絡先であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="f5b04-132">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-133">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="f5b04-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="f5b04-134">ユーザーがフォルダーの所有者であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="f5b04-135">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-136">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="f5b04-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="f5b04-137">ユーザーがフォルダーを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="f5b04-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-139">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="f5b04-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="f5b04-140">ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="f5b04-141">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f5b04-142">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="f5b04-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="f5b04-143">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f5b04-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="f5b04-144">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5b04-145">親要素</span><span class="sxs-lookup"><span data-stu-id="f5b04-145">Parent elements</span></span>

|<span data-ttu-id="f5b04-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5b04-146">**Element**</span></span>|<span data-ttu-id="f5b04-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5b04-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5b04-148">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="f5b04-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="f5b04-149">フォルダーのアクセス許可を予定表の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f5b04-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="f5b04-150">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5b04-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5b04-151">備考</span><span class="sxs-lookup"><span data-stu-id="f5b04-151">Remarks</span></span>

<span data-ttu-id="f5b04-152">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f5b04-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5b04-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="f5b04-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5b04-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="f5b04-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5b04-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f5b04-155">Schema Name</span></span>  <br/> |<span data-ttu-id="f5b04-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f5b04-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5b04-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f5b04-157">Validation File</span></span>  <br/> |<span data-ttu-id="f5b04-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f5b04-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5b04-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f5b04-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5b04-160">False</span><span class="sxs-lookup"><span data-stu-id="f5b04-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5b04-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5b04-161">See also</span></span>



- [<span data-ttu-id="f5b04-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f5b04-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f5b04-163">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="f5b04-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

