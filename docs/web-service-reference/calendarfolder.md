---
title: CalendarFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolder
api_type:
- schema
ms.assetid: 48687a78-e757-4c04-9641-bf4302c6b565
description: CalendarFolder 要素は、主に予定表アイテムを含むフォルダーを表します。
ms.openlocfilehash: dcd0ab9d7dea1152766997de0618b3dcceed5567
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461493"
---
# <a name="calendarfolder"></a><span data-ttu-id="cc2db-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="cc2db-103">CalendarFolder</span></span>

<span data-ttu-id="cc2db-104">**Calendarfolder**要素は、主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
```xml
<CalendarFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</CalendarFolder>
```

 <span data-ttu-id="cc2db-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="cc2db-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc2db-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc2db-106">Attributes and elements</span></span>

<span data-ttu-id="cc2db-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc2db-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc2db-108">Attributes</span></span>

<span data-ttu-id="cc2db-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc2db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc2db-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc2db-110">Child elements</span></span>

|<span data-ttu-id="cc2db-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="cc2db-111">**Element**</span></span>|<span data-ttu-id="cc2db-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc2db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc2db-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="cc2db-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="cc2db-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc2db-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="cc2db-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="cc2db-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="cc2db-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="cc2db-118">指定したフォルダーのフォルダークラスを表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-119">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="cc2db-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="cc2db-120">フォルダーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="cc2db-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="cc2db-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="cc2db-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="cc2db-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="cc2db-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="cc2db-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="cc2db-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="cc2db-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="cc2db-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="cc2db-129">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="cc2db-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="cc2db-131">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc2db-131">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="cc2db-132">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cc2db-132">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="cc2db-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="cc2db-134">共有されている予定表データに対してユーザーが持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="cc2db-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="cc2db-136">予定表フォルダーに対して構成されているアクセス許可がすべて含まれます。</span><span class="sxs-lookup"><span data-stu-id="cc2db-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc2db-137">親要素</span><span class="sxs-lookup"><span data-stu-id="cc2db-137">Parent elements</span></span>

|<span data-ttu-id="cc2db-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc2db-138">**Element**</span></span>|<span data-ttu-id="cc2db-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc2db-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc2db-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="cc2db-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="cc2db-141">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="cc2db-142">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="cc2db-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="cc2db-143">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="cc2db-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="cc2db-145">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="cc2db-146">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="cc2db-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="cc2db-147">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="cc2db-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="cc2db-148">フォルダー</span><span class="sxs-lookup"><span data-stu-id="cc2db-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cc2db-149">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc2db-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc2db-150">注釈</span><span class="sxs-lookup"><span data-stu-id="cc2db-150">Remarks</span></span>

<span data-ttu-id="cc2db-151">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc2db-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc2db-152">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cc2db-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc2db-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc2db-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc2db-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc2db-154">Schema Name</span></span>  <br/> |<span data-ttu-id="cc2db-155">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cc2db-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc2db-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc2db-156">Validation File</span></span>  <br/> |<span data-ttu-id="cc2db-157">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cc2db-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc2db-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cc2db-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc2db-159">正しくない</span><span class="sxs-lookup"><span data-stu-id="cc2db-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc2db-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc2db-160">See also</span></span>



- [<span data-ttu-id="cc2db-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc2db-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

