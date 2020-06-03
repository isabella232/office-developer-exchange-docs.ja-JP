---
title: SendItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: SendItem 操作は、Exchange ストアにある電子メールメッセージを送信するために使用されます。
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530339"
---
# <a name="senditem-operation"></a><span data-ttu-id="e68c6-103">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="e68c6-103">SendItem operation</span></span>

<span data-ttu-id="e68c6-104">SendItem 操作は、Exchange ストアにある電子メールメッセージを送信するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e68c6-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="e68c6-105">SendItem (電子メールメッセージ) の要求の例</span><span class="sxs-lookup"><span data-stu-id="e68c6-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="e68c6-106">Description</span><span class="sxs-lookup"><span data-stu-id="e68c6-106">Description</span></span>

<span data-ttu-id="e68c6-107">次の例は、電子メールメッセージを送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e68c6-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="e68c6-108">コード</span><span class="sxs-lookup"><span data-stu-id="e68c6-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e68c6-109">コメント</span><span class="sxs-lookup"><span data-stu-id="e68c6-109">Comments</span></span>

<span data-ttu-id="e68c6-110">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e68c6-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="e68c6-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="e68c6-111">Request elements</span></span>

<span data-ttu-id="e68c6-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e68c6-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e68c6-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="e68c6-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="e68c6-114">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e68c6-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="e68c6-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="e68c6-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="e68c6-116">Successful SendItem (電子メールメッセージ) 応答</span><span class="sxs-lookup"><span data-stu-id="e68c6-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="e68c6-117">Description</span><span class="sxs-lookup"><span data-stu-id="e68c6-117">Description</span></span>

<span data-ttu-id="e68c6-118">次の例は、成功した SendItem 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e68c6-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="e68c6-119">コード</span><span class="sxs-lookup"><span data-stu-id="e68c6-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="e68c6-120">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="e68c6-120">Successful response elements</span></span>

<span data-ttu-id="e68c6-121">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e68c6-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e68c6-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e68c6-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e68c6-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="e68c6-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="e68c6-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e68c6-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e68c6-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e68c6-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="e68c6-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e68c6-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="e68c6-127">コメント</span><span class="sxs-lookup"><span data-stu-id="e68c6-127">Comments</span></span>

<span data-ttu-id="e68c6-128">[送信済みアイテム] 識別フォルダーにコピーを保存するために SendAndSaveCopy オプションが設定されているプリンシパルの [下書き] フォルダーにある電子メールメッセージを送信しようとする代理人は、送信済みアイテムのコピーを送信済みアイテムの識別フォルダーに移動することを黙って失敗します。</span><span class="sxs-lookup"><span data-stu-id="e68c6-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="e68c6-129">アイテムはプリンシパルの [下書き] フォルダーに残ります。</span><span class="sxs-lookup"><span data-stu-id="e68c6-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="e68c6-130">この問題の回避策は、プリンシパルのメールボックスを[DistinguishedFolderId](distinguishedfolderid.md)要素で指定することです。</span><span class="sxs-lookup"><span data-stu-id="e68c6-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="e68c6-131">代理人が電子メールメッセージを作成して、代理人のメールボックスの [下書き] フォルダーに保存する場合に考慮すべきもう1つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="e68c6-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="e68c6-132">代理人がアイテムを送信し、プリンシパルの送信済みアイテムの識別フォルダーにコピーを保存しようとすると、メッセージは正常に送信され、下書きメッセージは代理人の下書きフォルダーに残り、送信されたメッセージは代理人またはプリンシパルの [送信済みアイテム] フォルダーに表示されず、応答は成功します。</span><span class="sxs-lookup"><span data-stu-id="e68c6-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="e68c6-133">無効な SendItem (電子メールメッセージ) 要求の例</span><span class="sxs-lookup"><span data-stu-id="e68c6-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="e68c6-134">Description</span><span class="sxs-lookup"><span data-stu-id="e68c6-134">Description</span></span>

<span data-ttu-id="e68c6-135">次のコードサンプルは、無効な識別子を持つ要求の例を示しています。</span><span class="sxs-lookup"><span data-stu-id="e68c6-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="e68c6-136">コード</span><span class="sxs-lookup"><span data-stu-id="e68c6-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="e68c6-137">SendItem (電子メールメッセージ) エラー応答</span><span class="sxs-lookup"><span data-stu-id="e68c6-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="e68c6-138">Description</span><span class="sxs-lookup"><span data-stu-id="e68c6-138">Description</span></span>

<span data-ttu-id="e68c6-139">次の例は、無効な識別子を含む SendItem 要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e68c6-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="e68c6-140">コード</span><span class="sxs-lookup"><span data-stu-id="e68c6-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="e68c6-141">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="e68c6-141">Error response elements</span></span>

<span data-ttu-id="e68c6-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e68c6-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e68c6-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e68c6-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e68c6-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="e68c6-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="e68c6-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e68c6-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e68c6-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e68c6-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="e68c6-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="e68c6-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e68c6-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e68c6-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e68c6-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e68c6-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="e68c6-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="e68c6-150">See also</span></span>



[<span data-ttu-id="e68c6-151">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="e68c6-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="e68c6-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="e68c6-152">**SendItemType**</span></span>


- [<span data-ttu-id="e68c6-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e68c6-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

