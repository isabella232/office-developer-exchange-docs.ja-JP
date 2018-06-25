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
description: IndexedPageItemView 要素は、ページがどのように会話を説明または FindItem 操作または FindConversation 操作の要求の情報が返される項目です。
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831919"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="cbcc6-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="cbcc6-103">IndexedPageItemView</span></span>

<span data-ttu-id="cbcc6-104">**IndexedPageItemView**要素は、ページがどのように会話を説明または[FindItem 操作](finditem-operation.md)または[FindConversation 操作](findconversation-operation.md)の要求の情報が返される項目です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="cbcc6-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbcc6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cbcc6-106">Attributes and elements</span></span>

<span data-ttu-id="cbcc6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbcc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbcc6-108">Attributes</span></span>

|<span data-ttu-id="cbcc6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-109">**Attribute**</span></span>|<span data-ttu-id="cbcc6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cbcc6-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="cbcc6-112">アイテムや会話の応答を返すの最大数について説明します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="cbcc6-113">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="cbcc6-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-114">**Offset**</span></span> <br/> |<span data-ttu-id="cbcc6-115">**ベース ポイント**からのオフセットを示します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="cbcc6-116">**ベース ポイント**と等しい場合、開始オフセットが正の数値です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="cbcc6-117">**ベース ポイント**が終了する場合、オフセットが負の場合と処理されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="cbcc6-118">どの項目を識別または会話の応答で配信される最初になります。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="cbcc6-119">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cbcc6-120">**ベース ポイント**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="cbcc6-121">項目やテーマのページを一連の項目または検索条件を使用して検出された会話の前後から開始されるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="cbcc6-122">末尾からのシークを常に検索を進めます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="cbcc6-123">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="cbcc6-124">ベース ポイントの属性</span><span class="sxs-lookup"><span data-stu-id="cbcc6-124">BasePoint Attribute</span></span>

|<span data-ttu-id="cbcc6-125">**値**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-125">**Value**</span></span>|<span data-ttu-id="cbcc6-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cbcc6-127">先頭</span><span class="sxs-lookup"><span data-stu-id="cbcc6-127">Beginning</span></span>  <br/> |<span data-ttu-id="cbcc6-128">ページ ビューでは、会話やアイテムの検索結果セットの先頭から開始されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="cbcc6-129">終了</span><span class="sxs-lookup"><span data-stu-id="cbcc6-129">End</span></span>  <br/> |<span data-ttu-id="cbcc6-130">ページ ビューは、見つかった会話やアイテム セットの末尾から開始します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cbcc6-131">子要素</span><span class="sxs-lookup"><span data-stu-id="cbcc6-131">Child elements</span></span>

<span data-ttu-id="cbcc6-132">なし。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbcc6-133">親要素</span><span class="sxs-lookup"><span data-stu-id="cbcc6-133">Parent elements</span></span>

|<span data-ttu-id="cbcc6-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-134">**Element**</span></span>|<span data-ttu-id="cbcc6-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbcc6-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbcc6-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="cbcc6-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="cbcc6-137">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="cbcc6-138">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="cbcc6-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="cbcc6-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="cbcc6-140">メールボックス内の会話を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cbcc6-141">備考</span><span class="sxs-lookup"><span data-stu-id="cbcc6-141">Remarks</span></span>

<span data-ttu-id="cbcc6-142">末尾からのシークでは、オフセットによって識別される原点に移動します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="cbcc6-143">さらに、ポインターが再び要求されたレコードの数によって。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="cbcc6-144">などの場合は 100 個のレコードがある、オフセットが末尾から 25、75 から検索を開始します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="cbcc6-145">10 個のレコードが返された場合ポインターが逆方向、さらに 10 が 65 を記録し、65 75 からのレコードを返します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="cbcc6-146">次のインデックスは、64 です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-146">The next index is 64.</span></span> <span data-ttu-id="cbcc6-147">ページの末尾からの次のオフセットは、100-36 に相当する 64 です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="cbcc6-148">36 は、次のインデックス付きのページを取得する、末尾からの次のオフセットの値です。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="cbcc6-149">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="cbcc6-150">例</span><span class="sxs-lookup"><span data-stu-id="cbcc6-150">Example</span></span>

<span data-ttu-id="cbcc6-151">[FindItem 操作](finditem-operation.md)要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="cbcc6-152">ID とトピックは、各項目が返されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="cbcc6-153">最大六つのアイテムは、 **MaxEntriesReturned**属性で指定されている、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="cbcc6-154">アイテムは、重要度別にグループ化の順序を昇順に表示されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="cbcc6-155">グループ内のアイテムは、件名ごとに集約されます。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
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

## <a name="element-information"></a><span data-ttu-id="cbcc6-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="cbcc6-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbcc6-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="cbcc6-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cbcc6-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cbcc6-158">Schema Name</span></span>  <br/> |<span data-ttu-id="cbcc6-159">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cbcc6-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cbcc6-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cbcc6-160">Validation File</span></span>  <br/> |<span data-ttu-id="cbcc6-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cbcc6-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cbcc6-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cbcc6-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="cbcc6-163">False</span><span class="sxs-lookup"><span data-stu-id="cbcc6-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbcc6-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbcc6-164">See also</span></span>



<span data-ttu-id="cbcc6-165">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="cbcc6-165">[FindItem operation](finditem-operation.md)</span></span>
  
<span data-ttu-id="cbcc6-166">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="cbcc6-166">[FindConversation operation](findconversation-operation.md)</span></span>


[<span data-ttu-id="cbcc6-167">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="cbcc6-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

