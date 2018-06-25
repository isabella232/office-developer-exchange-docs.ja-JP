---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: RootFolder 要素には、FindItem 操作時に単一のルート フォルダーの検索の結果が含まれています。
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833254"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="477ab-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="477ab-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="477ab-104">**RootFolder**要素には、 [FindItem 操作](finditem-operation.md)中に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="477ab-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="477ab-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="477ab-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="477ab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="477ab-106">Attributes and elements</span></span>

<span data-ttu-id="477ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="477ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="477ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="477ab-108">Attributes</span></span>

|<span data-ttu-id="477ab-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="477ab-109">**Attribute**</span></span>|<span data-ttu-id="477ab-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="477ab-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="477ab-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="477ab-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="477ab-112">インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="477ab-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="477ab-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="477ab-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="477ab-114">分数のページ ビューを使用するときに、次の要求に使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="477ab-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="477ab-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="477ab-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="477ab-116">分数形式のページングを実行する場合、次の要求に使用する分母を表します。</span><span class="sxs-lookup"><span data-stu-id="477ab-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="477ab-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="477ab-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="477ab-118">さらにページングが必要ないように、現在の結果が、クエリの最後の項目を含めるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="477ab-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="477ab-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="477ab-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="477ab-120">制限を満たすアイテムの総数を表します。</span><span class="sxs-lookup"><span data-stu-id="477ab-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="477ab-121">グループ化された[FindItem 操作](finditem-operation.md)では、 **TotalItemsInView**属性は、ビュー内の項目の合計数とグループ数の合計を返します。</span><span class="sxs-lookup"><span data-stu-id="477ab-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="477ab-122">子要素</span><span class="sxs-lookup"><span data-stu-id="477ab-122">Child elements</span></span>

|<span data-ttu-id="477ab-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="477ab-123">**Element**</span></span>|<span data-ttu-id="477ab-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="477ab-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="477ab-125">Items</span><span class="sxs-lookup"><span data-stu-id="477ab-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="477ab-126">見つかったアイテムの配列が含まれています[FindItem 操作](finditem-operation.md)要求で指定された検索条件があります。</span><span class="sxs-lookup"><span data-stu-id="477ab-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="477ab-127">グループ</span><span class="sxs-lookup"><span data-stu-id="477ab-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="477ab-128">検出されたグループのコレクションが含まれています[FindItem 操作](finditem-operation.md)要求で指定された検索と集計の基準が存在します。</span><span class="sxs-lookup"><span data-stu-id="477ab-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="477ab-129">親要素</span><span class="sxs-lookup"><span data-stu-id="477ab-129">Parent elements</span></span>

|<span data-ttu-id="477ab-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="477ab-130">**Element**</span></span>|<span data-ttu-id="477ab-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="477ab-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="477ab-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="477ab-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="477ab-133">[FindItem 操作](finditem-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="477ab-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="477ab-134">備考</span><span class="sxs-lookup"><span data-stu-id="477ab-134">Remarks</span></span>

<span data-ttu-id="477ab-135">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="477ab-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="477ab-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="477ab-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="477ab-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="477ab-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="477ab-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="477ab-138">Schema name</span></span>  <br/> |<span data-ttu-id="477ab-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="477ab-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="477ab-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="477ab-140">Validation file</span></span>  <br/> |<span data-ttu-id="477ab-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="477ab-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="477ab-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="477ab-142">Can be empty</span></span>  <br/> |<span data-ttu-id="477ab-143">False</span><span class="sxs-lookup"><span data-stu-id="477ab-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="477ab-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="477ab-144">See also</span></span>



<span data-ttu-id="477ab-145">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="477ab-145">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="477ab-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="477ab-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="477ab-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="477ab-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="477ab-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="477ab-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="477ab-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="477ab-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="477ab-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="477ab-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="477ab-151">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="477ab-151">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

