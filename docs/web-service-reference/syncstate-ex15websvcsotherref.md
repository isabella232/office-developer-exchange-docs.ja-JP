---
title: SyncState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: SyncState 要素には、要求が成功するたびに更新される、base64 でエンコードされた形式の同期データが含まれています。 これは、同期状態を識別するために使用されます。
ms.openlocfilehash: 8e2d9a633cdad0a124b87e4e794399c06d3b5445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458965"
---
# <a name="syncstate"></a><span data-ttu-id="7d692-104">SyncState</span><span class="sxs-lookup"><span data-stu-id="7d692-104">SyncState</span></span>

<span data-ttu-id="7d692-105">**Syncstate**要素には、要求が成功するたびに更新される、base64 でエンコードされた形式の同期データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d692-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="7d692-106">これは、同期状態を識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="7d692-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="7d692-107">**String**</span><span class="sxs-lookup"><span data-stu-id="7d692-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d692-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d692-108">Attributes and elements</span></span>

<span data-ttu-id="7d692-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d692-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d692-110">属性</span><span class="sxs-lookup"><span data-stu-id="7d692-110">Attributes</span></span>

<span data-ttu-id="7d692-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7d692-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d692-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7d692-112">Child elements</span></span>

<span data-ttu-id="7d692-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7d692-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d692-114">親要素</span><span class="sxs-lookup"><span data-stu-id="7d692-114">Parent elements</span></span>

|<span data-ttu-id="7d692-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d692-115">**Element**</span></span>|<span data-ttu-id="7d692-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d692-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d692-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="7d692-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="7d692-118">クライアント上のフォルダー階層を同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7d692-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="7d692-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7d692-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="7d692-120">SyncFolderHierarchy 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7d692-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="7d692-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7d692-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="7d692-122">Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7d692-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="7d692-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7d692-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="7d692-124">SyncFolderItems 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7d692-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d692-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7d692-125">Text value</span></span>

<span data-ttu-id="7d692-126">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d692-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d692-127">注釈</span><span class="sxs-lookup"><span data-stu-id="7d692-127">Remarks</span></span>

<span data-ttu-id="7d692-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7d692-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d692-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d692-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d692-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d692-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d692-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d692-131">Schema name</span></span>  <br/> |<span data-ttu-id="7d692-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7d692-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d692-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d692-133">Validation file</span></span>  <br/> |<span data-ttu-id="7d692-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7d692-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d692-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7d692-135">Can be empty</span></span>  <br/> |<span data-ttu-id="7d692-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="7d692-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d692-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d692-137">See also</span></span>



[<span data-ttu-id="7d692-138">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="7d692-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="7d692-139">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="7d692-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="7d692-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d692-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

