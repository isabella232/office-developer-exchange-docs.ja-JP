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
description: AggregateOn 要素は、グループ化された FindItem 結果セットのグループ化されたアイテムの順序を決定するために使用されるプロパティを表します。
ms.openlocfilehash: 04359c187ef11538d64f8f0d3ea2fe84bc3d048b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463567"
---
# <a name="aggregateon"></a><span data-ttu-id="56d5b-103">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="56d5b-103">AggregateOn</span></span>

<span data-ttu-id="56d5b-104">**AggregateOn**要素は、グループ化された FindItem 結果セットのグループ化されたアイテムの順序を決定するために使用されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-104">The **AggregateOn** element represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span> 
  
- [<span data-ttu-id="56d5b-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="56d5b-105">FindItem</span></span>](finditem.md)  
- [<span data-ttu-id="56d5b-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="56d5b-106">GroupBy</span></span>](groupby.md)
- [<span data-ttu-id="56d5b-107">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="56d5b-107">AggregateOn</span></span>](aggregateon.md)
  
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
 
<span data-ttu-id="56d5b-108">**AggregateOnType**</span><span class="sxs-lookup"><span data-stu-id="56d5b-108">**AggregateOnType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="56d5b-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56d5b-109">Attributes and elements</span></span>

<span data-ttu-id="56d5b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56d5b-111">属性</span><span class="sxs-lookup"><span data-stu-id="56d5b-111">Attributes</span></span>

|<span data-ttu-id="56d5b-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="56d5b-112">**Attribute**</span></span>|<span data-ttu-id="56d5b-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="56d5b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56d5b-114">**Aggregate**</span><span class="sxs-lookup"><span data-stu-id="56d5b-114">**Aggregate**</span></span> <br/> | <span data-ttu-id="56d5b-115">アイテムのグループの順序付けに使用される[FieldURI](fielduri.md)要素によって識別されるプロパティの最大値または最小値を示します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-115">Indicates the maximum or minimum value of the property identified by the [FieldURI](fielduri.md) element that is used for ordering the groups of items.</span></span><br/><br/><span data-ttu-id="56d5b-116">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="56d5b-116">The following are the possible values:</span></span>  <br/><br/><span data-ttu-id="56d5b-117">-最小</span><span class="sxs-lookup"><span data-stu-id="56d5b-117">- Minimum</span></span>  <br/><span data-ttu-id="56d5b-118">-最大</span><span class="sxs-lookup"><span data-stu-id="56d5b-118">- Maximum</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="56d5b-119">子要素</span><span class="sxs-lookup"><span data-stu-id="56d5b-119">Child elements</span></span>

|<span data-ttu-id="56d5b-120">**Element**</span><span class="sxs-lookup"><span data-stu-id="56d5b-120">**Element**</span></span>|<span data-ttu-id="56d5b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="56d5b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56d5b-122">FieldURI</span><span class="sxs-lookup"><span data-stu-id="56d5b-122">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="56d5b-123">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-123">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="56d5b-124">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="56d5b-124">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="56d5b-125">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-125">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="56d5b-126">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="56d5b-126">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="56d5b-127">取得、設定、または作成する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-127">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56d5b-128">親要素</span><span class="sxs-lookup"><span data-stu-id="56d5b-128">Parent elements</span></span>

|<span data-ttu-id="56d5b-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="56d5b-129">**Element**</span></span>|<span data-ttu-id="56d5b-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="56d5b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56d5b-131">GroupBy</span><span class="sxs-lookup"><span data-stu-id="56d5b-131">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="56d5b-132">FindItem クエリの任意のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-132">Specifies arbitrary groupings for FindItem queries.</span></span>  <br/> <span data-ttu-id="56d5b-133">この要素の XPath 式を次に示します。`/FindItem/GroupBy`</span><span class="sxs-lookup"><span data-stu-id="56d5b-133">The following is the XPath expression to this element:  `/FindItem/GroupBy`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56d5b-134">注釈</span><span class="sxs-lookup"><span data-stu-id="56d5b-134">Remarks</span></span>

<span data-ttu-id="56d5b-135">[FindItem 操作](finditem-operation.md)は、グループ化された結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-135">The [FindItem operation](finditem-operation.md) can return grouped results.</span></span> <span data-ttu-id="56d5b-136">グループ化された結果内で、特定のグループ化プロパティの値が同じであるすべてのアイテムが一緒に収集され、そのグループの子として表示されます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-136">Within grouped results, all items that have the same value for a given grouping property are gathered together and presented as children of that group.</span></span> <span data-ttu-id="56d5b-137">たとえば、送信者によってグループ化した場合、すべての電子メールは送信者 A、送信者 B のどちらからの場合でも、別のグループに整理されます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-137">For example, if you group by sender, all e-mails are organized into separate groups based on whether they are from sender A, sender B, and so on.</span></span> <span data-ttu-id="56d5b-138">これらのグループは、送信者グループの子です。</span><span class="sxs-lookup"><span data-stu-id="56d5b-138">These groups are children of the sender group.</span></span> 
  
<span data-ttu-id="56d5b-139">Sender グループ内の各グループには、各送信者から送られた実際の電子メールなど、アイテムのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="56d5b-139">Each of the groups within the sender group contains a collection of items, such as the actual e-mails that came from each sender.</span></span> <span data-ttu-id="56d5b-140">並べ替え[順序](sortorder.md)要素を使用して、グループ内のアイテムを並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-140">You can use the [SortOrder](sortorder.md) element to sort the items within a group.</span></span> <span data-ttu-id="56d5b-141">ただし、アイテムのプロパティ値に基づいてグループを並べ替えるには、aggregation を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56d5b-141">To sort the groups based on an item's property values, however, you must use aggregation.</span></span> 
  
<span data-ttu-id="56d5b-142">集約では、グループの順序は、グループ内のアイテムの特定のプロパティに基づきます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-142">With aggregation, the order of groups is based on a specific property of the items within the group.</span></span> <span data-ttu-id="56d5b-143">集約を使用してグループ内のアイテムを並べ替える場合は、グループを並べ替えるための代表的なプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56d5b-143">When you use aggregation to sort items within a group, you must identify a representative property by which to sort the groups.</span></span> <span data-ttu-id="56d5b-144">**AggregateOn**要素を使用して、典型的なプロパティを指定できます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-144">You can use the **AggregateOn** element to specify the representative property.</span></span> 
  
<span data-ttu-id="56d5b-145">代表的なプロパティを指定すると、**集計**属性を使用して、グループが、識別されたプロパティの最大値または最小値に従って並べ替えられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-145">When a representative property is identified, the **Aggregate** attribute is used to indicate whether the groups are sorted according to the maximum or the minimum value of the identified property.</span></span> <span data-ttu-id="56d5b-146">**Aggregate**属性が [最大] に設定されている場合、グループは**AggregateOn**プロパティの最大値を先頭に並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-146">If the **Aggregate** attribute is set to Maximum, the groups are sorted beginning with the largest value for the **AggregateOn** property.</span></span> <span data-ttu-id="56d5b-147">**Aggregate**属性が [最小] に設定されている場合、グループは**AggregateOn**プロパティの最小値を先頭に並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-147">If the **Aggregate** attribute is set to Minimum, the groups are sorted beginning with the smallest value for the **AggregateOn** property.</span></span> 
  
<span data-ttu-id="56d5b-148">たとえば、sender でグループ化されたクエリを発行する場合に、最新の電子メールメッセージが一番上になるようにグループの順序を指定する場合は、送信者によってグループ化し、**集約**属性が [最大] で受信した日付/時刻を集計することができます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-148">For example, if you want to issue a FindItem grouped query, grouping by sender, but you want to order the groups so that the group with the most recent e-mail message is on top, you can group by sender and aggregate on date/time received with an **Aggregate** attribute of Maximum.</span></span> 
  
<span data-ttu-id="56d5b-149">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="56d5b-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="56d5b-150">例</span><span class="sxs-lookup"><span data-stu-id="56d5b-150">Example</span></span>

<span data-ttu-id="56d5b-151">次の例は、グループ化された FindItem 要求と応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="56d5b-151">The following example shows a grouped FindItem request and response.</span></span> <span data-ttu-id="56d5b-152">この例では、 **ConversationTopic**プロパティによってグループ化されたアイテムを返す要求を示します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-152">The example shows a request to return items grouped by the **ConversationTopic** property.</span></span> <span data-ttu-id="56d5b-153">2つのグループ A と B は、 [DateTimeReceived](datetimereceived.md)プロパティの最大値に基づいて、降順で返されます。</span><span class="sxs-lookup"><span data-stu-id="56d5b-153">Two groups, A and B, are returned in descending order based on the maximum value of the [DateTimeReceived](datetimereceived.md) property.</span></span> 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="56d5b-154">グループ内のアイテムを並べ替えるには、並べ替え[順序](sortorder.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="56d5b-154">To sort the items in a group, use the [SortOrder](sortorder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="56d5b-155">読みやすくするために、アイテムの識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="56d5b-155">The item identifiers and change keys have been shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="56d5b-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="56d5b-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56d5b-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="56d5b-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56d5b-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56d5b-158">Schema Name</span></span>  <br/> |<span data-ttu-id="56d5b-159">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="56d5b-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="56d5b-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56d5b-160">Validation File</span></span>  <br/> |<span data-ttu-id="56d5b-161">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="56d5b-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56d5b-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="56d5b-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="56d5b-163">正しくない</span><span class="sxs-lookup"><span data-stu-id="56d5b-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56d5b-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="56d5b-164">See also</span></span>

- [<span data-ttu-id="56d5b-165">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="56d5b-165">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="56d5b-166">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="56d5b-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="56d5b-167">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="56d5b-167">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

