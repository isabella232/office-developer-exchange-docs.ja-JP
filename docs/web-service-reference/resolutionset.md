---
title: 解像度セット
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
description: 解像度セット要素には、あいまいな名前の解決の配列が含まれています。
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467173"
---
# <a name="resolutionset"></a><span data-ttu-id="f06b8-103">解像度セット</span><span class="sxs-lookup"><span data-stu-id="f06b8-103">ResolutionSet</span></span>

<span data-ttu-id="f06b8-104">解像度**セット**要素には、あいまいな名前の解決の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f06b8-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="f06b8-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="f06b8-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="f06b8-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f06b8-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="f06b8-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f06b8-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="f06b8-108">解像度セット</span><span class="sxs-lookup"><span data-stu-id="f06b8-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="f06b8-109">**Arrayof解像度の種類**</span><span class="sxs-lookup"><span data-stu-id="f06b8-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f06b8-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f06b8-110">Attributes and elements</span></span>

<span data-ttu-id="f06b8-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f06b8-112">属性</span><span class="sxs-lookup"><span data-stu-id="f06b8-112">Attributes</span></span>

|<span data-ttu-id="f06b8-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="f06b8-113">**Attribute**</span></span>|<span data-ttu-id="f06b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f06b8-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f06b8-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="f06b8-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="f06b8-116">インデックス付きのページビューを使用している場合に、次の要求に使用する必要がある次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="f06b8-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="f06b8-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="f06b8-118">分数のページビューを使用しているときに、次の要求に対して使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="f06b8-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="f06b8-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="f06b8-120">分数のページビューを使用しているときに、次の要求に対して使用する次の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="f06b8-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="f06b8-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="f06b8-122">現在の結果にクエリの最後のアイテムが含まれている場合は、この属性は true になり、追加のページングは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="f06b8-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="f06b8-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="f06b8-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="f06b8-124">ビュー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f06b8-125">子要素</span><span class="sxs-lookup"><span data-stu-id="f06b8-125">Child elements</span></span>

|<span data-ttu-id="f06b8-126">**Element**</span><span class="sxs-lookup"><span data-stu-id="f06b8-126">**Element**</span></span>|<span data-ttu-id="f06b8-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="f06b8-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f06b8-128">Resolution</span><span class="sxs-lookup"><span data-stu-id="f06b8-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="f06b8-129">1つの解決済みエンティティを含みます。</span><span class="sxs-lookup"><span data-stu-id="f06b8-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f06b8-130">親要素</span><span class="sxs-lookup"><span data-stu-id="f06b8-130">Parent elements</span></span>

|<span data-ttu-id="f06b8-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="f06b8-131">**Element**</span></span>|<span data-ttu-id="f06b8-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="f06b8-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f06b8-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f06b8-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="f06b8-134">ResolveNames 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f06b8-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f06b8-135">注釈</span><span class="sxs-lookup"><span data-stu-id="f06b8-135">Remarks</span></span>

<span data-ttu-id="f06b8-136">**解像度セット**要素には、最大100個の解決済みエンティティを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f06b8-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="f06b8-137">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="f06b8-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f06b8-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f06b8-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f06b8-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="f06b8-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f06b8-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f06b8-140">Schema Name</span></span>  <br/> |<span data-ttu-id="f06b8-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f06b8-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f06b8-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f06b8-142">Validation File</span></span>  <br/> |<span data-ttu-id="f06b8-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f06b8-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f06b8-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f06b8-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="f06b8-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="f06b8-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f06b8-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="f06b8-146">See also</span></span>



[<span data-ttu-id="f06b8-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f06b8-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="f06b8-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="f06b8-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="f06b8-149">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="f06b8-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="f06b8-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f06b8-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

