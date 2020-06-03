---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: SyncFolderItems 要素は、Exchange ストアフォルダー内のアイテムを同期する要求を定義します。
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465150"
---
# <a name="syncfolderitems"></a><span data-ttu-id="1a05f-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1a05f-103">SyncFolderItems</span></span>

<span data-ttu-id="1a05f-104">**Syncfolderitems**要素は、Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="1a05f-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="1a05f-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a05f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1a05f-106">Attributes and elements</span></span>

<span data-ttu-id="1a05f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a05f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a05f-108">Attributes</span></span>

<span data-ttu-id="1a05f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a05f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a05f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a05f-110">Child elements</span></span>

|<span data-ttu-id="1a05f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1a05f-111">**Element**</span></span>|<span data-ttu-id="1a05f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a05f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a05f-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="1a05f-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="1a05f-114">SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="1a05f-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1a05f-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1a05f-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="1a05f-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="1a05f-117">同期するアイテムを含むフォルダを表します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="1a05f-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1a05f-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1a05f-119">SyncState</span><span class="sxs-lookup"><span data-stu-id="1a05f-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1a05f-120">要求が成功するたびに更新される同期データの base64 でエンコードされた形式が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="1a05f-121">これは、同期状態を識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="1a05f-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1a05f-123">無視</span><span class="sxs-lookup"><span data-stu-id="1a05f-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="1a05f-124">同期中にスキップするアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="1a05f-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1a05f-126">Maxの戻り値</span><span class="sxs-lookup"><span data-stu-id="1a05f-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="1a05f-127">同期応答で返すことができる変更の最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="1a05f-128">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1a05f-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1a05f-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="1a05f-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="1a05f-130">同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1a05f-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="1a05f-131">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a05f-132">親要素</span><span class="sxs-lookup"><span data-stu-id="1a05f-132">Parent elements</span></span>

<span data-ttu-id="1a05f-133">なし。</span><span class="sxs-lookup"><span data-stu-id="1a05f-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a05f-134">注釈</span><span class="sxs-lookup"><span data-stu-id="1a05f-134">Remarks</span></span>

<span data-ttu-id="1a05f-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1a05f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a05f-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1a05f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a05f-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a05f-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a05f-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a05f-138">Schema name</span></span>  <br/> |<span data-ttu-id="1a05f-139">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1a05f-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="1a05f-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a05f-140">Validation file</span></span>  <br/> |<span data-ttu-id="1a05f-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1a05f-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a05f-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1a05f-142">Can be empty</span></span>  <br/> |<span data-ttu-id="1a05f-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="1a05f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a05f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a05f-144">See also</span></span>



[<span data-ttu-id="1a05f-145">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="1a05f-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="1a05f-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a05f-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

