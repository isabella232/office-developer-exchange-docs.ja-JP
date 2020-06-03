---
title: アクセス許可
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
description: Permission 要素は、ユーザーがフォルダーに対して持つアクセス許可を定義します。
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459259"
---
# <a name="permission"></a><span data-ttu-id="e74ea-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e74ea-103">Permission</span></span>

<span data-ttu-id="e74ea-104">Permission 要素は、ユーザーがフォルダーに対して持つアクセス**許可**を定義します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
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

 <span data-ttu-id="e74ea-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="e74ea-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e74ea-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e74ea-106">Attributes and elements</span></span>

<span data-ttu-id="e74ea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e74ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="e74ea-108">Attributes</span></span>

<span data-ttu-id="e74ea-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e74ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e74ea-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e74ea-110">Child elements</span></span>

|<span data-ttu-id="e74ea-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e74ea-111">**Element**</span></span>|<span data-ttu-id="e74ea-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e74ea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e74ea-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="e74ea-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="e74ea-114">ユーザーがフォルダーにアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="e74ea-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="e74ea-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="e74ea-117">ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="e74ea-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="e74ea-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="e74ea-120">ユーザーにフォルダー内のアイテムを削除する権限があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="e74ea-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="e74ea-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="e74ea-123">ユーザーにフォルダー内のアイテムを編集する権限があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="e74ea-124">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="e74ea-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="e74ea-126">ユーザーがフォルダーの連絡先であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="e74ea-127">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="e74ea-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="e74ea-129">ユーザーがフォルダーの所有者であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="e74ea-130">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="e74ea-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="e74ea-132">ユーザーがフォルダーを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="e74ea-133">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="e74ea-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="e74ea-135">ユーザーがフォルダーに対して持っているアクセス許可の組み合わせを表します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="e74ea-136">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="e74ea-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="e74ea-138">ユーザーがフォルダー内のアイテムを読み取る権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="e74ea-139">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e74ea-140">UserId</span><span class="sxs-lookup"><span data-stu-id="e74ea-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="e74ea-141">代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="e74ea-142">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e74ea-143">親要素</span><span class="sxs-lookup"><span data-stu-id="e74ea-143">Parent elements</span></span>

|<span data-ttu-id="e74ea-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="e74ea-144">**Element**</span></span>|<span data-ttu-id="e74ea-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="e74ea-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e74ea-146">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e74ea-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="e74ea-147">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e74ea-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="e74ea-148">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e74ea-149">注釈</span><span class="sxs-lookup"><span data-stu-id="e74ea-149">Remarks</span></span>

<span data-ttu-id="e74ea-150">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e74ea-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e74ea-151">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e74ea-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="e74ea-152">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="e74ea-152">Version differences</span></span>

<span data-ttu-id="e74ea-153">Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。</span><span class="sxs-lookup"><span data-stu-id="e74ea-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="e74ea-154">フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="e74ea-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e74ea-155">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e74ea-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e74ea-156">Namespace</span><span class="sxs-lookup"><span data-stu-id="e74ea-156">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e74ea-157">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e74ea-157">Schema Name</span></span>  <br/> |<span data-ttu-id="e74ea-158">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e74ea-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="e74ea-159">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e74ea-159">Validation File</span></span>  <br/> |<span data-ttu-id="e74ea-160">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e74ea-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e74ea-161">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e74ea-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="e74ea-162">正しくない</span><span class="sxs-lookup"><span data-stu-id="e74ea-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e74ea-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="e74ea-163">See also</span></span>



- [<span data-ttu-id="e74ea-164">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e74ea-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e74ea-165">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="e74ea-165">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

