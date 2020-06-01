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
description: GetItem 操作は、Exchange ストアから連絡先アイテムを取得するために使用されます。
ms.openlocfilehash: 93e8dbe28e130ab64d4b8d12d2befde1f77ae8fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460023"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="64d85-103">GetItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="64d85-103">GetItem operation (contact)</span></span>

<span data-ttu-id="64d85-104">GetItem 操作は、Exchange ストアから連絡先アイテムを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="64d85-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="64d85-105">GetItem (連絡先) 要求の例</span><span class="sxs-lookup"><span data-stu-id="64d85-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="64d85-106">説明</span><span class="sxs-lookup"><span data-stu-id="64d85-106">Description</span></span>

<span data-ttu-id="64d85-107">次の例は、Exchange ストアからアイテムを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="64d85-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="64d85-108">コード</span><span class="sxs-lookup"><span data-stu-id="64d85-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
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

### <a name="comments"></a><span data-ttu-id="64d85-109">コメント</span><span class="sxs-lookup"><span data-stu-id="64d85-109">Comments</span></span>

<span data-ttu-id="64d85-110">Exchange ストアからアイテムを取得する要求では、すべてのアイテムの種類に対して同じ形式が使用されます。</span><span class="sxs-lookup"><span data-stu-id="64d85-110">The request to get an item from the Exchange store takes the same form for all item types.</span></span> <span data-ttu-id="64d85-111">さまざまなアイテムが応答図形に基づいて異なる情報を返すため、さまざまなアイテムに対する要求に対する応答は異なります。</span><span class="sxs-lookup"><span data-stu-id="64d85-111">The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="64d85-112">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="64d85-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="64d85-113">Request 要素</span><span class="sxs-lookup"><span data-stu-id="64d85-113">Request elements</span></span>

<span data-ttu-id="64d85-114">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="64d85-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="64d85-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="64d85-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="64d85-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="64d85-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="64d85-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="64d85-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="64d85-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="64d85-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="64d85-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="64d85-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="64d85-120">成功した GetItem (連絡先) 応答</span><span class="sxs-lookup"><span data-stu-id="64d85-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="64d85-121">説明</span><span class="sxs-lookup"><span data-stu-id="64d85-121">Description</span></span>

<span data-ttu-id="64d85-122">次のコード例では、**すべての Allproperties**[baseshape](baseshape.md)に対して、成功した GetItem 応答を示します。</span><span class="sxs-lookup"><span data-stu-id="64d85-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="64d85-123">コード</span><span class="sxs-lookup"><span data-stu-id="64d85-123">Code</span></span>

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
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="64d85-124">コメント</span><span class="sxs-lookup"><span data-stu-id="64d85-124">Comments</span></span>

<span data-ttu-id="64d85-125">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="64d85-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="64d85-126">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="64d85-126">Successful response elements</span></span>

<span data-ttu-id="64d85-127">次の要素は、[連絡先] アイテムの**Allproperties**の応答図形を使用して、GetItem 要求の応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="64d85-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="64d85-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="64d85-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="64d85-129">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="64d85-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="64d85-130">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="64d85-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="64d85-131">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="64d85-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="64d85-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="64d85-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="64d85-133">Items</span><span class="sxs-lookup"><span data-stu-id="64d85-133">Items</span></span>](items.md)
    
- [<span data-ttu-id="64d85-134">連絡先</span><span class="sxs-lookup"><span data-stu-id="64d85-134">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="64d85-135">ItemId</span><span class="sxs-lookup"><span data-stu-id="64d85-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="64d85-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="64d85-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="64d85-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="64d85-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="64d85-138">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="64d85-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="64d85-139">Body</span><span class="sxs-lookup"><span data-stu-id="64d85-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="64d85-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="64d85-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- <span data-ttu-id="64d85-141">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="64d85-141">[Size](size.md)</span></span>
    
- [<span data-ttu-id="64d85-142">Importance</span><span class="sxs-lookup"><span data-stu-id="64d85-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="64d85-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="64d85-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="64d85-144">IsDraft</span><span class="sxs-lookup"><span data-stu-id="64d85-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="64d85-145">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="64d85-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="64d85-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="64d85-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="64d85-147">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="64d85-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="64d85-148">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="64d85-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="64d85-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="64d85-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="64d85-150">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="64d85-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="64d85-151">Culture</span><span class="sxs-lookup"><span data-stu-id="64d85-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="64d85-152">FileAs</span><span class="sxs-lookup"><span data-stu-id="64d85-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="64d85-153">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="64d85-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="64d85-154">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="64d85-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="64d85-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="64d85-155">GivenName</span></span>](givenname.md)
    
- <span data-ttu-id="64d85-156">[[頭文字](initials.md)]</span><span class="sxs-lookup"><span data-stu-id="64d85-156">[Initials](initials.md)</span></span>
    
- [<span data-ttu-id="64d85-157">CompleteName</span><span class="sxs-lookup"><span data-stu-id="64d85-157">CompleteName</span></span>](completename.md)
    
- [<span data-ttu-id="64d85-158">FirstName</span><span class="sxs-lookup"><span data-stu-id="64d85-158">FirstName</span></span>](firstname.md)
    
- [<span data-ttu-id="64d85-159">LastName</span><span class="sxs-lookup"><span data-stu-id="64d85-159">LastName</span></span>](lastname.md)
    
- [<span data-ttu-id="64d85-160">FullName</span><span class="sxs-lookup"><span data-stu-id="64d85-160">FullName</span></span>](fullname.md)
    
- [<span data-ttu-id="64d85-161">CompanyName</span><span class="sxs-lookup"><span data-stu-id="64d85-161">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="64d85-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="64d85-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="64d85-163">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="64d85-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="64d85-164">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="64d85-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="64d85-165">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="64d85-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="64d85-166">所在</span><span class="sxs-lookup"><span data-stu-id="64d85-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="64d85-167">市区町村</span><span class="sxs-lookup"><span data-stu-id="64d85-167">City</span></span>](city.md)
    
- [<span data-ttu-id="64d85-168">State</span><span class="sxs-lookup"><span data-stu-id="64d85-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="64d85-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="64d85-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="64d85-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="64d85-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="64d85-171">Entry (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="64d85-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="64d85-172">JobTitle</span><span class="sxs-lookup"><span data-stu-id="64d85-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="64d85-173">姓</span><span class="sxs-lookup"><span data-stu-id="64d85-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="64d85-174">無効な GetItem (Contact) 要求の例</span><span class="sxs-lookup"><span data-stu-id="64d85-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="64d85-175">説明</span><span class="sxs-lookup"><span data-stu-id="64d85-175">Description</span></span>

<span data-ttu-id="64d85-176">次のコード例は、無効な要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="64d85-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="64d85-177">コード</span><span class="sxs-lookup"><span data-stu-id="64d85-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
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

### <a name="comments"></a><span data-ttu-id="64d85-178">コメント</span><span class="sxs-lookup"><span data-stu-id="64d85-178">Comments</span></span>

<span data-ttu-id="64d85-179">読みやすくするために、アイテム識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="64d85-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="64d85-180">GetItem (連絡先) エラー応答</span><span class="sxs-lookup"><span data-stu-id="64d85-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="64d85-181">説明</span><span class="sxs-lookup"><span data-stu-id="64d85-181">Description</span></span>

<span data-ttu-id="64d85-182">次のコード例は、GetItem (連絡先) 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="64d85-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="64d85-183">コード</span><span class="sxs-lookup"><span data-stu-id="64d85-183">Code</span></span>

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
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="64d85-184">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="64d85-184">Error response elements</span></span>

<span data-ttu-id="64d85-185">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="64d85-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="64d85-186">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="64d85-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="64d85-187">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="64d85-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="64d85-188">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="64d85-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="64d85-189">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="64d85-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="64d85-190">MessageText</span><span class="sxs-lookup"><span data-stu-id="64d85-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="64d85-191">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="64d85-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="64d85-192">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="64d85-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="64d85-193">Items</span><span class="sxs-lookup"><span data-stu-id="64d85-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="64d85-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="64d85-194">See also</span></span>



<span data-ttu-id="64d85-195">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="64d85-195">[GetItem operation](getitem-operation.md)</span></span>


- [<span data-ttu-id="64d85-196">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="64d85-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

