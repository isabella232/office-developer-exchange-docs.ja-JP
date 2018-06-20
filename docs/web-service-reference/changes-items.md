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
description: 変更要素には、クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759619"
---
# <a name="changes-items"></a><span data-ttu-id="0a57d-103">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="0a57d-103">Changes (Items)</span></span>

<span data-ttu-id="0a57d-104">**変更**要素には、クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a57d-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="0a57d-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0a57d-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="0a57d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a57d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="0a57d-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a57d-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="0a57d-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="0a57d-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="0a57d-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="0a57d-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a57d-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0a57d-110">Attributes and elements</span></span>

<span data-ttu-id="0a57d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a57d-112">属性</span><span class="sxs-lookup"><span data-stu-id="0a57d-112">Attributes</span></span>

<span data-ttu-id="0a57d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0a57d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a57d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="0a57d-114">Child elements</span></span>

|<span data-ttu-id="0a57d-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="0a57d-115">**Element**</span></span>|<span data-ttu-id="0a57d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a57d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a57d-117">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="0a57d-118">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0a57d-119">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0a57d-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="0a57d-120">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0a57d-121">(ItemSync) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="0a57d-122">ローカル クライアント ストアで削除するのには 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0a57d-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="0a57d-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="0a57d-124">アイテムを開封したときに、 [SyncFolderItems 操作](syncfolderitems-operation.md)の応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="0a57d-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="0a57d-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0a57d-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a57d-126">親要素</span><span class="sxs-lookup"><span data-stu-id="0a57d-126">Parent elements</span></span>

|<span data-ttu-id="0a57d-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="0a57d-127">**Element**</span></span>|<span data-ttu-id="0a57d-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a57d-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a57d-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a57d-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="0a57d-130">[SyncFolderItems 操作](syncfolderitems-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a57d-131">備考</span><span class="sxs-lookup"><span data-stu-id="0a57d-131">Remarks</span></span>

<span data-ttu-id="0a57d-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0a57d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a57d-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="0a57d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a57d-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="0a57d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a57d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a57d-135">Schema name</span></span>  <br/> |<span data-ttu-id="0a57d-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0a57d-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a57d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a57d-137">Validation file</span></span>  <br/> |<span data-ttu-id="0a57d-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0a57d-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a57d-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0a57d-139">Can be empty</span></span>  <br/> |<span data-ttu-id="0a57d-140">False</span><span class="sxs-lookup"><span data-stu-id="0a57d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a57d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="0a57d-141">See also</span></span>



[<span data-ttu-id="0a57d-142">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="0a57d-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="0a57d-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0a57d-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

