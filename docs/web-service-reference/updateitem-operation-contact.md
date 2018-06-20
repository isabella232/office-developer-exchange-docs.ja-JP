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
description: UpdateItem 操作を使用して、Exchange ストア内の連絡先アイテムのプロパティを更新します。
ms.openlocfilehash: f2a501ce8e69068cd30b58011adf4defc68ce365
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839860"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="fae75-103">UpdateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="fae75-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="fae75-104">UpdateItem 操作を使用して、Exchange ストア内の連絡先アイテムのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fae75-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="fae75-105">UpdateItem (連絡先) の要求の例</span><span class="sxs-lookup"><span data-stu-id="fae75-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="fae75-106">説明</span><span class="sxs-lookup"><span data-stu-id="fae75-106">Description</span></span>

<span data-ttu-id="fae75-107">次のコード例は、連絡先の電子メール アドレスを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fae75-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="fae75-108">コード</span><span class="sxs-lookup"><span data-stu-id="fae75-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
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

### <a name="comments"></a><span data-ttu-id="fae75-109">コメント</span><span class="sxs-lookup"><span data-stu-id="fae75-109">Comments</span></span>

<span data-ttu-id="fae75-110">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="fae75-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="fae75-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="fae75-111">Request elements</span></span>

<span data-ttu-id="fae75-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="fae75-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fae75-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="fae75-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="fae75-114">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="fae75-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="fae75-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="fae75-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="fae75-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="fae75-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="fae75-117">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="fae75-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="fae75-118">SetItemField</span><span class="sxs-lookup"><span data-stu-id="fae75-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="fae75-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fae75-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="fae75-120">Contact</span><span class="sxs-lookup"><span data-stu-id="fae75-120">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="fae75-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fae75-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="fae75-122">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="fae75-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="fae75-123">UpdateItem (連絡先) を正常な応答</span><span class="sxs-lookup"><span data-stu-id="fae75-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="fae75-124">説明</span><span class="sxs-lookup"><span data-stu-id="fae75-124">Description</span></span>

<span data-ttu-id="fae75-125">UpdateItem 正常な応答を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="fae75-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="fae75-126">コード</span><span class="sxs-lookup"><span data-stu-id="fae75-126">Code</span></span>

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
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="fae75-127">コメント</span><span class="sxs-lookup"><span data-stu-id="fae75-127">Comments</span></span>

<span data-ttu-id="fae75-128">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="fae75-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="fae75-129">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="fae75-129">Successful response elements</span></span>

<span data-ttu-id="fae75-130">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="fae75-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fae75-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fae75-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fae75-132">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="fae75-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="fae75-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fae75-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fae75-134">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fae75-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="fae75-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fae75-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fae75-136">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="fae75-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="fae75-137">Contact</span><span class="sxs-lookup"><span data-stu-id="fae75-137">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="fae75-138">ItemId</span><span class="sxs-lookup"><span data-stu-id="fae75-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="fae75-139">UpdateItem (連絡先) 要求の無効な使用例</span><span class="sxs-lookup"><span data-stu-id="fae75-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="fae75-140">説明</span><span class="sxs-lookup"><span data-stu-id="fae75-140">Description</span></span>

<span data-ttu-id="fae75-141">次のコード例は、無効な要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="fae75-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fae75-142">コード</span><span class="sxs-lookup"><span data-stu-id="fae75-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
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

### <a name="comments"></a><span data-ttu-id="fae75-143">コメント</span><span class="sxs-lookup"><span data-stu-id="fae75-143">Comments</span></span>

<span data-ttu-id="fae75-144">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="fae75-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="fae75-145">UpdateItem (連絡先) のエラー応答</span><span class="sxs-lookup"><span data-stu-id="fae75-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="fae75-146">説明</span><span class="sxs-lookup"><span data-stu-id="fae75-146">Description</span></span>

<span data-ttu-id="fae75-147">UpdateItem (連絡先) 要求に対するエラー応答をコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fae75-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fae75-148">コード</span><span class="sxs-lookup"><span data-stu-id="fae75-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'http://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fae75-149">コメント</span><span class="sxs-lookup"><span data-stu-id="fae75-149">Comments</span></span>

<span data-ttu-id="fae75-150">スキーマ検証エラーが原因で発生するエラー応答の SOAP 本文で使用されているいくつかの要素は、メッセージまたは型のスキーマで定義されていません。</span><span class="sxs-lookup"><span data-stu-id="fae75-150">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas.</span></span> <span data-ttu-id="fae75-151">**詳細**要素には、エラーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fae75-151">The **detail** element contains information about the error.</span></span> <span data-ttu-id="fae75-152">[ResponseCode](responsecode.md)要素には、エラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fae75-152">The [ResponseCode](responsecode.md) element contains the error code.</span></span> <span data-ttu-id="fae75-153">[メッセージ](message-ex15websvcsotherref.md)要素には、1 つが使用可能な場合、エラーの説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fae75-153">The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available.</span></span> <span data-ttu-id="fae75-154">**直線**要素は、スキーマ検証エラーが発生した行番号について説明します。</span><span class="sxs-lookup"><span data-stu-id="fae75-154">The **Line** element describes the line number where the schema validation error occurred.</span></span> <span data-ttu-id="fae75-155">**位置**の要素は、XML ドキュメントの左端の文字の位置について説明します。</span><span class="sxs-lookup"><span data-stu-id="fae75-155">The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fae75-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="fae75-156">See also</span></span>



<span data-ttu-id="fae75-157">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="fae75-157">[UpdateItem operation](updateitem-operation.md)</span></span>

