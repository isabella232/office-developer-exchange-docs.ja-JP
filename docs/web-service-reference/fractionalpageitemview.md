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
description: FractionalPageItemView 要素は、ページ ビューが開始して、FindItem 要求内のアイテムの最大数が返される場所を説明します。
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760592"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="6a00c-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="6a00c-103">FractionalPageItemView</span></span>

<span data-ttu-id="6a00c-104">**FractionalPageItemView**要素は、ページ ビューが開始して、 [FindItem](finditem.md)要求内のアイテムの最大数が返される場所を説明します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="6a00c-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="6a00c-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="6a00c-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="6a00c-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="6a00c-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="6a00c-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a00c-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a00c-108">Attributes and elements</span></span>

<span data-ttu-id="6a00c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a00c-110">属性</span><span class="sxs-lookup"><span data-stu-id="6a00c-110">Attributes</span></span>

|<span data-ttu-id="6a00c-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="6a00c-111">**Attribute**</span></span>|<span data-ttu-id="6a00c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a00c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6a00c-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="6a00c-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="6a00c-114">[FindItem](finditem.md)応答で返す結果の最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="6a00c-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6a00c-115">This attribute is optional.</span></span> <span data-ttu-id="6a00c-116">この属性を指定しない場合、呼び出しはすべての利用可能な項目を返します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="6a00c-117">**分子**</span><span class="sxs-lookup"><span data-stu-id="6a00c-117">**Numerator**</span></span> <br/> |<span data-ttu-id="6a00c-118">結果セットの先頭からのオフセットを表す分数の分子を表します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="6a00c-119">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-119">This attribute is required.</span></span> <span data-ttu-id="6a00c-120">分子は分母となる以下にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="6a00c-121">この属性は、0 以上である整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="6a00c-122">詳細については、このトピックの後半の「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a00c-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="6a00c-123">**分母**</span><span class="sxs-lookup"><span data-stu-id="6a00c-123">**Denominator**</span></span> <br/> |<span data-ttu-id="6a00c-124">結果セット内のアイテムの合計数の先頭からのオフセットを表す分数の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="6a00c-125">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-125">This attribute is required.</span></span> <span data-ttu-id="6a00c-126">この属性が 1 より大きい整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="6a00c-127">詳細については、このトピックの後半の「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a00c-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6a00c-128">子要素</span><span class="sxs-lookup"><span data-stu-id="6a00c-128">Child elements</span></span>

<span data-ttu-id="6a00c-129">なし。</span><span class="sxs-lookup"><span data-stu-id="6a00c-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a00c-130">親要素</span><span class="sxs-lookup"><span data-stu-id="6a00c-130">Parent elements</span></span>

|<span data-ttu-id="6a00c-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a00c-131">**Element**</span></span>|<span data-ttu-id="6a00c-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a00c-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a00c-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="6a00c-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="6a00c-134">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="6a00c-135">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6a00c-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a00c-136">備考</span><span class="sxs-lookup"><span data-stu-id="6a00c-136">Remarks</span></span>

<span data-ttu-id="6a00c-137">見つかった項目のセットの先頭からのページ ビュー オフセットは、分数で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a00c-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="6a00c-138">分数の**分子**と**分母**の属性によって定義されているは、情報のページを開始する位置について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="6a00c-139">などの**分子**が 4 と等しいし、**分母**を"5"と等しい、エントリで返される情報の開始ページには 5 分の 4 つの結果セットにする方法が配置されています。</span><span class="sxs-lookup"><span data-stu-id="6a00c-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="6a00c-140">割合は、0 に評価されると、結果セットの先頭を示します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="6a00c-141">分数を 1 つに評価する場合、結果セットの末尾を示します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6a00c-142">分数は、ページの開始位置を表す、結果セットにどのように多くの結果が返されます。</span><span class="sxs-lookup"><span data-stu-id="6a00c-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="6a00c-143">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6a00c-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6a00c-144">例</span><span class="sxs-lookup"><span data-stu-id="6a00c-144">Example</span></span>

<span data-ttu-id="6a00c-145">[FindItem](finditem.md)要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="6a00c-146">要求では、検索結果で起動する 2 番目後 3 番目にすべての項目結果セットから項目を返します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="6a00c-147">などの結果セットに 9 つの項目が含まれている場合、ページ ビューは、見つかった項目 3 分の 2 の方法で結果セットから、最大 12 個のアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="6a00c-148">この例では、ページは、7 番目の項目から開始されます。</span><span class="sxs-lookup"><span data-stu-id="6a00c-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="6a00c-149">第 7、8、および 9 番目の項目、ページが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6a00c-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="6a00c-150">分子がゼロに設定されている場合ページ ビューは結果セットの数は、 **MaxEntriesReturned**属性よりも小さい場合に限りすべての項目を返します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6a00c-151">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a00c-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a00c-152">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a00c-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6a00c-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a00c-153">Schema Name</span></span>  <br/> |<span data-ttu-id="6a00c-154">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a00c-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6a00c-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a00c-155">Validation File</span></span>  <br/> |<span data-ttu-id="6a00c-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6a00c-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a00c-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a00c-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a00c-158">False</span><span class="sxs-lookup"><span data-stu-id="6a00c-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a00c-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a00c-159">See also</span></span>



<span data-ttu-id="6a00c-160">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="6a00c-160">[FindItem operation](finditem-operation.md)</span></span>


[<span data-ttu-id="6a00c-161">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="6a00c-161">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

