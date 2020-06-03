---
title: 削除 (ItemSync)
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
description: Delete 要素は、ローカルクライアントストアで削除する1つの項目を識別します。
ms.openlocfilehash: 6e30ddc7f7248fe7ff7136e19ba58c7d5d8a800f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454681"
---
# <a name="delete-itemsync"></a><span data-ttu-id="10223-103">削除 (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="10223-103">Delete (ItemSync)</span></span>

<span data-ttu-id="10223-104">**Delete**要素は、ローカルクライアントストアで削除する1つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="10223-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="10223-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="10223-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="10223-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="10223-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="10223-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="10223-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="10223-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="10223-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="10223-109">削除 (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="10223-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="10223-110">**SyncFolderItemsDeleteType**</span><span class="sxs-lookup"><span data-stu-id="10223-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="10223-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="10223-111">Attributes and elements</span></span>

<span data-ttu-id="10223-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="10223-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10223-113">属性</span><span class="sxs-lookup"><span data-stu-id="10223-113">Attributes</span></span>

<span data-ttu-id="10223-114">なし。</span><span class="sxs-lookup"><span data-stu-id="10223-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10223-115">子要素</span><span class="sxs-lookup"><span data-stu-id="10223-115">Child elements</span></span>

|<span data-ttu-id="10223-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="10223-116">**Element**</span></span>|<span data-ttu-id="10223-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="10223-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10223-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="10223-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="10223-119">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="10223-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10223-120">親要素</span><span class="sxs-lookup"><span data-stu-id="10223-120">Parent elements</span></span>

|<span data-ttu-id="10223-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="10223-121">**Element**</span></span>|<span data-ttu-id="10223-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="10223-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10223-123">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="10223-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="10223-124">クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列を含みます。</span><span class="sxs-lookup"><span data-stu-id="10223-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="10223-125">注釈</span><span class="sxs-lookup"><span data-stu-id="10223-125">Remarks</span></span>

<span data-ttu-id="10223-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="10223-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10223-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="10223-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10223-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="10223-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10223-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="10223-129">Schema name</span></span>  <br/> |<span data-ttu-id="10223-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="10223-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="10223-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="10223-131">Validation file</span></span>  <br/> |<span data-ttu-id="10223-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="10223-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10223-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="10223-133">Can be empty</span></span>  <br/> |<span data-ttu-id="10223-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="10223-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10223-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="10223-135">See also</span></span>

- [<span data-ttu-id="10223-136">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="10223-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="10223-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="10223-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

