---
title: (ItemSync) を削除します。
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
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: ローカル クライアント ストアで削除するのには 1 つのアイテムを識別する要素を削除します。
ms.openlocfilehash: 18b7ae2f97db2de64896680c3aa76f2590c03177
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759965"
---
# <a name="delete-itemsync"></a><span data-ttu-id="1d486-103">(ItemSync) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1d486-103">Delete (ItemSync)</span></span>

<span data-ttu-id="1d486-104">要素の**削除**は、ローカル クライアント ストアで削除するのには 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="1d486-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="1d486-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="1d486-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="1d486-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d486-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="1d486-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d486-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="1d486-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="1d486-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="1d486-109">(ItemSync) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1d486-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="1d486-110">**SyncFolderItemsDeleteType**</span><span class="sxs-lookup"><span data-stu-id="1d486-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1d486-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1d486-111">Attributes and elements</span></span>

<span data-ttu-id="1d486-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d486-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d486-113">属性</span><span class="sxs-lookup"><span data-stu-id="1d486-113">Attributes</span></span>

<span data-ttu-id="1d486-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1d486-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d486-115">子要素</span><span class="sxs-lookup"><span data-stu-id="1d486-115">Child elements</span></span>

|<span data-ttu-id="1d486-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d486-116">**Element**</span></span>|<span data-ttu-id="1d486-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d486-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d486-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="1d486-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1d486-119">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d486-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d486-120">親要素</span><span class="sxs-lookup"><span data-stu-id="1d486-120">Parent elements</span></span>

|<span data-ttu-id="1d486-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d486-121">**Element**</span></span>|<span data-ttu-id="1d486-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d486-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d486-123">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="1d486-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="1d486-124">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d486-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d486-125">備考</span><span class="sxs-lookup"><span data-stu-id="1d486-125">Remarks</span></span>

<span data-ttu-id="1d486-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1d486-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d486-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="1d486-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d486-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="1d486-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d486-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d486-129">Schema name</span></span>  <br/> |<span data-ttu-id="1d486-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1d486-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d486-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d486-131">Validation file</span></span>  <br/> |<span data-ttu-id="1d486-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1d486-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d486-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1d486-133">Can be empty</span></span>  <br/> |<span data-ttu-id="1d486-134">False</span><span class="sxs-lookup"><span data-stu-id="1d486-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d486-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d486-135">See also</span></span>

- [<span data-ttu-id="1d486-136">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="1d486-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="1d486-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d486-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

