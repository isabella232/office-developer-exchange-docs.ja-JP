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
description: FolderIds 要素には、イベント通知のコピー、移動、取得、削除、または監視を行うフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530994"
---
# <a name="folderids"></a><span data-ttu-id="6d66c-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="6d66c-103">FolderIds</span></span>

<span data-ttu-id="6d66c-104">**FolderIds**要素には、イベント通知のコピー、移動、取得、削除、または監視を行うフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d66c-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="6d66c-105">**非 Emptyarrayofbasefolderidstype**</span><span class="sxs-lookup"><span data-stu-id="6d66c-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d66c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6d66c-106">Attributes and elements</span></span>

<span data-ttu-id="6d66c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d66c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d66c-108">Attributes</span></span>

<span data-ttu-id="6d66c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d66c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d66c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d66c-110">Child elements</span></span>

|<span data-ttu-id="6d66c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6d66c-111">**Element**</span></span>|<span data-ttu-id="6d66c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d66c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d66c-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="6d66c-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6d66c-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d66c-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6d66c-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6d66c-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6d66c-116">名前で参照できる Microsoft Exchange Server フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d66c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6d66c-117">Parent elements</span></span>

|<span data-ttu-id="6d66c-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d66c-118">**Element**</span></span>|<span data-ttu-id="6d66c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d66c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d66c-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="6d66c-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="6d66c-121">Exchange ストアからフォルダーを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="6d66c-122">この要素の XPath 式を次に示します。`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="6d66c-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="6d66c-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="6d66c-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="6d66c-124">Exchange ストアからフォルダーを削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="6d66c-125">この要素の XPath 式を次に示します。`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="6d66c-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="6d66c-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="6d66c-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="6d66c-127">Exchange ストアからフォルダーを削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="6d66c-128">この要素の XPath 式を次に示します。`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="6d66c-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="6d66c-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="6d66c-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="6d66c-130">Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="6d66c-131">この要素の XPath 式を次に示します。`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="6d66c-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="6d66c-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="6d66c-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="6d66c-133">Exchange ストア内のフォルダーをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="6d66c-134">この要素の XPath 式を次に示します。`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="6d66c-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="6d66c-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="6d66c-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="6d66c-136">プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="6d66c-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="6d66c-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="6d66c-138">プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="6d66c-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d66c-139">注釈</span><span class="sxs-lookup"><span data-stu-id="6d66c-139">Remarks</span></span>

<span data-ttu-id="6d66c-140">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6d66c-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d66c-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6d66c-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d66c-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d66c-142">Namespace</span></span>  <br/> |<span data-ttu-id="6d66c-143">https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="6d66c-143">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="6d66c-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d66c-144">Schema Name</span></span>  <br/> |<span data-ttu-id="6d66c-145">メッセージスキーマ。Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d66c-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="6d66c-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d66c-146">Validation File</span></span>  <br/> |<span data-ttu-id="6d66c-147">メッセージ .xsd。型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6d66c-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d66c-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d66c-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d66c-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="6d66c-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d66c-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d66c-150">See also</span></span>



[<span data-ttu-id="6d66c-151">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6d66c-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="6d66c-152">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6d66c-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="6d66c-153">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6d66c-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="6d66c-154">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6d66c-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="6d66c-155">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6d66c-155">Subscribe operation</span></span>](subscribe-operation.md)

