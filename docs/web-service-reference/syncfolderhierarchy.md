---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: SyncFolderHierarchy 要素は、クライアント上のフォルダー階層を同期する要求を定義します。
ms.openlocfilehash: 68b607dbf603e955f74dfaccadd3ce6c4c9fb6ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466648"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="1f930-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1f930-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="1f930-104">**Syncfolderhierarchy**要素は、クライアント上のフォルダー階層を同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1f930-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="1f930-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="1f930-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f930-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f930-106">Attributes and elements</span></span>

<span data-ttu-id="1f930-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f930-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f930-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f930-108">Attributes</span></span>

<span data-ttu-id="1f930-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1f930-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f930-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1f930-110">Child elements</span></span>

|<span data-ttu-id="1f930-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1f930-111">**Element**</span></span>|<span data-ttu-id="1f930-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f930-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f930-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="1f930-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="1f930-114">[Syncfolderhierarchy](syncfolderhierarchy.md)応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1f930-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="1f930-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="1f930-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="1f930-116">同期するアイテムを含むフォルダを表します。</span><span class="sxs-lookup"><span data-stu-id="1f930-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="1f930-117">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f930-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f930-118">SyncState</span><span class="sxs-lookup"><span data-stu-id="1f930-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1f930-119">要求が成功するたびに更新される同期データの base64 でエンコードされた形式が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1f930-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="1f930-120">これは、同期状態を識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f930-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f930-121">親要素</span><span class="sxs-lookup"><span data-stu-id="1f930-121">Parent elements</span></span>

<span data-ttu-id="1f930-122">なし。</span><span class="sxs-lookup"><span data-stu-id="1f930-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f930-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1f930-123">Remarks</span></span>

<span data-ttu-id="1f930-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f930-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f930-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f930-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f930-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f930-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f930-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f930-127">Schema name</span></span>  <br/> |<span data-ttu-id="1f930-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1f930-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f930-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f930-129">Validation file</span></span>  <br/> |<span data-ttu-id="1f930-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1f930-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f930-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f930-131">Can be empty</span></span>  <br/> |<span data-ttu-id="1f930-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f930-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f930-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f930-133">See also</span></span>



[<span data-ttu-id="1f930-134">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="1f930-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="1f930-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f930-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

