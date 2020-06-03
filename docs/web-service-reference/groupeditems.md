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
description: GroupedItems 要素は、グループ化された FindItem 操作呼び出しの結果であるアイテムのコレクションを表します。
ms.openlocfilehash: 0ee1ca3c6d0cf98e2daefa60a1cb1fd096cda478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530812"
---
# <a name="groupeditems"></a><span data-ttu-id="49475-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="49475-103">GroupedItems</span></span>

<span data-ttu-id="49475-104">**Groupeditems**要素は、グループ化された[FindItem 操作](finditem-operation.md)呼び出しの結果であるアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="49475-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="49475-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="49475-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="49475-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="49475-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="49475-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49475-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="49475-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="49475-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="49475-109">Groups</span><span class="sxs-lookup"><span data-stu-id="49475-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="49475-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="49475-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="49475-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="49475-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49475-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="49475-112">Attributes and elements</span></span>

<span data-ttu-id="49475-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49475-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49475-114">属性</span><span class="sxs-lookup"><span data-stu-id="49475-114">Attributes</span></span>

<span data-ttu-id="49475-115">なし。</span><span class="sxs-lookup"><span data-stu-id="49475-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49475-116">子要素</span><span class="sxs-lookup"><span data-stu-id="49475-116">Child elements</span></span>

|<span data-ttu-id="49475-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="49475-117">**Element**</span></span>|<span data-ttu-id="49475-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="49475-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49475-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="49475-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="49475-120">グループ化された[FindItem 操作](finditem-operation.md)の呼び出しでアイテムをグループ化するために使用されるプロパティの値を表します。</span><span class="sxs-lookup"><span data-stu-id="49475-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="49475-121">Items</span><span class="sxs-lookup"><span data-stu-id="49475-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="49475-122">グループ化されたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="49475-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49475-123">親要素</span><span class="sxs-lookup"><span data-stu-id="49475-123">Parent elements</span></span>

|<span data-ttu-id="49475-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="49475-124">**Element**</span></span>|<span data-ttu-id="49475-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="49475-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49475-126">Groups</span><span class="sxs-lookup"><span data-stu-id="49475-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="49475-127">[FindItem 操作](finditem-operation.md)要求で識別される検索および集約条件を含むグループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="49475-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49475-128">注釈</span><span class="sxs-lookup"><span data-stu-id="49475-128">Remarks</span></span>

<span data-ttu-id="49475-129">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="49475-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49475-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="49475-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49475-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="49475-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49475-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49475-132">Schema name</span></span>  <br/> |<span data-ttu-id="49475-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="49475-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="49475-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49475-134">Validation file</span></span>  <br/> |<span data-ttu-id="49475-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="49475-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49475-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="49475-136">Can be empty</span></span>  <br/> |<span data-ttu-id="49475-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="49475-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49475-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="49475-138">See also</span></span>



[<span data-ttu-id="49475-139">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="49475-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="49475-140">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="49475-140">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

