---
title: Permission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: アクセス許可要素では、フォルダーにユーザーが持つアクセス権を定義します。
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832735"
---
# <a name="permission"></a><span data-ttu-id="9ee2c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ee2c-103">Permission</span></span>

<span data-ttu-id="9ee2c-104">**アクセス許可**要素では、フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="9ee2c-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="9ee2c-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ee2c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ee2c-106">Attributes and elements</span></span>

<span data-ttu-id="9ee2c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ee2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ee2c-108">Attributes</span></span>

<span data-ttu-id="9ee2c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ee2c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ee2c-110">Child elements</span></span>

|<span data-ttu-id="9ee2c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ee2c-111">**Element**</span></span>|<span data-ttu-id="9ee2c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ee2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ee2c-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="9ee2c-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="9ee2c-114">ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="9ee2c-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="9ee2c-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="9ee2c-117">ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="9ee2c-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="9ee2c-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="9ee2c-120">ユーザーがフォルダー内のアイテムを削除する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="9ee2c-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="9ee2c-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="9ee2c-123">ユーザーがフォルダー内のアイテムを編集する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="9ee2c-124">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="9ee2c-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="9ee2c-126">ユーザーがフォルダーの連絡先であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="9ee2c-127">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="9ee2c-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="9ee2c-129">ユーザーがフォルダーの所有者であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="9ee2c-130">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="9ee2c-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="9ee2c-132">ユーザーがフォルダーを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="9ee2c-133">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9ee2c-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="9ee2c-135">フォルダーにユーザーが持つアクセス許可の組み合わせを表します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="9ee2c-136">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="9ee2c-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="9ee2c-138">ユーザーがフォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="9ee2c-139">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9ee2c-140">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="9ee2c-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="9ee2c-141">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="9ee2c-142">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ee2c-143">親要素</span><span class="sxs-lookup"><span data-stu-id="9ee2c-143">Parent elements</span></span>

|<span data-ttu-id="9ee2c-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ee2c-144">**Element**</span></span>|<span data-ttu-id="9ee2c-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ee2c-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ee2c-146">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ee2c-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="9ee2c-147">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="9ee2c-148">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ee2c-149">備考</span><span class="sxs-lookup"><span data-stu-id="9ee2c-149">Remarks</span></span>

<span data-ttu-id="9ee2c-150">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="9ee2c-151">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="9ee2c-152">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="9ee2c-152">Version differences</span></span>

<span data-ttu-id="9ee2c-153">アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="9ee2c-154">フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="9ee2c-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9ee2c-155">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ee2c-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ee2c-156">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ee2c-156">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ee2c-157">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ee2c-157">Schema Name</span></span>  <br/> |<span data-ttu-id="9ee2c-158">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9ee2c-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ee2c-159">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ee2c-159">Validation File</span></span>  <br/> |<span data-ttu-id="9ee2c-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ee2c-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ee2c-161">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ee2c-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ee2c-162">False</span><span class="sxs-lookup"><span data-stu-id="9ee2c-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ee2c-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ee2c-163">See also</span></span>



- [<span data-ttu-id="9ee2c-164">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ee2c-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9ee2c-165">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="9ee2c-165">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

