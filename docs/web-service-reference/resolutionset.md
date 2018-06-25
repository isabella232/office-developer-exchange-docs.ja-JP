---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: ResolutionSet 要素には、あいまいな名前の解決策の配列が含まれています。
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833160"
---
# <a name="resolutionset"></a><span data-ttu-id="fa6c4-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="fa6c4-103">ResolutionSet</span></span>

<span data-ttu-id="fa6c4-104">**ResolutionSet**要素には、あいまいな名前の解決策の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="fa6c4-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="fa6c4-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="fa6c4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fa6c4-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="fa6c4-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fa6c4-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="fa6c4-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="fa6c4-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="fa6c4-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa6c4-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fa6c4-110">Attributes and elements</span></span>

<span data-ttu-id="fa6c4-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa6c4-112">属性</span><span class="sxs-lookup"><span data-stu-id="fa6c4-112">Attributes</span></span>

|<span data-ttu-id="fa6c4-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-113">**Attribute**</span></span>|<span data-ttu-id="fa6c4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa6c4-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="fa6c4-116">次に、インデックス付きページング ビューを使用しているときに次の要求に使用するインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="fa6c4-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="fa6c4-118">分数のページ ビューを使用しているときに、次の要求に使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="fa6c4-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="fa6c4-120">分母分数のページ ビューを使用しているときに、次の要求に使用するを表します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="fa6c4-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="fa6c4-122">追加のページングが必要ないように、この属性が true の場合、現在の結果には、クエリの最後の項目が含まれているされます。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="fa6c4-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="fa6c4-124">ビュー内の項目の合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa6c4-125">子要素</span><span class="sxs-lookup"><span data-stu-id="fa6c4-125">Child elements</span></span>

|<span data-ttu-id="fa6c4-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-126">**Element**</span></span>|<span data-ttu-id="fa6c4-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa6c4-128">解決策</span><span class="sxs-lookup"><span data-stu-id="fa6c4-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="fa6c4-129">解決された 1 つのエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa6c4-130">親要素</span><span class="sxs-lookup"><span data-stu-id="fa6c4-130">Parent elements</span></span>

|<span data-ttu-id="fa6c4-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-131">**Element**</span></span>|<span data-ttu-id="fa6c4-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa6c4-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa6c4-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fa6c4-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="fa6c4-134">ResolveNames 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa6c4-135">備考</span><span class="sxs-lookup"><span data-stu-id="fa6c4-135">Remarks</span></span>

<span data-ttu-id="fa6c4-136">**ResolutionSet**要素には、100 の解決されたエンティティの最大を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="fa6c4-137">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fa6c4-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa6c4-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="fa6c4-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa6c4-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="fa6c4-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa6c4-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa6c4-140">Schema Name</span></span>  <br/> |<span data-ttu-id="fa6c4-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fa6c4-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fa6c4-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa6c4-142">Validation File</span></span>  <br/> |<span data-ttu-id="fa6c4-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fa6c4-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa6c4-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fa6c4-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa6c4-145">False</span><span class="sxs-lookup"><span data-stu-id="fa6c4-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa6c4-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa6c4-146">See also</span></span>



[<span data-ttu-id="fa6c4-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="fa6c4-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="fa6c4-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="fa6c4-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="fa6c4-149">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="fa6c4-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="fa6c4-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa6c4-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

