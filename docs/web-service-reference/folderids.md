---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: FolderIds 要素には、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760565"
---
# <a name="folderids"></a><span data-ttu-id="74dfe-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="74dfe-103">FolderIds</span></span>

<span data-ttu-id="74dfe-104">**FolderIds**要素には、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74dfe-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="74dfe-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="74dfe-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74dfe-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="74dfe-106">Attributes and elements</span></span>

<span data-ttu-id="74dfe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74dfe-108">属性</span><span class="sxs-lookup"><span data-stu-id="74dfe-108">Attributes</span></span>

<span data-ttu-id="74dfe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74dfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74dfe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74dfe-110">Child elements</span></span>

|<span data-ttu-id="74dfe-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="74dfe-111">**Element**</span></span>|<span data-ttu-id="74dfe-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74dfe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74dfe-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="74dfe-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="74dfe-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="74dfe-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="74dfe-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="74dfe-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="74dfe-116">名前で参照できる Microsoft Exchange Server のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74dfe-117">親要素</span><span class="sxs-lookup"><span data-stu-id="74dfe-117">Parent elements</span></span>

|<span data-ttu-id="74dfe-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="74dfe-118">**Element**</span></span>|<span data-ttu-id="74dfe-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="74dfe-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74dfe-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="74dfe-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="74dfe-121">Exchange ストアからフォルダーを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="74dfe-122">この要素への XPath 式は、次のようにします。`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="74dfe-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="74dfe-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="74dfe-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="74dfe-124">Exchange ストアからフォルダーを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="74dfe-125">この要素への XPath 式は、次のようにします。`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="74dfe-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="74dfe-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="74dfe-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="74dfe-127">Exchange ストアからフォルダーを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="74dfe-128">この要素への XPath 式は、次のようにします。`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="74dfe-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="74dfe-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="74dfe-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="74dfe-130">Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="74dfe-131">この要素への XPath 式は、次のようにします。`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="74dfe-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="74dfe-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="74dfe-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="74dfe-133">Exchange ストア内のフォルダーをコピーするのには要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="74dfe-134">この要素への XPath 式は、次のようにします。`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="74dfe-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="74dfe-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="74dfe-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="74dfe-136">プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="74dfe-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="74dfe-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="74dfe-138">プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="74dfe-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74dfe-139">備考</span><span class="sxs-lookup"><span data-stu-id="74dfe-139">Remarks</span></span>

<span data-ttu-id="74dfe-140">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="74dfe-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74dfe-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="74dfe-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74dfe-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="74dfe-142">Namespace</span></span>  <br/> |<span data-ttu-id="74dfe-143">http://schemas.microsoft.com/exchange/services/2006/messages と http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="74dfe-143">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="74dfe-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74dfe-144">Schema Name</span></span>  <br/> |<span data-ttu-id="74dfe-145">メッセージ スキーマです。タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="74dfe-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="74dfe-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74dfe-146">Validation File</span></span>  <br/> |<span data-ttu-id="74dfe-147">Messages.xsd です。Types.xsd</span><span class="sxs-lookup"><span data-stu-id="74dfe-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74dfe-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74dfe-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="74dfe-149">False</span><span class="sxs-lookup"><span data-stu-id="74dfe-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74dfe-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="74dfe-150">See also</span></span>



<span data-ttu-id="74dfe-151">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="74dfe-151">[GetFolder operation](getfolder-operation.md)</span></span>
  
[<span data-ttu-id="74dfe-152">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="74dfe-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="74dfe-153">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="74dfe-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="74dfe-154">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="74dfe-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="74dfe-155">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="74dfe-155">Subscribe operation</span></span>](subscribe-operation.md)

