---
title: (階層) の変更
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
description: 変更要素には、クライアント上のフォルダーや Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダー間の相違点の種類を表すの種類の変更の順序付けされた配列が含まれています。
ms.openlocfilehash: 15e4f9f37c5e4a4083260dcf379a49beb2260030
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759623"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="73c26-103">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="73c26-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="73c26-104">**変更**要素には、クライアント上のフォルダーや Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダー間の相違点の種類を表すの種類の変更の順序付けされた配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="73c26-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="73c26-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="73c26-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="73c26-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="73c26-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="73c26-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73c26-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="73c26-108">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="73c26-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="73c26-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="73c26-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73c26-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="73c26-110">Attributes and elements</span></span>

<span data-ttu-id="73c26-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73c26-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73c26-112">属性</span><span class="sxs-lookup"><span data-stu-id="73c26-112">Attributes</span></span>

<span data-ttu-id="73c26-113">なし。</span><span class="sxs-lookup"><span data-stu-id="73c26-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73c26-114">子要素</span><span class="sxs-lookup"><span data-stu-id="73c26-114">Child elements</span></span>

|<span data-ttu-id="73c26-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="73c26-115">**Element**</span></span>|<span data-ttu-id="73c26-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="73c26-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73c26-117">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="73c26-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="73c26-118">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="73c26-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="73c26-119">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="73c26-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="73c26-120">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="73c26-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="73c26-121">(集合的) を削除します。</span><span class="sxs-lookup"><span data-stu-id="73c26-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="73c26-122">ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="73c26-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73c26-123">親要素</span><span class="sxs-lookup"><span data-stu-id="73c26-123">Parent elements</span></span>

|<span data-ttu-id="73c26-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="73c26-124">**Element**</span></span>|<span data-ttu-id="73c26-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="73c26-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73c26-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73c26-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="73c26-127">SyncFolderHierarchy 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="73c26-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73c26-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="73c26-128">Text value</span></span>

<span data-ttu-id="73c26-129">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="73c26-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73c26-130">備考</span><span class="sxs-lookup"><span data-stu-id="73c26-130">Remarks</span></span>

<span data-ttu-id="73c26-131">EWS 仮想ディレクトリのクライアント アクセス サーバーの役割がインストールされている Exchange 2007 コンピューターには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="73c26-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73c26-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="73c26-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73c26-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="73c26-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73c26-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73c26-134">Schema name</span></span>  <br/> |<span data-ttu-id="73c26-135">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="73c26-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73c26-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73c26-136">Validation file</span></span>  <br/> |<span data-ttu-id="73c26-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73c26-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73c26-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="73c26-138">Can be empty</span></span>  <br/> |<span data-ttu-id="73c26-139">False</span><span class="sxs-lookup"><span data-stu-id="73c26-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73c26-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="73c26-140">See also</span></span>



[<span data-ttu-id="73c26-141">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="73c26-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


<span data-ttu-id="73c26-142">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="73c26-142">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
  
- [<span data-ttu-id="73c26-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="73c26-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

