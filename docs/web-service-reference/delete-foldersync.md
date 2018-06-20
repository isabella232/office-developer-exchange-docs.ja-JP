---
title: (集合的) を削除します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別する要素を削除します。
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19759957"
---
# <a name="delete-foldersync"></a><span data-ttu-id="c804c-103">(集合的) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c804c-103">Delete (FolderSync)</span></span>

<span data-ttu-id="c804c-104">要素の**削除**は、ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c804c-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="c804c-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c804c-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="c804c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c804c-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="c804c-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c804c-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="c804c-108">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="c804c-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="c804c-109">(集合的) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c804c-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="c804c-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="c804c-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c804c-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c804c-111">Attributes and elements</span></span>

<span data-ttu-id="c804c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c804c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c804c-113">属性</span><span class="sxs-lookup"><span data-stu-id="c804c-113">Attributes</span></span>

<span data-ttu-id="c804c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="c804c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c804c-115">子要素</span><span class="sxs-lookup"><span data-stu-id="c804c-115">Child elements</span></span>

|<span data-ttu-id="c804c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c804c-116">**Element**</span></span>|<span data-ttu-id="c804c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c804c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c804c-118">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="c804c-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="c804c-119">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c804c-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c804c-120">親要素</span><span class="sxs-lookup"><span data-stu-id="c804c-120">Parent elements</span></span>

|<span data-ttu-id="c804c-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="c804c-121">**Element**</span></span>|<span data-ttu-id="c804c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c804c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c804c-123">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="c804c-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="c804c-124">クライアント上のフォルダーや Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダー間の相違点の種類を表すの種類の変更の順序付けされた配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c804c-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c804c-125">備考</span><span class="sxs-lookup"><span data-stu-id="c804c-125">Remarks</span></span>

<span data-ttu-id="c804c-126">EWS 仮想ディレクトリのクライアント アクセス サーバーの役割がインストールされている Exchange 2007 コンピューターには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c804c-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c804c-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="c804c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c804c-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="c804c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c804c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c804c-129">Schema name</span></span>  <br/> |<span data-ttu-id="c804c-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c804c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c804c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c804c-131">Validation file</span></span>  <br/> |<span data-ttu-id="c804c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c804c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c804c-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c804c-133">Can be empty</span></span>  <br/> |<span data-ttu-id="c804c-134">False</span><span class="sxs-lookup"><span data-stu-id="c804c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c804c-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="c804c-135">See also</span></span>

- [<span data-ttu-id="c804c-136">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="c804c-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- <span data-ttu-id="c804c-137">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="c804c-137">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="c804c-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c804c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

