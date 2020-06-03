---
title: CopyItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: CopyItem 操作は、アイテムをコピーし、アイテムを別のフォルダーに配置します。
ms.openlocfilehash: ec07700a5ebbdc8774aa2134919634b8dfd02406
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462179"
---
# <a name="copyitem-operation"></a><span data-ttu-id="92e22-103">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="92e22-103">CopyItem operation</span></span>

<span data-ttu-id="92e22-104">**Copyitem**操作は、アイテムをコピーし、アイテムを別のフォルダーに配置します。</span><span class="sxs-lookup"><span data-stu-id="92e22-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="92e22-105">CopyItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="92e22-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="92e22-106">Description</span><span class="sxs-lookup"><span data-stu-id="92e22-106">Description</span></span>

<span data-ttu-id="92e22-107">次の**Copyitem**要求の例は、受信トレイにアイテムをコピーする要求を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="92e22-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="92e22-108">コード</span><span class="sxs-lookup"><span data-stu-id="92e22-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="92e22-109">コメント</span><span class="sxs-lookup"><span data-stu-id="92e22-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="92e22-110">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="92e22-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="92e22-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="92e22-111">Request elements</span></span>

<span data-ttu-id="92e22-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="92e22-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="92e22-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="92e22-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="92e22-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="92e22-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="92e22-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="92e22-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="92e22-116">ItemIds</span><span class="sxs-lookup"><span data-stu-id="92e22-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="92e22-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="92e22-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="92e22-118">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="92e22-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="92e22-119">**Copyitem**操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92e22-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="92e22-120">[Copyitem](copyitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="92e22-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="92e22-121">成功した CopyItem 応答</span><span class="sxs-lookup"><span data-stu-id="92e22-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="92e22-122">Description</span><span class="sxs-lookup"><span data-stu-id="92e22-122">Description</span></span>

<span data-ttu-id="92e22-123">次の例は、 **Copyitem**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="92e22-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="92e22-124">新しいアイテムのアイテム識別子は、応答メッセージで返されます。</span><span class="sxs-lookup"><span data-stu-id="92e22-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="92e22-125">メールボックス間またはメールボックスからパブリックフォルダー **Copyitem**操作への応答では、アイテム識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="92e22-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="92e22-126">コード</span><span class="sxs-lookup"><span data-stu-id="92e22-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="92e22-127">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="92e22-127">Successful response elements</span></span>

<span data-ttu-id="92e22-128">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="92e22-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="92e22-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="92e22-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="92e22-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="92e22-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="92e22-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="92e22-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="92e22-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="92e22-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="92e22-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92e22-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92e22-134">Items</span><span class="sxs-lookup"><span data-stu-id="92e22-134">Items</span></span>](items.md)
    
<span data-ttu-id="92e22-135">**Copyitem**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92e22-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="92e22-136">[Copyitemresponse](copyitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="92e22-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="92e22-137">CopyItem エラー応答</span><span class="sxs-lookup"><span data-stu-id="92e22-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="92e22-138">Description</span><span class="sxs-lookup"><span data-stu-id="92e22-138">Description</span></span>

<span data-ttu-id="92e22-139">次の例は、 **Copyitem**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="92e22-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="92e22-140">コード</span><span class="sxs-lookup"><span data-stu-id="92e22-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="92e22-141">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="92e22-141">Error response elements</span></span>

<span data-ttu-id="92e22-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="92e22-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="92e22-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="92e22-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="92e22-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="92e22-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="92e22-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="92e22-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="92e22-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="92e22-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="92e22-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="92e22-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="92e22-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92e22-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92e22-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="92e22-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="92e22-150">Items</span><span class="sxs-lookup"><span data-stu-id="92e22-150">Items</span></span>](items.md)
    
<span data-ttu-id="92e22-151">**Copyitem**操作のエラー応答メッセージに関するその他のオプションについては、「スキーマ階層」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92e22-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="92e22-152">[Copyitemresponse](copyitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="92e22-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="92e22-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="92e22-153">See also</span></span>



- [<span data-ttu-id="92e22-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="92e22-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

