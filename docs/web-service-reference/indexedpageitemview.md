---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: IndexedPageItemView 要素は、ページ化された会話またはアイテム情報が FindItem 操作または FindConversation 操作要求に対してどのように返されるかを表します。
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456914"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="845f2-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="845f2-103">IndexedPageItemView</span></span>

<span data-ttu-id="845f2-104">**Indexedpageitemview**要素は、ページ化された会話またはアイテム情報が[FindItem 操作](finditem-operation.md)または[findconversation 操作](findconversation-operation.md)要求に対してどのように返されるかを表します。</span><span class="sxs-lookup"><span data-stu-id="845f2-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="845f2-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="845f2-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="845f2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="845f2-106">Attributes and elements</span></span>

<span data-ttu-id="845f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="845f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="845f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="845f2-108">Attributes</span></span>

|<span data-ttu-id="845f2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="845f2-109">**Attribute**</span></span>|<span data-ttu-id="845f2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="845f2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="845f2-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="845f2-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="845f2-112">応答で返されるアイテムまたはスレッドの最大数を表します。</span><span class="sxs-lookup"><span data-stu-id="845f2-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="845f2-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="845f2-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="845f2-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="845f2-114">**Offset**</span></span> <br/> |<span data-ttu-id="845f2-115">**BasePoint**からのオフセットを記述します。</span><span class="sxs-lookup"><span data-stu-id="845f2-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="845f2-116">**BasePoint**が先頭と等しい場合、オフセットは正になります。</span><span class="sxs-lookup"><span data-stu-id="845f2-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="845f2-117">**BasePoint**が End と等しい場合、オフセットは負の値として処理されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="845f2-118">これにより、応答で最初に配信されるアイテムまたは会話が特定されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="845f2-119">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="845f2-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="845f2-120">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="845f2-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="845f2-121">アイテムまたはスレッドのページが、検索条件を使用して検出されたアイテムまたは会話のセットの先頭または末尾から開始するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="845f2-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="845f2-122">末尾からシークすると、常に逆方向に検索されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="845f2-123">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="845f2-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="845f2-124">BasePoint 属性</span><span class="sxs-lookup"><span data-stu-id="845f2-124">BasePoint Attribute</span></span>

|<span data-ttu-id="845f2-125">**値**</span><span class="sxs-lookup"><span data-stu-id="845f2-125">**Value**</span></span>|<span data-ttu-id="845f2-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="845f2-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="845f2-127">始まる</span><span class="sxs-lookup"><span data-stu-id="845f2-127">Beginning</span></span>  <br/> |<span data-ttu-id="845f2-128">ページビューは、検出されたスレッドまたはアイテムセットの先頭から開始されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="845f2-129">End</span><span class="sxs-lookup"><span data-stu-id="845f2-129">End</span></span>  <br/> |<span data-ttu-id="845f2-130">ページビューは、検出されたスレッドまたはアイテムセットの末尾から開始されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="845f2-131">子要素</span><span class="sxs-lookup"><span data-stu-id="845f2-131">Child elements</span></span>

<span data-ttu-id="845f2-132">なし。</span><span class="sxs-lookup"><span data-stu-id="845f2-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="845f2-133">親要素</span><span class="sxs-lookup"><span data-stu-id="845f2-133">Parent elements</span></span>

|<span data-ttu-id="845f2-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="845f2-134">**Element**</span></span>|<span data-ttu-id="845f2-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="845f2-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="845f2-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="845f2-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="845f2-137">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="845f2-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="845f2-138">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="845f2-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="845f2-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="845f2-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="845f2-140">メールボックス内のスレッドを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="845f2-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="845f2-141">注釈</span><span class="sxs-lookup"><span data-stu-id="845f2-141">Remarks</span></span>

<span data-ttu-id="845f2-142">最後からシークするには、オフセットで識別される原点への移動が必要になります。</span><span class="sxs-lookup"><span data-stu-id="845f2-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="845f2-143">さらに、要求されたレコードの数だけポインターが戻されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="845f2-144">たとえば、100レコードがあり、オフセットが最後から25である場合、検索は75から開始されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="845f2-145">10件のレコードが返された場合、ポインターは10レコード後ろに65に移動され、レコード 65 ~ 75 を返します。</span><span class="sxs-lookup"><span data-stu-id="845f2-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="845f2-146">次のインデックスは64です。</span><span class="sxs-lookup"><span data-stu-id="845f2-146">The next index is 64.</span></span> <span data-ttu-id="845f2-147">ページの最後からの次のオフセットは、36と等しい 100-64 です。</span><span class="sxs-lookup"><span data-stu-id="845f2-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="845f2-148">36は、次のインデックスページを取得するために末尾からの次のオフセットの値です。</span><span class="sxs-lookup"><span data-stu-id="845f2-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="845f2-149">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="845f2-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="845f2-150">例</span><span class="sxs-lookup"><span data-stu-id="845f2-150">Example</span></span>

<span data-ttu-id="845f2-151">次の例は、 [FindItem 操作](finditem-operation.md)要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="845f2-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="845f2-152">各アイテムは、ID と subject で返されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="845f2-153">応答では、 **maxん返さ**れた属性によって指定されているように、最大6つのアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="845f2-154">アイテムは重要度別にグループ化されて昇順に表示されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="845f2-155">グループ内のアイテムは、件名によって集約されます。</span><span class="sxs-lookup"><span data-stu-id="845f2-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
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
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
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

## <a name="element-information"></a><span data-ttu-id="845f2-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="845f2-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="845f2-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="845f2-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="845f2-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="845f2-158">Schema Name</span></span>  <br/> |<span data-ttu-id="845f2-159">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="845f2-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="845f2-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="845f2-160">Validation File</span></span>  <br/> |<span data-ttu-id="845f2-161">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="845f2-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="845f2-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="845f2-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="845f2-163">正しくない</span><span class="sxs-lookup"><span data-stu-id="845f2-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="845f2-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="845f2-164">See also</span></span>



[<span data-ttu-id="845f2-165">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="845f2-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="845f2-166">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="845f2-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="845f2-167">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="845f2-167">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

