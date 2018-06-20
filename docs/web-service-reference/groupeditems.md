---
title: GroupedItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: GroupedItems 要素は、グループ化された FindItem 操作の呼び出しの結果であるアイテムのコレクションを表します。
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831756"
---
# <a name="groupeditems"></a><span data-ttu-id="cf761-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="cf761-103">GroupedItems</span></span>

<span data-ttu-id="cf761-104">**GroupedItems**要素がグループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを表しますを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cf761-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="cf761-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="cf761-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="cf761-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cf761-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="cf761-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cf761-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="cf761-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="cf761-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="cf761-109">グループ</span><span class="sxs-lookup"><span data-stu-id="cf761-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="cf761-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="cf761-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="cf761-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="cf761-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf761-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cf761-112">Attributes and elements</span></span>

<span data-ttu-id="cf761-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf761-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf761-114">属性</span><span class="sxs-lookup"><span data-stu-id="cf761-114">Attributes</span></span>

<span data-ttu-id="cf761-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cf761-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf761-116">子要素</span><span class="sxs-lookup"><span data-stu-id="cf761-116">Child elements</span></span>

|<span data-ttu-id="cf761-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf761-117">**Element**</span></span>|<span data-ttu-id="cf761-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf761-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf761-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="cf761-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="cf761-120">グループ化された[FindItem 操作](finditem-operation.md)でアイテムをグループ化するために使用されるプロパティの値を表しますを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cf761-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="cf761-121">Items</span><span class="sxs-lookup"><span data-stu-id="cf761-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="cf761-122">グループ化された項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf761-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf761-123">親要素</span><span class="sxs-lookup"><span data-stu-id="cf761-123">Parent elements</span></span>

|<span data-ttu-id="cf761-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf761-124">**Element**</span></span>|<span data-ttu-id="cf761-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf761-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf761-126">グループ</span><span class="sxs-lookup"><span data-stu-id="cf761-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="cf761-127">[FindItem 操作](finditem-operation.md)の要求で指定されている検索と集計の基準で検出されたグループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf761-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf761-128">備考</span><span class="sxs-lookup"><span data-stu-id="cf761-128">Remarks</span></span>

<span data-ttu-id="cf761-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cf761-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf761-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="cf761-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf761-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="cf761-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf761-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf761-132">Schema name</span></span>  <br/> |<span data-ttu-id="cf761-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cf761-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf761-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf761-134">Validation file</span></span>  <br/> |<span data-ttu-id="cf761-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf761-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf761-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cf761-136">Can be empty</span></span>  <br/> |<span data-ttu-id="cf761-137">False</span><span class="sxs-lookup"><span data-stu-id="cf761-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf761-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf761-138">See also</span></span>



<span data-ttu-id="cf761-139">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="cf761-139">[FindItem operation](finditem-operation.md)</span></span>


[<span data-ttu-id="cf761-140">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="cf761-140">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

