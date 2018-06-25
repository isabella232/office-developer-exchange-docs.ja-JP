---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: ContactsView 要素は、連絡先アイテムをアルファベット順の表示名を基に検索を定義します。
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759694"
---
# <a name="contactsview"></a><span data-ttu-id="33162-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="33162-103">ContactsView</span></span>

<span data-ttu-id="33162-104">**ContactsView**要素は、連絡先アイテムをアルファベット順の表示名を基に検索を定義します。</span><span class="sxs-lookup"><span data-stu-id="33162-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="33162-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="33162-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="33162-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="33162-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="33162-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="33162-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="33162-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="33162-108">Attributes and elements</span></span>

<span data-ttu-id="33162-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33162-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33162-110">属性</span><span class="sxs-lookup"><span data-stu-id="33162-110">Attributes</span></span>

|<span data-ttu-id="33162-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="33162-111">**Attribute**</span></span>|<span data-ttu-id="33162-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="33162-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33162-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="33162-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="33162-114">[FindItem](finditem.md)応答で返す結果の最大数について説明します。</span><span class="sxs-lookup"><span data-stu-id="33162-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="33162-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="33162-115">**InitialName**</span></span> <br/> |<span data-ttu-id="33162-116">応答を取得する [連絡先] リストで、最初の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="33162-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="33162-117">指定の最初の名前は次のアルファベット順の名前、アドレス帳の文化のコンテキストで定義されている場合が返されます、次の名前が**FinalName**の後に来る場合を除く。</span><span class="sxs-lookup"><span data-stu-id="33162-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="33162-118">**InitialName**属性を省略すると、応答には、アドレス帳の最初の名前で始まる連絡先の一覧が含まれます。</span><span class="sxs-lookup"><span data-stu-id="33162-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="33162-119">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="33162-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="33162-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="33162-120">**FinalName**</span></span> <br/> |<span data-ttu-id="33162-121">応答を取得する連絡先リストの最後の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="33162-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="33162-122">**FinalName**属性を省略すると、応答には、指定した並べ替え順序内のすべての後続の連絡先が含まれます。</span><span class="sxs-lookup"><span data-stu-id="33162-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="33162-123">指定された最終的な名前でない場合、[連絡先] ボックスの一覧で、次のアルファベット順の名前文化のコンテキストで定義されている除外されます。</span><span class="sxs-lookup"><span data-stu-id="33162-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="33162-124">などの場合は FinalName =「名前」、名が連絡先リストではありませんが、設定されている連絡先は、Name1 の名前を表示または、名は含まれません。</span><span class="sxs-lookup"><span data-stu-id="33162-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="33162-125">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="33162-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="33162-126">子要素</span><span class="sxs-lookup"><span data-stu-id="33162-126">Child elements</span></span>

<span data-ttu-id="33162-127">なし。</span><span class="sxs-lookup"><span data-stu-id="33162-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33162-128">親要素</span><span class="sxs-lookup"><span data-stu-id="33162-128">Parent elements</span></span>

|<span data-ttu-id="33162-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="33162-129">**Element**</span></span>|<span data-ttu-id="33162-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="33162-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33162-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="33162-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="33162-132">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="33162-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="33162-133">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="33162-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33162-134">備考</span><span class="sxs-lookup"><span data-stu-id="33162-134">Remarks</span></span>

<span data-ttu-id="33162-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="33162-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="33162-136">例</span><span class="sxs-lookup"><span data-stu-id="33162-136">Example</span></span>

<span data-ttu-id="33162-137">要求の次の例では、友野司郎の表示名を持つ連絡先を開始する最初の 3 つの連絡先を検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="33162-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
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
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="33162-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="33162-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33162-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="33162-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33162-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33162-140">Schema Name</span></span>  <br/> |<span data-ttu-id="33162-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="33162-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="33162-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33162-142">Validation File</span></span>  <br/> |<span data-ttu-id="33162-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33162-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33162-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="33162-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="33162-145">False</span><span class="sxs-lookup"><span data-stu-id="33162-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33162-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="33162-146">See also</span></span>

- <span data-ttu-id="33162-147">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="33162-147">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="33162-148">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="33162-148">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

