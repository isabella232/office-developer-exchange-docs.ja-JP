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
description: CalendarFolder 要素は、主に予定表のアイテムを含むフォルダーを表します。
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759583"
---
# <a name="calendarfolder"></a><span data-ttu-id="754e0-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="754e0-103">CalendarFolder</span></span>

<span data-ttu-id="754e0-104">**CalendarFolder**要素は、主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
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

 <span data-ttu-id="754e0-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="754e0-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="754e0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="754e0-106">Attributes and elements</span></span>

<span data-ttu-id="754e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="754e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="754e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="754e0-108">Attributes</span></span>

<span data-ttu-id="754e0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="754e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="754e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="754e0-110">Child elements</span></span>

|<span data-ttu-id="754e0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="754e0-111">**Element**</span></span>|<span data-ttu-id="754e0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="754e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="754e0-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="754e0-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="754e0-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="754e0-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="754e0-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="754e0-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="754e0-118">指定されたフォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-119">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="754e0-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="754e0-120">フォルダーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="754e0-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="754e0-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="754e0-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="754e0-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="754e0-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="754e0-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="754e0-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="754e0-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="754e0-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="754e0-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="754e0-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="754e0-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="754e0-129">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="754e0-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="754e0-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="754e0-131">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-131">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="754e0-132">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="754e0-132">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="754e0-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="754e0-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="754e0-134">ユーザーが共有されている予定表データを持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="754e0-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="754e0-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="754e0-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="754e0-136">予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="754e0-137">親要素</span><span class="sxs-lookup"><span data-stu-id="754e0-137">Parent elements</span></span>

|<span data-ttu-id="754e0-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="754e0-138">**Element**</span></span>|<span data-ttu-id="754e0-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="754e0-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="754e0-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="754e0-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="754e0-141">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="754e0-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="754e0-142">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="754e0-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="754e0-143">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="754e0-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="754e0-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="754e0-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="754e0-145">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="754e0-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="754e0-146">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="754e0-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="754e0-147">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="754e0-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="754e0-148">フォルダー</span><span class="sxs-lookup"><span data-stu-id="754e0-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="754e0-149">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="754e0-150">備考</span><span class="sxs-lookup"><span data-stu-id="754e0-150">Remarks</span></span>

<span data-ttu-id="754e0-151">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="754e0-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="754e0-152">要素情報</span><span class="sxs-lookup"><span data-stu-id="754e0-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="754e0-153">名前空間</span><span class="sxs-lookup"><span data-stu-id="754e0-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="754e0-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="754e0-154">Schema Name</span></span>  <br/> |<span data-ttu-id="754e0-155">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="754e0-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="754e0-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="754e0-156">Validation File</span></span>  <br/> |<span data-ttu-id="754e0-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="754e0-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="754e0-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="754e0-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="754e0-159">False</span><span class="sxs-lookup"><span data-stu-id="754e0-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="754e0-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="754e0-160">See also</span></span>



- [<span data-ttu-id="754e0-161">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="754e0-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

