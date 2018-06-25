---
title: GetItem 操作 (連絡先)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: GetItem 操作を使用すると、Exchange ストアから連絡先アイテムを取得します。
ms.openlocfilehash: 8d7436421f0c54a49345e8ef6b37cb442bca4277
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760774"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="58209-103">GetItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="58209-103">GetItem operation (contact)</span></span>

<span data-ttu-id="58209-104">GetItem 操作を使用すると、Exchange ストアから連絡先アイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="58209-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="58209-105">GetItem (連絡先) の要求の例</span><span class="sxs-lookup"><span data-stu-id="58209-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="58209-106">説明</span><span class="sxs-lookup"><span data-stu-id="58209-106">Description</span></span>

<span data-ttu-id="58209-107">次の例では、Exchange ストアからアイテムを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="58209-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="58209-108">コード</span><span class="sxs-lookup"><span data-stu-id="58209-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="58209-109">コメント</span><span class="sxs-lookup"><span data-stu-id="58209-109">Comments</span></span>

<span data-ttu-id="58209-110">Exchange ストアから項目を取得する要求は、すべての項目の種類、同じ形式をとります。</span><span class="sxs-lookup"><span data-stu-id="58209-110">The request to get an item from the Exchange store takes the same form for all item types.</span></span> <span data-ttu-id="58209-111">さまざまなアイテムには、避難用図形を基にさまざまな情報が返されるので、さまざまなアイテムの要求に対する応答が変更されます。</span><span class="sxs-lookup"><span data-stu-id="58209-111">The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="58209-112">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="58209-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="58209-113">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="58209-113">Request elements</span></span>

<span data-ttu-id="58209-114">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="58209-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="58209-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="58209-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="58209-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="58209-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="58209-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="58209-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="58209-118">Itemid</span><span class="sxs-lookup"><span data-stu-id="58209-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="58209-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="58209-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="58209-120">GetItem (連絡先) を正常な応答</span><span class="sxs-lookup"><span data-stu-id="58209-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="58209-121">説明</span><span class="sxs-lookup"><span data-stu-id="58209-121">Description</span></span>

<span data-ttu-id="58209-122">次のコード例では、 **AllProperties**[BaseShape](baseshape.md)の正常な GetItem 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="58209-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="58209-123">コード</span><span class="sxs-lookup"><span data-stu-id="58209-123">Code</span></span>

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
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="58209-124">コメント</span><span class="sxs-lookup"><span data-stu-id="58209-124">Comments</span></span>

<span data-ttu-id="58209-125">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="58209-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="58209-126">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="58209-126">Successful response elements</span></span>

<span data-ttu-id="58209-127">次の要素は、連絡先アイテムの**AllProperties**の応答の形をした GetItem 要求に対して、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="58209-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="58209-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="58209-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="58209-129">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="58209-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="58209-130">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="58209-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="58209-131">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="58209-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="58209-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58209-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58209-133">Items</span><span class="sxs-lookup"><span data-stu-id="58209-133">Items</span></span>](items.md)
    
- [<span data-ttu-id="58209-134">Contact</span><span class="sxs-lookup"><span data-stu-id="58209-134">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="58209-135">ItemId</span><span class="sxs-lookup"><span data-stu-id="58209-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="58209-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="58209-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="58209-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="58209-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="58209-138">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="58209-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="58209-139">Body/本文</span><span class="sxs-lookup"><span data-stu-id="58209-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="58209-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="58209-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="58209-141">Size</span><span class="sxs-lookup"><span data-stu-id="58209-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="58209-142">Importance</span><span class="sxs-lookup"><span data-stu-id="58209-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="58209-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="58209-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="58209-144">IsDraft</span><span class="sxs-lookup"><span data-stu-id="58209-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="58209-145">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="58209-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="58209-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="58209-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="58209-147">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="58209-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="58209-148">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="58209-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="58209-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="58209-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="58209-150">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="58209-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="58209-151">カルチャ</span><span class="sxs-lookup"><span data-stu-id="58209-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="58209-152">表題</span><span class="sxs-lookup"><span data-stu-id="58209-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="58209-153">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="58209-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="58209-154">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="58209-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58209-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="58209-155">GivenName</span></span>](givenname.md)
    
- <span data-ttu-id="58209-156">[[頭文字]](initials.md)</span><span class="sxs-lookup"><span data-stu-id="58209-156">[Initials](initials.md)</span></span>
    
- [<span data-ttu-id="58209-157">CompleteName</span><span class="sxs-lookup"><span data-stu-id="58209-157">CompleteName</span></span>](completename.md)
    
- <span data-ttu-id="58209-158">[[部署名]](firstname.md)</span><span class="sxs-lookup"><span data-stu-id="58209-158">[FirstName](firstname.md)</span></span>
    
- <span data-ttu-id="58209-159">[[氏名]](lastname.md)</span><span class="sxs-lookup"><span data-stu-id="58209-159">[LastName](lastname.md)</span></span>
    
- [<span data-ttu-id="58209-160">FullName</span><span class="sxs-lookup"><span data-stu-id="58209-160">FullName</span></span>](fullname.md)
    
- <span data-ttu-id="58209-161">[[得意先名]](companyname.md)</span><span class="sxs-lookup"><span data-stu-id="58209-161">[CompanyName](companyname.md)</span></span>
    
- [<span data-ttu-id="58209-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="58209-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="58209-163">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="58209-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="58209-164">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="58209-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="58209-165">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="58209-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="58209-166">番地</span><span class="sxs-lookup"><span data-stu-id="58209-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="58209-167">City</span><span class="sxs-lookup"><span data-stu-id="58209-167">City</span></span>](city.md)
    
- [<span data-ttu-id="58209-168">State</span><span class="sxs-lookup"><span data-stu-id="58209-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="58209-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="58209-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="58209-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="58209-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="58209-171">入力 (電話番号)</span><span class="sxs-lookup"><span data-stu-id="58209-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="58209-172">役職</span><span class="sxs-lookup"><span data-stu-id="58209-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="58209-173">姓</span><span class="sxs-lookup"><span data-stu-id="58209-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="58209-174">GetItem (連絡先) 要求の無効な使用例</span><span class="sxs-lookup"><span data-stu-id="58209-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="58209-175">説明</span><span class="sxs-lookup"><span data-stu-id="58209-175">Description</span></span>

<span data-ttu-id="58209-176">次のコード例は、無効な要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="58209-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="58209-177">コード</span><span class="sxs-lookup"><span data-stu-id="58209-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="58209-178">コメント</span><span class="sxs-lookup"><span data-stu-id="58209-178">Comments</span></span>

<span data-ttu-id="58209-179">アイテム識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="58209-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="58209-180">GetItem (連絡先) のエラー応答</span><span class="sxs-lookup"><span data-stu-id="58209-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="58209-181">説明</span><span class="sxs-lookup"><span data-stu-id="58209-181">Description</span></span>

<span data-ttu-id="58209-182">GetItem (連絡先) の要求にエラー応答をコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58209-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="58209-183">コード</span><span class="sxs-lookup"><span data-stu-id="58209-183">Code</span></span>

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
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="58209-184">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="58209-184">Error response elements</span></span>

<span data-ttu-id="58209-185">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="58209-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="58209-186">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="58209-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="58209-187">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="58209-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="58209-188">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="58209-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="58209-189">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="58209-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="58209-190">MessageText</span><span class="sxs-lookup"><span data-stu-id="58209-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="58209-191">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58209-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58209-192">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="58209-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="58209-193">Items</span><span class="sxs-lookup"><span data-stu-id="58209-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="58209-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="58209-194">See also</span></span>



<span data-ttu-id="58209-195">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="58209-195">[GetItem operation](getitem-operation.md)</span></span>


- [<span data-ttu-id="58209-196">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="58209-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

