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
description: MoveItem 操作を使用して、1 つまたは複数の項目を単一の宛先フォルダーに移動します。
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832492"
---
# <a name="moveitem-operation"></a><span data-ttu-id="05633-103">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="05633-103">MoveItem operation</span></span>

<span data-ttu-id="05633-104">**MoveItem**操作を使用して、1 つまたは複数の項目を単一の宛先フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="05633-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="05633-105">MoveItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="05633-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="05633-106">説明</span><span class="sxs-lookup"><span data-stu-id="05633-106">Description</span></span>

<span data-ttu-id="05633-107">**MoveItem**要求の次の例では、[下書き] フォルダーにアイテムを移動する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="05633-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="05633-108">コード</span><span class="sxs-lookup"><span data-stu-id="05633-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="05633-109">コメント</span><span class="sxs-lookup"><span data-stu-id="05633-109">Comments</span></span>

<span data-ttu-id="05633-110">[ToFolderId](tofolderid.md)要素は、項目の移動先フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="05633-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="05633-111">[Itemid](itemids.md)コレクション内のすべてのアイテムがコピー先のフォルダー終了することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="05633-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="05633-112">別のインストール先のフォルダーにアイテムを配置するのには別の**MoveItem**呼び出しを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="05633-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="05633-113">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="05633-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="05633-114">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="05633-114">Request elements</span></span>

<span data-ttu-id="05633-115">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="05633-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="05633-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="05633-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="05633-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="05633-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="05633-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="05633-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="05633-119">Itemid</span><span class="sxs-lookup"><span data-stu-id="05633-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="05633-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="05633-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="05633-121">MoveItem 応答の例</span><span class="sxs-lookup"><span data-stu-id="05633-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="05633-122">説明</span><span class="sxs-lookup"><span data-stu-id="05633-122">Description</span></span>

<span data-ttu-id="05633-123">**MoveItem**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="05633-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="05633-124">応答メッセージでは、新しい項目の項目の識別子が返されます。</span><span class="sxs-lookup"><span data-stu-id="05633-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="05633-125">**MoveItem**操作のパブリック フォルダーには、応答間のメールボックスまたはメールボックスのアイテム識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="05633-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="05633-126">コード</span><span class="sxs-lookup"><span data-stu-id="05633-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="05633-127">コメント</span><span class="sxs-lookup"><span data-stu-id="05633-127">Comments</span></span>

<span data-ttu-id="05633-128">移動が成功した場合、 **MoveItem**操作は成功を示します。</span><span class="sxs-lookup"><span data-stu-id="05633-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="05633-129">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="05633-129">Successful response elements</span></span>

<span data-ttu-id="05633-130">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="05633-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="05633-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="05633-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="05633-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="05633-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="05633-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="05633-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="05633-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="05633-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="05633-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="05633-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="05633-136">Items</span><span class="sxs-lookup"><span data-stu-id="05633-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="05633-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="05633-137">See also</span></span>



- [<span data-ttu-id="05633-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="05633-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

