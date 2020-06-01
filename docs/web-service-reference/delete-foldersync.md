---
title: Delete (FolderSync)
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
description: Delete 要素は、ローカルクライアントストアで削除する1つのフォルダーを識別します。
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454982"
---
# <a name="delete-foldersync"></a><span data-ttu-id="0b0b1-103">Delete (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="0b0b1-103">Delete (FolderSync)</span></span>

<span data-ttu-id="0b0b1-104">**Delete**要素は、ローカルクライアントストアで削除する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="0b0b1-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="0b0b1-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="0b0b1-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b0b1-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="0b0b1-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b0b1-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="0b0b1-108">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="0b0b1-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="0b0b1-109">Delete (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="0b0b1-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="0b0b1-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="0b0b1-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0b0b1-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0b0b1-111">Attributes and elements</span></span>

<span data-ttu-id="0b0b1-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b0b1-113">属性</span><span class="sxs-lookup"><span data-stu-id="0b0b1-113">Attributes</span></span>

<span data-ttu-id="0b0b1-114">なし。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b0b1-115">子要素</span><span class="sxs-lookup"><span data-stu-id="0b0b1-115">Child elements</span></span>

|<span data-ttu-id="0b0b1-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="0b0b1-116">**Element**</span></span>|<span data-ttu-id="0b0b1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b0b1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b0b1-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="0b0b1-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0b0b1-119">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b0b1-120">親要素</span><span class="sxs-lookup"><span data-stu-id="0b0b1-120">Parent elements</span></span>

|<span data-ttu-id="0b0b1-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b0b1-121">**Element**</span></span>|<span data-ttu-id="0b0b1-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b0b1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b0b1-123">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="0b0b1-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="0b0b1-124">クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b0b1-125">注釈</span><span class="sxs-lookup"><span data-stu-id="0b0b1-125">Remarks</span></span>

<span data-ttu-id="0b0b1-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 コンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b0b1-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0b0b1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b0b1-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b0b1-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b0b1-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b0b1-129">Schema name</span></span>  <br/> |<span data-ttu-id="0b0b1-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0b0b1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b0b1-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b0b1-131">Validation file</span></span>  <br/> |<span data-ttu-id="0b0b1-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0b0b1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b0b1-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0b0b1-133">Can be empty</span></span>  <br/> |<span data-ttu-id="0b0b1-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="0b0b1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b0b1-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b0b1-135">See also</span></span>

- [<span data-ttu-id="0b0b1-136">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="0b0b1-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- <span data-ttu-id="0b0b1-137">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="0b0b1-137">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="0b0b1-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b0b1-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

