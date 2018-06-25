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
description: SearchFolder の要素は、メールボックスに格納されている検索フォルダーを表します。
ms.openlocfilehash: d842c54dab7950c68e26804b676834c2d95debad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833302"
---
# <a name="searchfolder"></a><span data-ttu-id="f0f1e-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f0f1e-103">SearchFolder</span></span>

<span data-ttu-id="f0f1e-104">**SearchFolder**の要素は、メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="f0f1e-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="f0f1e-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0f1e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f0f1e-106">Attributes and elements</span></span>

<span data-ttu-id="f0f1e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0f1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0f1e-108">Attributes</span></span>

<span data-ttu-id="f0f1e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0f1e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0f1e-110">Child elements</span></span>

|<span data-ttu-id="f0f1e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0f1e-111">**Element**</span></span>|<span data-ttu-id="f0f1e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0f1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f1e-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="f0f1e-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="f0f1e-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f0f1e-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="f0f1e-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="f0f1e-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="f0f1e-118">指定されたフォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-119">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="f0f1e-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="f0f1e-120">フォルダーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="f0f1e-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="f0f1e-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="f0f1e-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="f0f1e-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="f0f1e-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f0f1e-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="f0f1e-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="f0f1e-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="f0f1e-129">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="f0f1e-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="f0f1e-131">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="f0f1e-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="f0f1e-133">検索フォルダーを定義するパラメーターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f0f1e-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="f0f1e-135">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="f0f1e-136">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="f0f1e-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="f0f1e-138">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="f0f1e-139">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-139">This element is read-only.</span></span> <span data-ttu-id="f0f1e-140">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0f1e-141">親要素</span><span class="sxs-lookup"><span data-stu-id="f0f1e-141">Parent elements</span></span>

|<span data-ttu-id="f0f1e-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0f1e-142">**Element**</span></span>|<span data-ttu-id="f0f1e-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0f1e-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f1e-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="f0f1e-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="f0f1e-145">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-146">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="f0f1e-147">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-148">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="f0f1e-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="f0f1e-149">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-150">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="f0f1e-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="f0f1e-151">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f0f1e-152">フォルダー</span><span class="sxs-lookup"><span data-stu-id="f0f1e-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f0f1e-153">フォルダーの操作に使用するフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0f1e-154">備考</span><span class="sxs-lookup"><span data-stu-id="f0f1e-154">Remarks</span></span>

 <span data-ttu-id="f0f1e-155">**SearchFolder**を使用して通常の検索フォルダーと MicrosoftOfficeOutlook と Outlook Web Access の表示の両方のフォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="f0f1e-156">Outlook と Outlook Web Access に表示する検索フォルダーを使用して識別されたフォルダーの下にあるフォルダーを作成しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="f0f1e-157">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f0f1e-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0f1e-158">要素情報</span><span class="sxs-lookup"><span data-stu-id="f0f1e-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0f1e-159">名前空間</span><span class="sxs-lookup"><span data-stu-id="f0f1e-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0f1e-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0f1e-160">Schema Name</span></span>  <br/> |<span data-ttu-id="f0f1e-161">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f0f1e-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0f1e-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0f1e-162">Validation File</span></span>  <br/> |<span data-ttu-id="f0f1e-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f0f1e-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0f1e-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0f1e-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0f1e-165">False</span><span class="sxs-lookup"><span data-stu-id="f0f1e-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0f1e-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0f1e-166">See also</span></span>



- [<span data-ttu-id="f0f1e-167">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0f1e-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

