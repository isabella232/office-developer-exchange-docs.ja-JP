---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: SearchFolder 要素は、メールボックスに格納されている検索フォルダーを表します。
ms.openlocfilehash: e1d5893e00f3b199451622061785e2566c6f32e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464008"
---
# <a name="searchfolder"></a><span data-ttu-id="d8d4d-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d8d4d-103">SearchFolder</span></span>

<span data-ttu-id="d8d4d-104">**Searchfolder**要素は、メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 <span data-ttu-id="d8d4d-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="d8d4d-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8d4d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d8d4d-106">Attributes and elements</span></span>

<span data-ttu-id="d8d4d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8d4d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8d4d-108">Attributes</span></span>

<span data-ttu-id="d8d4d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8d4d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d8d4d-110">Child elements</span></span>

|<span data-ttu-id="d8d4d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d8d4d-111">**Element**</span></span>|<span data-ttu-id="d8d4d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8d4d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8d4d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="d8d4d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d8d4d-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d8d4d-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d8d4d-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="d8d4d-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="d8d4d-118">指定したフォルダーのフォルダークラスを表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-119">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="d8d4d-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="d8d4d-120">フォルダーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d8d4d-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="d8d4d-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="d8d4d-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="d8d4d-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="d8d4d-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d8d4d-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="d8d4d-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="d8d4d-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="d8d4d-129">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="d8d4d-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="d8d4d-131">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="d8d4d-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="d8d4d-133">検索フォルダーを定義するパラメーターを含みます。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="d8d4d-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="d8d4d-135">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="d8d4d-136">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="d8d4d-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="d8d4d-138">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="d8d4d-139">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-139">This element is read-only.</span></span> <span data-ttu-id="d8d4d-140">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8d4d-141">親要素</span><span class="sxs-lookup"><span data-stu-id="d8d4d-141">Parent elements</span></span>

|<span data-ttu-id="d8d4d-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8d4d-142">**Element**</span></span>|<span data-ttu-id="d8d4d-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8d4d-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8d4d-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="d8d4d-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="d8d4d-145">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-146">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d8d4d-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="d8d4d-147">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-148">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="d8d4d-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="d8d4d-149">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-150">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d8d4d-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="d8d4d-151">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="d8d4d-152">フォルダー</span><span class="sxs-lookup"><span data-stu-id="d8d4d-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d8d4d-153">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8d4d-154">注釈</span><span class="sxs-lookup"><span data-stu-id="d8d4d-154">Remarks</span></span>

 <span data-ttu-id="d8d4d-155">**Searchfolder**は、通常の検索フォルダーと Microsoft office outlook および Outlook Web Access の表示可能な検索フォルダーの両方に使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="d8d4d-156">検索フォルダーが Outlook および Outlook Web Access に表示されるようにするには、SearchFolders 識別フォルダーの下にフォルダーを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="d8d4d-157">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d8d4d-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8d4d-158">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d8d4d-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8d4d-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8d4d-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8d4d-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8d4d-160">Schema Name</span></span>  <br/> |<span data-ttu-id="d8d4d-161">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d8d4d-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8d4d-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8d4d-162">Validation File</span></span>  <br/> |<span data-ttu-id="d8d4d-163">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d8d4d-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8d4d-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d8d4d-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8d4d-165">正しくない</span><span class="sxs-lookup"><span data-stu-id="d8d4d-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8d4d-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8d4d-166">See also</span></span>



- [<span data-ttu-id="d8d4d-167">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d8d4d-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

