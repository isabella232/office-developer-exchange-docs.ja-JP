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
description: RootFolder 要素には、FindItem 操作中の1つのルートフォルダーの検索結果が含まれています。
ms.openlocfilehash: 3bbab325dff26139739c50ef519b215aea620a0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457131"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="1896f-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="1896f-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="1896f-104">**RootFolder**要素には、 [FindItem 操作](finditem-operation.md)中の1つのルートフォルダーの検索結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1896f-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="1896f-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="1896f-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1896f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1896f-106">Attributes and elements</span></span>

<span data-ttu-id="1896f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1896f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1896f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1896f-108">Attributes</span></span>

|<span data-ttu-id="1896f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1896f-109">**Attribute**</span></span>|<span data-ttu-id="1896f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1896f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1896f-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="1896f-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="1896f-112">インデックス付きページングビューを使用するときに次の要求に使用される次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="1896f-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="1896f-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="1896f-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="1896f-114">分数のページビューを使用するときに、次の要求に対して使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="1896f-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="1896f-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="1896f-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="1896f-116">分数のページングを行うときに、次の要求に対して使用する次の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="1896f-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="1896f-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="1896f-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="1896f-118">現在の結果にクエリの最後のアイテムが含まれているかどうかを示します。この場合、追加のページングは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1896f-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="1896f-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="1896f-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="1896f-120">制限に合格したアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="1896f-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="1896f-121">グループ化された[FindItem 操作](finditem-operation.md)では、 **Totalitemsinview**属性は、ビュー内のアイテムの合計数とグループの合計数を返します。</span><span class="sxs-lookup"><span data-stu-id="1896f-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1896f-122">子要素</span><span class="sxs-lookup"><span data-stu-id="1896f-122">Child elements</span></span>

|<span data-ttu-id="1896f-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="1896f-123">**Element**</span></span>|<span data-ttu-id="1896f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="1896f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1896f-125">Items</span><span class="sxs-lookup"><span data-stu-id="1896f-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="1896f-126">[FindItem 操作](finditem-operation.md)要求で識別された検索条件を持つアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1896f-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1896f-127">Groups</span><span class="sxs-lookup"><span data-stu-id="1896f-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="1896f-128">[FindItem 操作](finditem-operation.md)要求で識別される検索および集約の条件を持つグループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1896f-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1896f-129">親要素</span><span class="sxs-lookup"><span data-stu-id="1896f-129">Parent elements</span></span>

|<span data-ttu-id="1896f-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="1896f-130">**Element**</span></span>|<span data-ttu-id="1896f-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="1896f-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1896f-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1896f-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="1896f-133">[FindItem 操作](finditem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="1896f-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1896f-134">注釈</span><span class="sxs-lookup"><span data-stu-id="1896f-134">Remarks</span></span>

<span data-ttu-id="1896f-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1896f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1896f-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1896f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1896f-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="1896f-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1896f-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1896f-138">Schema name</span></span>  <br/> |<span data-ttu-id="1896f-139">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1896f-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1896f-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1896f-140">Validation file</span></span>  <br/> |<span data-ttu-id="1896f-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1896f-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1896f-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1896f-142">Can be empty</span></span>  <br/> |<span data-ttu-id="1896f-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="1896f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1896f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="1896f-144">See also</span></span>



<span data-ttu-id="1896f-145">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1896f-145">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="1896f-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="1896f-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="1896f-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="1896f-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="1896f-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="1896f-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="1896f-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="1896f-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="1896f-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="1896f-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="1896f-151">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="1896f-151">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

