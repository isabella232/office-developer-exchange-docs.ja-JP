---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: FractionalPageItemView 要素は、ページビューの開始位置と、FindItem 要求で返されるアイテムの最大数を表します。
ms.openlocfilehash: cbf45838558873dc5846823c2d1b26cf2c8af514
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461311"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="2b255-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="2b255-103">FractionalPageItemView</span></span>

<span data-ttu-id="2b255-104">**FractionalPageItemView**要素は、ページビューの開始位置と、 [FindItem](finditem.md)要求で返されるアイテムの最大数を表します。</span><span class="sxs-lookup"><span data-stu-id="2b255-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="2b255-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="2b255-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="2b255-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="2b255-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="2b255-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="2b255-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b255-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2b255-108">Attributes and elements</span></span>

<span data-ttu-id="2b255-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b255-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b255-110">属性</span><span class="sxs-lookup"><span data-stu-id="2b255-110">Attributes</span></span>

|<span data-ttu-id="2b255-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="2b255-111">**Attribute**</span></span>|<span data-ttu-id="2b255-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b255-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b255-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="2b255-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="2b255-114">[FindItem](finditem.md)応答で返される結果の最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b255-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="2b255-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2b255-115">This attribute is optional.</span></span> <span data-ttu-id="2b255-116">この属性が指定されていない場合、呼び出しは利用可能なすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="2b255-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="2b255-117">**分子**</span><span class="sxs-lookup"><span data-stu-id="2b255-117">**Numerator**</span></span> <br/> |<span data-ttu-id="2b255-118">結果セットの先頭からの、分数のオフセットの分子を表します。</span><span class="sxs-lookup"><span data-stu-id="2b255-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="2b255-119">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="2b255-119">This attribute is required.</span></span> <span data-ttu-id="2b255-120">分子は、分母以下の値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b255-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="2b255-121">この属性は、ゼロ以上の整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b255-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="2b255-122">詳細については、このトピックで後述する「備考」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b255-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="2b255-123">**分母**</span><span class="sxs-lookup"><span data-stu-id="2b255-123">**Denominator**</span></span> <br/> |<span data-ttu-id="2b255-124">結果セット内の項目の総数の先頭からの、分単位のオフセットの分母を表します。</span><span class="sxs-lookup"><span data-stu-id="2b255-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="2b255-125">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="2b255-125">This attribute is required.</span></span> <span data-ttu-id="2b255-126">この属性は、1より大きい整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b255-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="2b255-127">詳細については、このトピックで後述する「備考」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b255-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2b255-128">子要素</span><span class="sxs-lookup"><span data-stu-id="2b255-128">Child elements</span></span>

<span data-ttu-id="2b255-129">なし。</span><span class="sxs-lookup"><span data-stu-id="2b255-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b255-130">親要素</span><span class="sxs-lookup"><span data-stu-id="2b255-130">Parent elements</span></span>

|<span data-ttu-id="2b255-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="2b255-131">**Element**</span></span>|<span data-ttu-id="2b255-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b255-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b255-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="2b255-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="2b255-134">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b255-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="2b255-135">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b255-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b255-136">注釈</span><span class="sxs-lookup"><span data-stu-id="2b255-136">Remarks</span></span>

<span data-ttu-id="2b255-137">検索されたアイテムのセットの先頭からのページビューオフセットは、分数で示されます。</span><span class="sxs-lookup"><span data-stu-id="2b255-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="2b255-138">**分子**および**分母**属性で定義されている分数は、情報のページが開始する場所を示します。</span><span class="sxs-lookup"><span data-stu-id="2b255-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="2b255-139">たとえば、**分子**が4で、**分母**が5の場合、返された情報のページは、結果セット内の fifths にあるエントリから始まります。</span><span class="sxs-lookup"><span data-stu-id="2b255-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="2b255-140">分数が0に評価された場合は、結果セットの開始を示します。</span><span class="sxs-lookup"><span data-stu-id="2b255-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="2b255-141">分数が1に評価される場合は、結果セットの末尾を示します。</span><span class="sxs-lookup"><span data-stu-id="2b255-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2b255-142">分数は、結果セット内の結果の数ではなく、ページの開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="2b255-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="2b255-143">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2b255-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="2b255-144">例</span><span class="sxs-lookup"><span data-stu-id="2b255-144">Example</span></span>

<span data-ttu-id="2b255-145">次の例は、 [FindItem](finditem.md)要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="2b255-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="2b255-146">要求は、結果セット内のすべてのアイテムの第3番目の第3番目の後に開始される検索結果からアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="2b255-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2b255-147">たとえば、結果セットに9個のアイテムが含まれている場合、ページングされたビューは最大12個のアイテムを返します。これは、結果セットの途中で3分間に見つかったアイテムから始まります。</span><span class="sxs-lookup"><span data-stu-id="2b255-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="2b255-148">この場合、ページは7番目の項目から開始されます。</span><span class="sxs-lookup"><span data-stu-id="2b255-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="2b255-149">ページには7番目、8番目、9番目のアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2b255-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="2b255-150">分子が0に設定されている場合、ページビューは、結果セット内のすべてのアイテムを返します。この値は、 **Maxん返され**た属性の値よりも小さくなります。</span><span class="sxs-lookup"><span data-stu-id="2b255-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2b255-151">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2b255-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b255-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b255-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2b255-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b255-153">Schema Name</span></span>  <br/> |<span data-ttu-id="2b255-154">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2b255-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2b255-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b255-155">Validation File</span></span>  <br/> |<span data-ttu-id="2b255-156">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2b255-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b255-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2b255-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b255-158">正しくない</span><span class="sxs-lookup"><span data-stu-id="2b255-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b255-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b255-159">See also</span></span>



<span data-ttu-id="2b255-160">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="2b255-160">[FindItem operation](finditem-operation.md)</span></span>


[<span data-ttu-id="2b255-161">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="2b255-161">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

