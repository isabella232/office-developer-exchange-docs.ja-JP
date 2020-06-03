---
title: 変更 (アイテム)
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
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: Changes 要素には、クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列が含まれています。
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463266"
---
# <a name="changes-items"></a><span data-ttu-id="b8abf-103">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="b8abf-103">Changes (Items)</span></span>

<span data-ttu-id="b8abf-104">**Changes**要素には、クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b8abf-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="b8abf-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b8abf-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="b8abf-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b8abf-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="b8abf-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b8abf-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="b8abf-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="b8abf-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="b8abf-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="b8abf-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8abf-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8abf-110">Attributes and elements</span></span>

<span data-ttu-id="b8abf-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8abf-112">属性</span><span class="sxs-lookup"><span data-stu-id="b8abf-112">Attributes</span></span>

<span data-ttu-id="b8abf-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b8abf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8abf-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b8abf-114">Child elements</span></span>

|<span data-ttu-id="b8abf-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="b8abf-115">**Element**</span></span>|<span data-ttu-id="b8abf-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8abf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8abf-117">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b8abf-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="b8abf-118">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="b8abf-119">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b8abf-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="b8abf-120">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="b8abf-121">削除 (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b8abf-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="b8abf-122">ローカルクライアントストアで削除する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="b8abf-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="b8abf-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="b8abf-124">アイテムが読み取られたときに、 [Syncfolderitems 操作](syncfolderitems-operation.md)の応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="b8abf-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="b8abf-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8abf-126">親要素</span><span class="sxs-lookup"><span data-stu-id="b8abf-126">Parent elements</span></span>

|<span data-ttu-id="b8abf-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8abf-127">**Element**</span></span>|<span data-ttu-id="b8abf-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8abf-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8abf-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b8abf-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="b8abf-130">[Syncfolderitems 操作](syncfolderitems-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="b8abf-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8abf-131">注釈</span><span class="sxs-lookup"><span data-stu-id="b8abf-131">Remarks</span></span>

<span data-ttu-id="b8abf-132">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="b8abf-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8abf-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8abf-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8abf-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8abf-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8abf-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8abf-135">Schema name</span></span>  <br/> |<span data-ttu-id="b8abf-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8abf-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8abf-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8abf-137">Validation file</span></span>  <br/> |<span data-ttu-id="b8abf-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b8abf-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8abf-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8abf-139">Can be empty</span></span>  <br/> |<span data-ttu-id="b8abf-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="b8abf-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8abf-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8abf-141">See also</span></span>



[<span data-ttu-id="b8abf-142">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="b8abf-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="b8abf-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b8abf-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

