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
description: PermissionLevel 要素は、ユーザーがフォルダーに必要なアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832730"
---
# <a name="permissionlevel"></a><span data-ttu-id="45955-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="45955-104">PermissionLevel</span></span>

<span data-ttu-id="45955-105">**PermissionLevel**要素は、ユーザーがフォルダーに必要なアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="45955-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="45955-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="45955-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="45955-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="45955-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45955-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45955-108">Attributes and elements</span></span>

<span data-ttu-id="45955-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45955-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45955-110">属性</span><span class="sxs-lookup"><span data-stu-id="45955-110">Attributes</span></span>

<span data-ttu-id="45955-111">なし。</span><span class="sxs-lookup"><span data-stu-id="45955-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45955-112">子要素</span><span class="sxs-lookup"><span data-stu-id="45955-112">Child elements</span></span>

<span data-ttu-id="45955-113">なし。</span><span class="sxs-lookup"><span data-stu-id="45955-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="45955-114">親要素</span><span class="sxs-lookup"><span data-stu-id="45955-114">Parent elements</span></span>

|<span data-ttu-id="45955-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="45955-115">**Element**</span></span>|<span data-ttu-id="45955-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="45955-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45955-117">Permission</span><span class="sxs-lookup"><span data-stu-id="45955-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="45955-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="45955-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="45955-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="45955-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45955-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45955-120">Text value</span></span>

<span data-ttu-id="45955-121">次の表は、 **PermissionLevel**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="45955-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="45955-122">**PermissionLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="45955-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="45955-123">**値**</span><span class="sxs-lookup"><span data-stu-id="45955-123">**Value**</span></span>|<span data-ttu-id="45955-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="45955-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45955-125">なし</span><span class="sxs-lookup"><span data-stu-id="45955-125">None</span></span>  <br/> |<span data-ttu-id="45955-126">そのユーザーの権限を持ってフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="45955-127">Owner</span><span class="sxs-lookup"><span data-stu-id="45955-127">Owner</span></span>  <br/> |<span data-ttu-id="45955-128">ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="45955-129">ユーザーは、フォルダーの所有者とフォルダーの連絡先の両方です。</span><span class="sxs-lookup"><span data-stu-id="45955-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="45955-130">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="45955-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="45955-131">ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="45955-132">Editor</span><span class="sxs-lookup"><span data-stu-id="45955-132">Editor</span></span>  <br/> |<span data-ttu-id="45955-133">ユーザーが作成、読み取り、編集、およびフォルダー内のすべてのアイテムを削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="45955-134">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="45955-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="45955-135">ユーザーを作成し、フォルダー内のすべてのアイテム編集しユーザーを作成するアイテムのみを削除し、ことサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="45955-136">作成者</span><span class="sxs-lookup"><span data-stu-id="45955-136">Author</span></span>  <br/> |<span data-ttu-id="45955-137">ユーザーを作成し、フォルダー内のすべてのアイテムし編集および削除できますユーザーが作成したアイテムのみを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="45955-138">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="45955-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="45955-139">ユーザーを作成し、フォルダー内のすべてのアイテムを読み取るし、ことユーザーが作成したアイテムのみを削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="45955-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="45955-140">Reviewer</span></span>  <br/> |<span data-ttu-id="45955-141">ユーザーがフォルダー内のすべてのアイテムを読み取ることができますを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="45955-142">Contributor</span><span class="sxs-lookup"><span data-stu-id="45955-142">Contributor</span></span>  <br/> |<span data-ttu-id="45955-143">ユーザーがフォルダーにアイテムを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="45955-144">フォルダーの内容は表示されません。</span><span class="sxs-lookup"><span data-stu-id="45955-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="45955-145">カスタム</span><span class="sxs-lookup"><span data-stu-id="45955-145">Custom</span></span>  <br/> |<span data-ttu-id="45955-146">ユーザーがフォルダーのカスタム アクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="45955-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="45955-147">備考</span><span class="sxs-lookup"><span data-stu-id="45955-147">Remarks</span></span>

<span data-ttu-id="45955-148">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="45955-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45955-149">要素情報</span><span class="sxs-lookup"><span data-stu-id="45955-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45955-150">名前空間</span><span class="sxs-lookup"><span data-stu-id="45955-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="45955-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45955-151">Schema Name</span></span>  <br/> |<span data-ttu-id="45955-152">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="45955-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="45955-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45955-153">Validation File</span></span>  <br/> |<span data-ttu-id="45955-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="45955-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="45955-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45955-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="45955-156">False</span><span class="sxs-lookup"><span data-stu-id="45955-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45955-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="45955-157">See also</span></span>



- [<span data-ttu-id="45955-158">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45955-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="45955-159">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="45955-159">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

