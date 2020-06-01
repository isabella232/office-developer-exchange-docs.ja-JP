---
title: UpdateItem 操作 (連絡先)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 298fdd71-a83d-4407-9728-4f0a8e2d857c
description: UpdateItem 操作は、Exchange ストア内の連絡先アイテムのプロパティを更新するために使用されます。
ms.openlocfilehash: 66e1b91ea3154d8a501339aed7b398970e8f5392
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459827"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="5a0e0-103">UpdateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="5a0e0-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="5a0e0-104">UpdateItem 操作は、Exchange ストア内の連絡先アイテムのプロパティを更新するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="5a0e0-105">UpdateItem (Contact) 要求の例</span><span class="sxs-lookup"><span data-stu-id="5a0e0-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5a0e0-106">説明</span><span class="sxs-lookup"><span data-stu-id="5a0e0-106">Description</span></span>

<span data-ttu-id="5a0e0-107">次のコード例は、連絡先の電子メールアドレスを更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a0e0-108">コード</span><span class="sxs-lookup"><span data-stu-id="5a0e0-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAA=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress1"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">changedemail@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5a0e0-109">コメント</span><span class="sxs-lookup"><span data-stu-id="5a0e0-109">Comments</span></span>

<span data-ttu-id="5a0e0-110">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5a0e0-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="5a0e0-111">Request elements</span></span>

<span data-ttu-id="5a0e0-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5a0e0-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5a0e0-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="5a0e0-114">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="5a0e0-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="5a0e0-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="5a0e0-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="5a0e0-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="5a0e0-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5a0e0-117">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="5a0e0-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="5a0e0-118">SetItemField</span><span class="sxs-lookup"><span data-stu-id="5a0e0-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="5a0e0-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5a0e0-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="5a0e0-120">連絡先</span><span class="sxs-lookup"><span data-stu-id="5a0e0-120">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="5a0e0-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5a0e0-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="5a0e0-122">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5a0e0-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="5a0e0-123">成功した UpdateItem (連絡先) 応答</span><span class="sxs-lookup"><span data-stu-id="5a0e0-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="5a0e0-124">説明</span><span class="sxs-lookup"><span data-stu-id="5a0e0-124">Description</span></span>

<span data-ttu-id="5a0e0-125">次のコード例は、正常な UpdateItem 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a0e0-126">コード</span><span class="sxs-lookup"><span data-stu-id="5a0e0-126">Code</span></span>

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
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABYx" />
            </t:Contact>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5a0e0-127">コメント</span><span class="sxs-lookup"><span data-stu-id="5a0e0-127">Comments</span></span>

<span data-ttu-id="5a0e0-128">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="5a0e0-129">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="5a0e0-129">Successful response elements</span></span>

<span data-ttu-id="5a0e0-130">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5a0e0-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5a0e0-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5a0e0-132">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="5a0e0-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="5a0e0-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a0e0-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a0e0-134">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5a0e0-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="5a0e0-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a0e0-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5a0e0-136">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="5a0e0-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="5a0e0-137">連絡先</span><span class="sxs-lookup"><span data-stu-id="5a0e0-137">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="5a0e0-138">ItemId</span><span class="sxs-lookup"><span data-stu-id="5a0e0-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="5a0e0-139">無効な UpdateItem (連絡先) 要求の例</span><span class="sxs-lookup"><span data-stu-id="5a0e0-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5a0e0-140">説明</span><span class="sxs-lookup"><span data-stu-id="5a0e0-140">Description</span></span>

<span data-ttu-id="5a0e0-141">次のコード例は、無効な要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a0e0-142">コード</span><span class="sxs-lookup"><span data-stu-id="5a0e0-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress4"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress4">changedemail2@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5a0e0-143">コメント</span><span class="sxs-lookup"><span data-stu-id="5a0e0-143">Comments</span></span>

<span data-ttu-id="5a0e0-144">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="5a0e0-145">UpdateItem (Contact) エラー応答</span><span class="sxs-lookup"><span data-stu-id="5a0e0-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="5a0e0-146">説明</span><span class="sxs-lookup"><span data-stu-id="5a0e0-146">Description</span></span>

<span data-ttu-id="5a0e0-147">次のコード例は、UpdateItem (連絡先) 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a0e0-148">コード</span><span class="sxs-lookup"><span data-stu-id="5a0e0-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'https://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5a0e0-149">コメント</span><span class="sxs-lookup"><span data-stu-id="5a0e0-149">Comments</span></span>

<span data-ttu-id="5a0e0-150">スキーマ検証エラーによって発生したエラー応答の SOAP 本文で使用されている一部の要素は、メッセージまたは種類のスキーマで定義されていません。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-150">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas.</span></span> <span data-ttu-id="5a0e0-151">**Detail**要素には、エラーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-151">The **detail** element contains information about the error.</span></span> <span data-ttu-id="5a0e0-152">応答[secの](responsecode.md)要素にエラーコードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-152">The [ResponseCode](responsecode.md) element contains the error code.</span></span> <span data-ttu-id="5a0e0-153">[メッセージ](message-ex15websvcsotherref.md)要素には、エラーの説明が含まれています (使用可能な場合)。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-153">The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available.</span></span> <span data-ttu-id="5a0e0-154">**Line**要素は、スキーマ検証エラーが発生した行番号を示します。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-154">The **Line** element describes the line number where the schema validation error occurred.</span></span> <span data-ttu-id="5a0e0-155">**Position**要素は、XML ドキュメントの左端の文字からの位置を表します。</span><span class="sxs-lookup"><span data-stu-id="5a0e0-155">The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5a0e0-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a0e0-156">See also</span></span>



<span data-ttu-id="5a0e0-157">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5a0e0-157">[UpdateItem operation](updateitem-operation.md)</span></span>

