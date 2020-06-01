---
title: MoveItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: MoveItem 操作は、1つまたは複数のアイテムを1つの宛先フォルダーに移動するために使用されます。
ms.openlocfilehash: 6a455e483ad2e5c84b91cfaa7562f4f1ec46a112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465682"
---
# <a name="moveitem-operation"></a><span data-ttu-id="c9f93-103">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="c9f93-103">MoveItem operation</span></span>

<span data-ttu-id="c9f93-104">**Moveitem**操作は、1つまたは複数のアイテムを1つの宛先フォルダーに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c9f93-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="c9f93-105">MoveItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="c9f93-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="c9f93-106">説明</span><span class="sxs-lookup"><span data-stu-id="c9f93-106">Description</span></span>

<span data-ttu-id="c9f93-107">次の**Moveitem**要求の例は、アイテムを [下書き] フォルダーに移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c9f93-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c9f93-108">コード</span><span class="sxs-lookup"><span data-stu-id="c9f93-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c9f93-109">コメント</span><span class="sxs-lookup"><span data-stu-id="c9f93-109">Comments</span></span>

<span data-ttu-id="c9f93-110">[ToFolderId](tofolderid.md)要素は、アイテムの移動先のフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9f93-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="c9f93-111">[Itemids](itemids.md)コレクションに一覧表示されているすべての項目は、宛先フォルダーに配置されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c9f93-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="c9f93-112">異なる移動先フォルダーにアイテムを配置するには、個別の**Moveitem**呼び出しを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9f93-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c9f93-113">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c9f93-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="c9f93-114">Request 要素</span><span class="sxs-lookup"><span data-stu-id="c9f93-114">Request elements</span></span>

<span data-ttu-id="c9f93-115">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="c9f93-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c9f93-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="c9f93-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="c9f93-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="c9f93-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="c9f93-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c9f93-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c9f93-119">ItemIds</span><span class="sxs-lookup"><span data-stu-id="c9f93-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="c9f93-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="c9f93-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="c9f93-121">MoveItem 応答の例</span><span class="sxs-lookup"><span data-stu-id="c9f93-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="c9f93-122">説明</span><span class="sxs-lookup"><span data-stu-id="c9f93-122">Description</span></span>

<span data-ttu-id="c9f93-123">次の例は、 **Moveitem**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="c9f93-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="c9f93-124">新しいアイテムのアイテム識別子は、応答メッセージで返されます。</span><span class="sxs-lookup"><span data-stu-id="c9f93-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="c9f93-125">メールボックス間またはメールボックスからパブリックフォルダー **moveitem**操作への応答では、アイテム識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="c9f93-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c9f93-126">コード</span><span class="sxs-lookup"><span data-stu-id="c9f93-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c9f93-127">コメント</span><span class="sxs-lookup"><span data-stu-id="c9f93-127">Comments</span></span>

<span data-ttu-id="c9f93-128">移動が成功した場合、 **Moveitem**操作は成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="c9f93-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="c9f93-129">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="c9f93-129">Successful response elements</span></span>

<span data-ttu-id="c9f93-130">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="c9f93-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c9f93-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c9f93-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c9f93-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="c9f93-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="c9f93-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c9f93-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c9f93-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c9f93-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="c9f93-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c9f93-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c9f93-136">Items</span><span class="sxs-lookup"><span data-stu-id="c9f93-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="c9f93-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9f93-137">See also</span></span>



- [<span data-ttu-id="c9f93-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c9f93-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

