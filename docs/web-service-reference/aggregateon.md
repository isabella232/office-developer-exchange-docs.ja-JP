---
title: AggregateOn
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: AggregateOn 要素は、グループ化された FindItem 結果セットをグループ化した項目の順序を決定するために使用されるプロパティを表します。
ms.openlocfilehash: fe14de23e6a4c90d826200cae927427acfccc3c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759305"
---
# <a name="aggregateon"></a><span data-ttu-id="d13ca-103">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="d13ca-103">AggregateOn</span></span>

<span data-ttu-id="d13ca-104">**AggregateOn**要素は、グループ化された FindItem 結果セットをグループ化した項目の順序を決定するために使用されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-104">The **AggregateOn** element represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span> 
  
- [<span data-ttu-id="d13ca-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="d13ca-105">FindItem</span></span>](finditem.md)  
- [<span data-ttu-id="d13ca-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="d13ca-106">GroupBy</span></span>](groupby.md)
- [<span data-ttu-id="d13ca-107">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="d13ca-107">AggregateOn</span></span>](aggregateon.md)
  
```xml
<AggregateOn>
   <FieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <IndexedFieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <ExtendedFieldURI/>
</AggregateOn>
```
 
<span data-ttu-id="d13ca-108">**AggregateOnType**</span><span class="sxs-lookup"><span data-stu-id="d13ca-108">**AggregateOnType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d13ca-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d13ca-109">Attributes and elements</span></span>

<span data-ttu-id="d13ca-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d13ca-111">属性</span><span class="sxs-lookup"><span data-stu-id="d13ca-111">Attributes</span></span>

|<span data-ttu-id="d13ca-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="d13ca-112">**Attribute**</span></span>|<span data-ttu-id="d13ca-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="d13ca-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d13ca-114">**Aggregate**</span><span class="sxs-lookup"><span data-stu-id="d13ca-114">**Aggregate**</span></span> <br/> | <span data-ttu-id="d13ca-115">アイテムのグループの順序付けに使用される[FieldURI](fielduri.md)要素によって識別されるプロパティの最大値または最小値を示します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-115">Indicates the maximum or minimum value of the property identified by the [FieldURI](fielduri.md) element that is used for ordering the groups of items.</span></span><br/><br/><span data-ttu-id="d13ca-116">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="d13ca-116">The following are the possible values:</span></span>  <br/><br/><span data-ttu-id="d13ca-117">-最小値</span><span class="sxs-lookup"><span data-stu-id="d13ca-117">- Minimum</span></span>  <br/><span data-ttu-id="d13ca-118">-最大</span><span class="sxs-lookup"><span data-stu-id="d13ca-118">- Maximum</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d13ca-119">子要素</span><span class="sxs-lookup"><span data-stu-id="d13ca-119">Child elements</span></span>

|<span data-ttu-id="d13ca-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d13ca-120">**Element**</span></span>|<span data-ttu-id="d13ca-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d13ca-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d13ca-122">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d13ca-122">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d13ca-123">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-123">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d13ca-124">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d13ca-124">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d13ca-125">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-125">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="d13ca-126">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d13ca-126">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d13ca-127">取得、設定、または作成する拡張の MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-127">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d13ca-128">親要素</span><span class="sxs-lookup"><span data-stu-id="d13ca-128">Parent elements</span></span>

|<span data-ttu-id="d13ca-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="d13ca-129">**Element**</span></span>|<span data-ttu-id="d13ca-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="d13ca-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d13ca-131">GroupBy</span><span class="sxs-lookup"><span data-stu-id="d13ca-131">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="d13ca-132">FindItem クエリの任意のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-132">Specifies arbitrary groupings for FindItem queries.</span></span>  <br/> <span data-ttu-id="d13ca-133">この要素への XPath 式は、次のようにします。`/FindItem/GroupBy`</span><span class="sxs-lookup"><span data-stu-id="d13ca-133">The following is the XPath expression to this element:  `/FindItem/GroupBy`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d13ca-134">備考</span><span class="sxs-lookup"><span data-stu-id="d13ca-134">Remarks</span></span>

<span data-ttu-id="d13ca-135">[FindItem 操作](finditem-operation.md)では、グループ化された結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-135">The [FindItem operation](finditem-operation.md) can return grouped results.</span></span> <span data-ttu-id="d13ca-136">グループ化された結果を指定したグループ化のプロパティに対して同じ値を持つすべての項目がまとめし、そのグループの子として表示されます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-136">Within grouped results, all items that have the same value for a given grouping property are gathered together and presented as children of that group.</span></span> <span data-ttu-id="d13ca-137">たとえば、送信者をグループ化する場合すべてのメールは送信者 A、B、送信側に、いるかどうかに基づいて別のグループに編成されています。</span><span class="sxs-lookup"><span data-stu-id="d13ca-137">For example, if you group by sender, all e-mails are organized into separate groups based on whether they are from sender A, sender B, and so on.</span></span> <span data-ttu-id="d13ca-138">これらのグループは、送信者のグループの子です。</span><span class="sxs-lookup"><span data-stu-id="d13ca-138">These groups are children of the sender group.</span></span> 
  
<span data-ttu-id="d13ca-139">送信者グループ内のグループのそれぞれには、実際の送信者から送信された電子メールなどの項目のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d13ca-139">Each of the groups within the sender group contains a collection of items, such as the actual e-mails that came from each sender.</span></span> <span data-ttu-id="d13ca-140">グループ内のアイテムを並べ替えるには、[並べ替え順序](sortorder.md)の要素を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-140">You can use the [SortOrder](sortorder.md) element to sort the items within a group.</span></span> <span data-ttu-id="d13ca-141">ただし、アイテムのプロパティの値に基づいてグループを並べ替えるには、集計を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d13ca-141">To sort the groups based on an item's property values, however, you must use aggregation.</span></span> 
  
<span data-ttu-id="d13ca-142">集約、グループの順序は、グループ内のアイテムの特定のプロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="d13ca-142">With aggregation, the order of groups is based on a specific property of the items within the group.</span></span> <span data-ttu-id="d13ca-143">集計を使用して、グループ内のアイテムを並べ替えるには、グループの並べ替えに使用する代表的なプロパティを識別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d13ca-143">When you use aggregation to sort items within a group, you must identify a representative property by which to sort the groups.</span></span> <span data-ttu-id="d13ca-144">**AggregateOn**要素を使用すると、代表的なプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-144">You can use the **AggregateOn** element to specify the representative property.</span></span> 
  
<span data-ttu-id="d13ca-145">代表的なプロパティを識別すると、**集計**属性が最大値または特定のプロパティの最小値のグループを並べ替えるかどうかを示すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-145">When a representative property is identified, the **Aggregate** attribute is used to indicate whether the groups are sorted according to the maximum or the minimum value of the identified property.</span></span> <span data-ttu-id="d13ca-146">**集計**属性は、最大値に設定されている場合、 **AggregateOn**プロパティの最大値で始まるグループが並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-146">If the **Aggregate** attribute is set to Maximum, the groups are sorted beginning with the largest value for the **AggregateOn** property.</span></span> <span data-ttu-id="d13ca-147">**集計**属性は、最小値に設定されている場合、 **AggregateOn**プロパティの最小値で始まるグループが並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-147">If the **Aggregate** attribute is set to Minimum, the groups are sorted beginning with the smallest value for the **AggregateOn** property.</span></span> 
  
<span data-ttu-id="d13ca-148">など、送信者別にグループ化 FindItem のグループ化されたクエリを発行する場合は、最新の電子メール メッセージのグループが上になるようにグループを注文することができますによってグループ化する送信者と集計、**集計**を受信した日付と時刻の最大値の属性です。</span><span class="sxs-lookup"><span data-stu-id="d13ca-148">For example, if you want to issue a FindItem grouped query, grouping by sender, but you want to order the groups so that the group with the most recent e-mail message is on top, you can group by sender and aggregate on date/time received with an **Aggregate** attribute of Maximum.</span></span> 
  
<span data-ttu-id="d13ca-149">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d13ca-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="d13ca-150">例</span><span class="sxs-lookup"><span data-stu-id="d13ca-150">Example</span></span>

<span data-ttu-id="d13ca-151">次の例では、グループ化された FindItem 要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-151">The following example shows a grouped FindItem request and response.</span></span> <span data-ttu-id="d13ca-152">**ConversationTopic**プロパティでグループ化された項目を返す要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d13ca-152">The example shows a request to return items grouped by the **ConversationTopic** property.</span></span> <span data-ttu-id="d13ca-153">A と B の 2 つのグループは、 [DateTimeReceived](datetimereceived.md)プロパティの最大値に基づく順序を降順で返されます。</span><span class="sxs-lookup"><span data-stu-id="d13ca-153">Two groups, A and B, are returned in descending order based on the maximum value of the [DateTimeReceived](datetimereceived.md) property.</span></span> 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="message:ConversationTopic"/>
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AdditionalProperties>    
      </ItemShape>
      <IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="20" Offset="0"/>
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="message:ConversationTopic"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
<!-- EXAMPLE RESPONSE -->
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>B</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAH=" ChangeKey="CQAAABY" />
                    <t:DateTimeReceived>2006-09-14T23:59:18Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnAHR=" ChangeKey="CQAAAw" />
                    <t:DateTimeReceived>2006-09-15T00:00:24Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnA==" ChangeKey="CQAAJXT" />
                    <t:DateTimeReceived>2006-09-15T00:22:45Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>A</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAAA==" ChangeKey="CQCJNe" />
                    <t:DateTimeReceived>2006-09-14T23:56:12Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQWgAA==" ChangeKey="CQAACJV6" />
                    <t:DateTimeReceived>2006-09-14T23:57:33Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAAA==" ChangeKey="CQA6CJXw" />
                    <t:DateTimeReceived>2006-09-15T00:23:31Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d13ca-154">グループ内のアイテムを並べ替えるには、[並べ替え順序](sortorder.md)の要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-154">To sort the items in a group, use the [SortOrder](sortorder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d13ca-155">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d13ca-155">The item identifiers and change keys have been shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d13ca-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="d13ca-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d13ca-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="d13ca-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d13ca-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d13ca-158">Schema Name</span></span>  <br/> |<span data-ttu-id="d13ca-159">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d13ca-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="d13ca-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d13ca-160">Validation File</span></span>  <br/> |<span data-ttu-id="d13ca-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d13ca-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d13ca-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d13ca-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="d13ca-163">False</span><span class="sxs-lookup"><span data-stu-id="d13ca-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d13ca-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="d13ca-164">See also</span></span>

- <span data-ttu-id="d13ca-165">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="d13ca-165">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="d13ca-166">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d13ca-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d13ca-167">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="d13ca-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

