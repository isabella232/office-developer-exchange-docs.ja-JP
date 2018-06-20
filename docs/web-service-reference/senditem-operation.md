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
description: SendItem 操作を使用して配置されている電子メール メッセージを送信する Exchange ストアにします。
ms.openlocfilehash: 780778b1599d0d5e5f4b6e5b58b67773bbe18cda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833336"
---
# <a name="senditem-operation"></a><span data-ttu-id="05248-103">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="05248-103">SendItem operation</span></span>

<span data-ttu-id="05248-104">SendItem 操作を使用して配置されている電子メール メッセージを送信する Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="05248-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="05248-105">SendItem (電子メール メッセージ) の要求の例</span><span class="sxs-lookup"><span data-stu-id="05248-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="05248-106">説明</span><span class="sxs-lookup"><span data-stu-id="05248-106">Description</span></span>

<span data-ttu-id="05248-107">次の例では、電子メール メッセージを送信する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="05248-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="05248-108">コード</span><span class="sxs-lookup"><span data-stu-id="05248-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="05248-109">コメント</span><span class="sxs-lookup"><span data-stu-id="05248-109">Comments</span></span>

<span data-ttu-id="05248-110">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="05248-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="05248-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="05248-111">Request elements</span></span>

<span data-ttu-id="05248-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="05248-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="05248-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="05248-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="05248-114">Itemid</span><span class="sxs-lookup"><span data-stu-id="05248-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="05248-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="05248-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="05248-116">SendItem (電子メール メッセージ) の正常な応答</span><span class="sxs-lookup"><span data-stu-id="05248-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="05248-117">説明</span><span class="sxs-lookup"><span data-stu-id="05248-117">Description</span></span>

<span data-ttu-id="05248-118">SendItem の正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="05248-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="05248-119">コード</span><span class="sxs-lookup"><span data-stu-id="05248-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="05248-120">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="05248-120">Successful response elements</span></span>

<span data-ttu-id="05248-121">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="05248-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="05248-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="05248-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="05248-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="05248-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="05248-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="05248-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="05248-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="05248-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="05248-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="05248-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="05248-127">コメント</span><span class="sxs-lookup"><span data-stu-id="05248-127">Comments</span></span>

<span data-ttu-id="05248-128">代理人設定識別フォルダー送信済みアイテムを識別する送信済みアイテムのコピーを移動するのには失敗、送信済みアイテムのコピーを保存する SendAndSaveCopy オプションを使用してプリンシパルの [下書き] フォルダーにある電子メール メッセージを送信しようとしています。フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="05248-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="05248-129">アイテムは、プリンシパルの [下書き] フォルダーに残ります。</span><span class="sxs-lookup"><span data-stu-id="05248-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="05248-130">この問題を回避する方法では、 [DistinguishedFolderId](distinguishedfolderid.md)要素内のプリンシパルのメールボックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="05248-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="05248-131">考慮すべきその他のシナリオは、代理人が電子メール メッセージを作成し、代理人のメールボックスの [下書き] フォルダーに保存するときです。</span><span class="sxs-lookup"><span data-stu-id="05248-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="05248-132">デリゲートは、アイテムを送信し、プリンシパルの送信済みアイテムの識別フォルダーにコピーを保存しようとすると、メッセージは正常に送信、代理人の [下書き] フォルダーに下書きメッセージは送信済みのメッセージがない、上司またはプリンシパルアイテム] フォルダーに送信し、応答は、成功します。</span><span class="sxs-lookup"><span data-stu-id="05248-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="05248-133">SendItem (電子メール メッセージ) 要求の無効な使用例</span><span class="sxs-lookup"><span data-stu-id="05248-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="05248-134">説明</span><span class="sxs-lookup"><span data-stu-id="05248-134">Description</span></span>

<span data-ttu-id="05248-135">次のコード サンプルでは、要求に無効な識別子の例を示します。</span><span class="sxs-lookup"><span data-stu-id="05248-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="05248-136">コード</span><span class="sxs-lookup"><span data-stu-id="05248-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="05248-137">SendItem (電子メール メッセージ) のエラー応答</span><span class="sxs-lookup"><span data-stu-id="05248-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="05248-138">説明</span><span class="sxs-lookup"><span data-stu-id="05248-138">Description</span></span>

<span data-ttu-id="05248-139">SendItem 要求に対して無効な識別子が含まれていますエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="05248-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="05248-140">コード</span><span class="sxs-lookup"><span data-stu-id="05248-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="05248-141">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="05248-141">Error response elements</span></span>

<span data-ttu-id="05248-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="05248-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="05248-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="05248-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="05248-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="05248-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="05248-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="05248-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="05248-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="05248-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="05248-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="05248-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="05248-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="05248-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="05248-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="05248-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="05248-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="05248-150">See also</span></span>



<span data-ttu-id="05248-151">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="05248-151">[SendItem operation](senditem-operation.md)</span></span>
  
 <span data-ttu-id="05248-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="05248-152">**SendItemType**</span></span>


- [<span data-ttu-id="05248-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="05248-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

