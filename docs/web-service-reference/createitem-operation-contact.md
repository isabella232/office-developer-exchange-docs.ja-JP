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
description: CreateItem 操作を使用して、Exchange ストア内の連絡先を作成します。
ms.openlocfilehash: 05e4715f3c6675401ae7afac852395f7459c02c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759834"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="2ef35-103">CreateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="2ef35-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="2ef35-104">CreateItem 操作を使用して、Exchange ストア内の連絡先を作成します。</span><span class="sxs-lookup"><span data-stu-id="2ef35-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ef35-105">備考</span><span class="sxs-lookup"><span data-stu-id="2ef35-105">Remarks</span></span>

<span data-ttu-id="2ef35-106">個人用配布リストの作成はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ef35-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="2ef35-107">[CompleteName](completename.md)コンテナー内のすべてのプロパティは読み取り専用であり、連絡先アイテムに設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="2ef35-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="2ef35-108">CreateItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="2ef35-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="2ef35-109">説明</span><span class="sxs-lookup"><span data-stu-id="2ef35-109">Description</span></span>

<span data-ttu-id="2ef35-110">有効な createitem メソッドの SOAP 要求の次の例では、既定の連絡先フォルダーに連絡先を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="2ef35-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="2ef35-111">コード</span><span class="sxs-lookup"><span data-stu-id="2ef35-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" >
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

### <a name="request-elements"></a><span data-ttu-id="2ef35-112">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="2ef35-112">Request elements</span></span>

<span data-ttu-id="2ef35-113">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2ef35-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2ef35-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="2ef35-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="2ef35-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="2ef35-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="2ef35-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="2ef35-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="2ef35-117">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="2ef35-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="2ef35-118">Contact</span><span class="sxs-lookup"><span data-stu-id="2ef35-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="2ef35-119">表題</span><span class="sxs-lookup"><span data-stu-id="2ef35-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="2ef35-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="2ef35-120">GivenName</span></span>](givenname.md)
    
- <span data-ttu-id="2ef35-121">[[得意先名]](companyname.md)</span><span class="sxs-lookup"><span data-stu-id="2ef35-121">[CompanyName](companyname.md)</span></span>
    
- [<span data-ttu-id="2ef35-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="2ef35-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="2ef35-123">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2ef35-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="2ef35-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="2ef35-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="2ef35-125">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="2ef35-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="2ef35-126">番地</span><span class="sxs-lookup"><span data-stu-id="2ef35-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="2ef35-127">City</span><span class="sxs-lookup"><span data-stu-id="2ef35-127">City</span></span>](city.md)
    
- [<span data-ttu-id="2ef35-128">State</span><span class="sxs-lookup"><span data-stu-id="2ef35-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="2ef35-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2ef35-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="2ef35-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="2ef35-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="2ef35-131">入力 (電話番号)</span><span class="sxs-lookup"><span data-stu-id="2ef35-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="2ef35-132">役職</span><span class="sxs-lookup"><span data-stu-id="2ef35-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="2ef35-133">姓</span><span class="sxs-lookup"><span data-stu-id="2ef35-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="2ef35-134">Createitem メソッドの要求が成功しました。</span><span class="sxs-lookup"><span data-stu-id="2ef35-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="2ef35-135">説明</span><span class="sxs-lookup"><span data-stu-id="2ef35-135">Description</span></span>

<span data-ttu-id="2ef35-136">次の例では、連絡先が作成されている CreateItem 要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="2ef35-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="2ef35-137">この例では、応答には、新しく作成されたアイテムの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ef35-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="2ef35-138">コード</span><span class="sxs-lookup"><span data-stu-id="2ef35-138">Code</span></span>

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="2ef35-139">コメント</span><span class="sxs-lookup"><span data-stu-id="2ef35-139">Comments</span></span>

<span data-ttu-id="2ef35-140">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="2ef35-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="2ef35-141">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="2ef35-141">Successful response elements</span></span>

<span data-ttu-id="2ef35-142">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2ef35-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2ef35-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2ef35-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2ef35-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="2ef35-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="2ef35-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2ef35-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2ef35-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2ef35-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="2ef35-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2ef35-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2ef35-148">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="2ef35-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="2ef35-149">Contact</span><span class="sxs-lookup"><span data-stu-id="2ef35-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="2ef35-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="2ef35-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="2ef35-151">CreateItem 要求の無効な使用例</span><span class="sxs-lookup"><span data-stu-id="2ef35-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="2ef35-152">説明</span><span class="sxs-lookup"><span data-stu-id="2ef35-152">Description</span></span>

<span data-ttu-id="2ef35-153">次の使用例は、互換性のない方法ですが、有効な XML が含まれている要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="2ef35-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="2ef35-154">検索フォルダーで連絡先を作成できません。</span><span class="sxs-lookup"><span data-stu-id="2ef35-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="2ef35-155">コード</span><span class="sxs-lookup"><span data-stu-id="2ef35-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
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

## <a name="createitem-contact-error-response"></a><span data-ttu-id="2ef35-156">Createitem メソッド (連絡先) のエラー応答</span><span class="sxs-lookup"><span data-stu-id="2ef35-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="2ef35-157">説明</span><span class="sxs-lookup"><span data-stu-id="2ef35-157">Description</span></span>

<span data-ttu-id="2ef35-158">次の使用例は、createitem メソッド (連絡先) の要求にエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2ef35-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="2ef35-159">コード</span><span class="sxs-lookup"><span data-stu-id="2ef35-159">Code</span></span>

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="2ef35-160">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="2ef35-160">Error response elements</span></span>

<span data-ttu-id="2ef35-161">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2ef35-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2ef35-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2ef35-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2ef35-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="2ef35-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="2ef35-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2ef35-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2ef35-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2ef35-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="2ef35-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="2ef35-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2ef35-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2ef35-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2ef35-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2ef35-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="2ef35-169">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="2ef35-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="2ef35-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ef35-170">See also</span></span>



<span data-ttu-id="2ef35-171">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="2ef35-171">[CreateItem operation](createitem-operation.md)</span></span>

