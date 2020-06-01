---
title: 変更 (階層)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Changes 要素には、クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463273"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="c951f-103">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="c951f-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="c951f-104">**Changes**要素には、クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c951f-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="c951f-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c951f-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="c951f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c951f-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c951f-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c951f-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="c951f-108">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="c951f-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="c951f-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="c951f-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c951f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c951f-110">Attributes and elements</span></span>

<span data-ttu-id="c951f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c951f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c951f-112">属性</span><span class="sxs-lookup"><span data-stu-id="c951f-112">Attributes</span></span>

<span data-ttu-id="c951f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c951f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c951f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="c951f-114">Child elements</span></span>

|<span data-ttu-id="c951f-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="c951f-115">**Element**</span></span>|<span data-ttu-id="c951f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="c951f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c951f-117">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c951f-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="c951f-118">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c951f-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c951f-119">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c951f-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="c951f-120">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c951f-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c951f-121">Delete (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c951f-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="c951f-122">ローカルクライアントストアで削除する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c951f-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c951f-123">親要素</span><span class="sxs-lookup"><span data-stu-id="c951f-123">Parent elements</span></span>

|<span data-ttu-id="c951f-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="c951f-124">**Element**</span></span>|<span data-ttu-id="c951f-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="c951f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c951f-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c951f-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="c951f-127">SyncFolderHierarchy 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c951f-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c951f-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c951f-128">Text value</span></span>

<span data-ttu-id="c951f-129">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="c951f-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c951f-130">注釈</span><span class="sxs-lookup"><span data-stu-id="c951f-130">Remarks</span></span>

<span data-ttu-id="c951f-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 コンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c951f-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c951f-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c951f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c951f-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="c951f-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c951f-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c951f-134">Schema name</span></span>  <br/> |<span data-ttu-id="c951f-135">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c951f-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c951f-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c951f-136">Validation file</span></span>  <br/> |<span data-ttu-id="c951f-137">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c951f-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c951f-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c951f-138">Can be empty</span></span>  <br/> |<span data-ttu-id="c951f-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="c951f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c951f-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="c951f-140">See also</span></span>



[<span data-ttu-id="c951f-141">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="c951f-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


<span data-ttu-id="c951f-142">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="c951f-142">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
  
- [<span data-ttu-id="c951f-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c951f-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

