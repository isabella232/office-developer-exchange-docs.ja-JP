---
title: CreateItem 操作 (連絡先)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: CreateItem 操作は、Exchange ストアで連絡先を作成するために使用されます。
ms.openlocfilehash: e1d78392b94d328cf687655cd93e6c9568f6274f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457124"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="42ce6-103">CreateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="42ce6-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="42ce6-104">CreateItem 操作は、Exchange ストアで連絡先を作成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="42ce6-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42ce6-105">注釈</span><span class="sxs-lookup"><span data-stu-id="42ce6-105">Remarks</span></span>

<span data-ttu-id="42ce6-106">プライベート配布リストの作成はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42ce6-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="42ce6-107">[CompleteName](completename.md)コンテナー内のすべてのプロパティは読み取り専用であり、連絡先アイテムには設定できません。</span><span class="sxs-lookup"><span data-stu-id="42ce6-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="42ce6-108">CreateItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="42ce6-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="42ce6-109">Description</span><span class="sxs-lookup"><span data-stu-id="42ce6-109">Description</span></span>

<span data-ttu-id="42ce6-110">次の有効な CreateItem SOAP 要求の例は、既定の連絡先フォルダーに連絡先を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="42ce6-111">コード</span><span class="sxs-lookup"><span data-stu-id="42ce6-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="42ce6-112">Request 要素</span><span class="sxs-lookup"><span data-stu-id="42ce6-112">Request elements</span></span>

<span data-ttu-id="42ce6-113">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="42ce6-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="42ce6-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="42ce6-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="42ce6-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="42ce6-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="42ce6-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="42ce6-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="42ce6-117">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="42ce6-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="42ce6-118">Contact</span><span class="sxs-lookup"><span data-stu-id="42ce6-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="42ce6-119">FileAs</span><span class="sxs-lookup"><span data-stu-id="42ce6-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="42ce6-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="42ce6-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="42ce6-121">CompanyName</span><span class="sxs-lookup"><span data-stu-id="42ce6-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="42ce6-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="42ce6-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="42ce6-123">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="42ce6-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="42ce6-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="42ce6-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="42ce6-125">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="42ce6-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="42ce6-126">所在</span><span class="sxs-lookup"><span data-stu-id="42ce6-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="42ce6-127">市区町村</span><span class="sxs-lookup"><span data-stu-id="42ce6-127">City</span></span>](city.md)
    
- [<span data-ttu-id="42ce6-128">State</span><span class="sxs-lookup"><span data-stu-id="42ce6-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="42ce6-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="42ce6-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="42ce6-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="42ce6-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="42ce6-131">Entry (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="42ce6-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="42ce6-132">JobTitle</span><span class="sxs-lookup"><span data-stu-id="42ce6-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="42ce6-133">姓</span><span class="sxs-lookup"><span data-stu-id="42ce6-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="42ce6-134">成功した CreateItem 要求</span><span class="sxs-lookup"><span data-stu-id="42ce6-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="42ce6-135">Description</span><span class="sxs-lookup"><span data-stu-id="42ce6-135">Description</span></span>

<span data-ttu-id="42ce6-136">次の例は、連絡先を作成した CreateItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="42ce6-137">この例では、応答に新しく作成されたアイテムの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="42ce6-138">コード</span><span class="sxs-lookup"><span data-stu-id="42ce6-138">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="42ce6-139">コメント</span><span class="sxs-lookup"><span data-stu-id="42ce6-139">Comments</span></span>

<span data-ttu-id="42ce6-140">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="42ce6-141">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="42ce6-141">Successful response elements</span></span>

<span data-ttu-id="42ce6-142">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="42ce6-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="42ce6-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="42ce6-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="42ce6-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="42ce6-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="42ce6-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="42ce6-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="42ce6-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="42ce6-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="42ce6-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="42ce6-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="42ce6-148">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="42ce6-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="42ce6-149">Contact</span><span class="sxs-lookup"><span data-stu-id="42ce6-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="42ce6-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="42ce6-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="42ce6-151">無効な CreateItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="42ce6-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="42ce6-152">Description</span><span class="sxs-lookup"><span data-stu-id="42ce6-152">Description</span></span>

<span data-ttu-id="42ce6-153">次の例は、有効な XML で互換性のない命令を含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="42ce6-154">検索フォルダーに連絡先を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="42ce6-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="42ce6-155">コード</span><span class="sxs-lookup"><span data-stu-id="42ce6-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a><span data-ttu-id="42ce6-156">CreateItem (Contact) エラー応答</span><span class="sxs-lookup"><span data-stu-id="42ce6-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="42ce6-157">Description</span><span class="sxs-lookup"><span data-stu-id="42ce6-157">Description</span></span>

<span data-ttu-id="42ce6-158">次の例は、CreateItem (Contact) 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="42ce6-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="42ce6-159">コード</span><span class="sxs-lookup"><span data-stu-id="42ce6-159">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="42ce6-160">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="42ce6-160">Error response elements</span></span>

<span data-ttu-id="42ce6-161">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="42ce6-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="42ce6-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="42ce6-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="42ce6-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="42ce6-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="42ce6-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="42ce6-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="42ce6-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="42ce6-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="42ce6-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="42ce6-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="42ce6-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="42ce6-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="42ce6-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="42ce6-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="42ce6-169">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="42ce6-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="42ce6-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="42ce6-170">See also</span></span>



[<span data-ttu-id="42ce6-171">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="42ce6-171">CreateItem operation</span></span>](createitem-operation.md)

