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
description: ContactsView 要素は、アルファベットの表示名に基づいて連絡先アイテムの検索を定義します。
ms.openlocfilehash: 23c3fe13c44cdd0e5a054ecb3378bc3d633e55aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463819"
---
# <a name="contactsview"></a><span data-ttu-id="5e262-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="5e262-103">ContactsView</span></span>

<span data-ttu-id="5e262-104">**ContactsView**要素は、アルファベットの表示名に基づいて連絡先アイテムの検索を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e262-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="5e262-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="5e262-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="5e262-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="5e262-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="5e262-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="5e262-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5e262-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5e262-108">Attributes and elements</span></span>

<span data-ttu-id="5e262-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5e262-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e262-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e262-110">Attributes</span></span>

|<span data-ttu-id="5e262-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="5e262-111">**Attribute**</span></span>|<span data-ttu-id="5e262-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e262-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e262-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="5e262-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="5e262-114">[FindItem](finditem.md)応答で返される結果の最大数を表します。</span><span class="sxs-lookup"><span data-stu-id="5e262-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="5e262-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="5e262-115">**InitialName**</span></span> <br/> |<span data-ttu-id="5e262-116">応答で返される連絡先リストの最初の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e262-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="5e262-117">指定したイニシャル名が連絡先リストにない場合は、次の名前が**ファイナライズ名**の後にある場合を除いて、文化的コンテキストによって定義された次のアルファベット名が返されます。</span><span class="sxs-lookup"><span data-stu-id="5e262-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="5e262-118">**Initialname**属性が省略されている場合、応答には、連絡先リストの最初の名前から始まる連絡先の一覧が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e262-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="5e262-119">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5e262-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="5e262-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="5e262-120">**FinalName**</span></span> <br/> |<span data-ttu-id="5e262-121">応答で返される連絡先リストの姓を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e262-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="5e262-122">**Finalname**属性が省略されている場合、応答には、指定された並べ替え順序に後続のすべての連絡先が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e262-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="5e262-123">指定した最終名が連絡先リストにない場合は、文化的コンテキストによって定義された次のアルファベット名が除外されます。</span><span class="sxs-lookup"><span data-stu-id="5e262-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="5e262-124">たとえば、FinalName = "Name" (名前が連絡先リストに含まれていない) の場合、Name1 または名前の表示名を持つ連絡先は含まれません。</span><span class="sxs-lookup"><span data-stu-id="5e262-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="5e262-125">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5e262-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5e262-126">子要素</span><span class="sxs-lookup"><span data-stu-id="5e262-126">Child elements</span></span>

<span data-ttu-id="5e262-127">なし。</span><span class="sxs-lookup"><span data-stu-id="5e262-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e262-128">親要素</span><span class="sxs-lookup"><span data-stu-id="5e262-128">Parent elements</span></span>

|<span data-ttu-id="5e262-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="5e262-129">**Element**</span></span>|<span data-ttu-id="5e262-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e262-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e262-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="5e262-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="5e262-132">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e262-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="5e262-133">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e262-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e262-134">注釈</span><span class="sxs-lookup"><span data-stu-id="5e262-134">Remarks</span></span>

<span data-ttu-id="5e262-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5e262-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="5e262-136">例</span><span class="sxs-lookup"><span data-stu-id="5e262-136">Example</span></span>

<span data-ttu-id="5e262-137">次の要求例は、友野司郎の表示名を持つ連絡先から始まる最初の3つの連絡先を検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e262-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="5e262-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5e262-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e262-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e262-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5e262-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5e262-140">Schema Name</span></span>  <br/> |<span data-ttu-id="5e262-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5e262-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5e262-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5e262-142">Validation File</span></span>  <br/> |<span data-ttu-id="5e262-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5e262-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5e262-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5e262-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e262-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="5e262-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e262-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e262-146">See also</span></span>

- <span data-ttu-id="5e262-147">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5e262-147">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="5e262-148">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="5e262-148">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

