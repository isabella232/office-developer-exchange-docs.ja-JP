---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: PermissionLevel 要素は、ユーザーがフォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458041"
---
# <a name="permissionlevel"></a><span data-ttu-id="81e17-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="81e17-104">PermissionLevel</span></span>

<span data-ttu-id="81e17-105">**Permissionlevel**要素は、ユーザーがフォルダーに対して持っているアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="81e17-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="81e17-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="81e17-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="81e17-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="81e17-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81e17-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="81e17-108">Attributes and elements</span></span>

<span data-ttu-id="81e17-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="81e17-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81e17-110">属性</span><span class="sxs-lookup"><span data-stu-id="81e17-110">Attributes</span></span>

<span data-ttu-id="81e17-111">なし。</span><span class="sxs-lookup"><span data-stu-id="81e17-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81e17-112">子要素</span><span class="sxs-lookup"><span data-stu-id="81e17-112">Child elements</span></span>

<span data-ttu-id="81e17-113">なし。</span><span class="sxs-lookup"><span data-stu-id="81e17-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81e17-114">親要素</span><span class="sxs-lookup"><span data-stu-id="81e17-114">Parent elements</span></span>

|<span data-ttu-id="81e17-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="81e17-115">**Element**</span></span>|<span data-ttu-id="81e17-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="81e17-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81e17-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81e17-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="81e17-118">ユーザーがフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="81e17-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="81e17-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="81e17-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="81e17-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="81e17-120">Text value</span></span>

<span data-ttu-id="81e17-121">次の表に、 **Permissionlevel**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="81e17-122">**PermissionLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="81e17-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="81e17-123">**値**</span><span class="sxs-lookup"><span data-stu-id="81e17-123">**Value**</span></span>|<span data-ttu-id="81e17-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="81e17-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="81e17-125">なし</span><span class="sxs-lookup"><span data-stu-id="81e17-125">None</span></span>  <br/> |<span data-ttu-id="81e17-126">ユーザーがフォルダーに対するアクセス許可を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="81e17-127">Owner</span><span class="sxs-lookup"><span data-stu-id="81e17-127">Owner</span></span>  <br/> |<span data-ttu-id="81e17-128">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="81e17-129">ユーザーはフォルダーの所有者とフォルダーの両方の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="81e17-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="81e17-130">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="81e17-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="81e17-131">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="81e17-132">エディター</span><span class="sxs-lookup"><span data-stu-id="81e17-132">Editor</span></span>  <br/> |<span data-ttu-id="81e17-133">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="81e17-134">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="81e17-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="81e17-135">ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを編集および削除し、サブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="81e17-136">設定元</span><span class="sxs-lookup"><span data-stu-id="81e17-136">Author</span></span>  <br/> |<span data-ttu-id="81e17-137">ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを編集および削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="81e17-138">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="81e17-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="81e17-139">ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="81e17-140">レビュー担当者</span><span class="sxs-lookup"><span data-stu-id="81e17-140">Reviewer</span></span>  <br/> |<span data-ttu-id="81e17-141">ユーザーがフォルダー内のすべてのアイテムを読み取ることができることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="81e17-142">共同作成者</span><span class="sxs-lookup"><span data-stu-id="81e17-142">Contributor</span></span>  <br/> |<span data-ttu-id="81e17-143">ユーザーがフォルダー内にアイテムを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="81e17-144">フォルダーの内容は表示されません。</span><span class="sxs-lookup"><span data-stu-id="81e17-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="81e17-145">Custom</span><span class="sxs-lookup"><span data-stu-id="81e17-145">Custom</span></span>  <br/> |<span data-ttu-id="81e17-146">ユーザーがフォルダーに対して独自のアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="81e17-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81e17-147">注釈</span><span class="sxs-lookup"><span data-stu-id="81e17-147">Remarks</span></span>

<span data-ttu-id="81e17-148">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="81e17-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81e17-149">要素の情報</span><span class="sxs-lookup"><span data-stu-id="81e17-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81e17-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="81e17-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81e17-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="81e17-151">Schema Name</span></span>  <br/> |<span data-ttu-id="81e17-152">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="81e17-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="81e17-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="81e17-153">Validation File</span></span>  <br/> |<span data-ttu-id="81e17-154">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="81e17-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81e17-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="81e17-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="81e17-156">正しくない</span><span class="sxs-lookup"><span data-stu-id="81e17-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81e17-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="81e17-157">See also</span></span>



- [<span data-ttu-id="81e17-158">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="81e17-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="81e17-159">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="81e17-159">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

