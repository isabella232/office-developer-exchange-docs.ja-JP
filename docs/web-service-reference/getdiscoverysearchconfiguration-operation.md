---
title: GetDiscoverySearchConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: GetDiscoverySearchConfiguration EWS 操作に関する情報を検索します。
ms.openlocfilehash: 4db435988a9954b921e7851986b6f92ffedbad94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461024"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="0837f-103">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="0837f-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="0837f-104">**Getdiscoverysearchconfiguration** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0837f-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="0837f-105">**Getdiscoverysearchconfiguration**操作は、インプレース保持、保存された探索検索、および探索検索が有効になっているメールボックスの構成情報を返します。</span><span class="sxs-lookup"><span data-stu-id="0837f-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="0837f-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0837f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="0837f-107">GetDiscoverySearchConfiguration 操作の使用</span><span class="sxs-lookup"><span data-stu-id="0837f-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="0837f-108">**Getdiscoverysearchconfiguration**操作は、探索検索の構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0837f-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="0837f-109">要求には、次の引数の1つ以上を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0837f-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="0837f-110">[Searchid](searchid.md) —保存された探索検索を識別します。</span><span class="sxs-lookup"><span data-stu-id="0837f-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="0837f-111">この引数が要求で送信される場合、他の引数の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="0837f-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="0837f-112">[Expandgroupmembership](expandgroupmembership.md) : グループメンバーシップが応答で展開されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="0837f-113">値が**true の場合**は、すべての検索可能なメールボックスが応答で返されるように、グループメンバーシップが展開されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="0837f-114">値が**false**の場合は、応答でグループのみが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="0837f-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) —インプレースホールド構成に加えて、すべての検索可能なメールボックスが返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="0837f-116">値が**true の場合**は、インプレースホールド構成のみが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="0837f-117">値が**false**の場合は、すべての検索可能なメールボックス識別子がインプレースホールド識別子に加えて返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="0837f-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="0837f-118">この要素が存在しない場合の既定の動作は、 **false**の値と同じです。</span><span class="sxs-lookup"><span data-stu-id="0837f-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="0837f-119">GetDiscoverySearchConfiguration 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0837f-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="0837f-120">**Getdiscoverysearchconfiguration**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0837f-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0837f-121">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="0837f-121">**Header name**</span></span>|<span data-ttu-id="0837f-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="0837f-122">**Element**</span></span>|<span data-ttu-id="0837f-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="0837f-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0837f-124">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="0837f-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="0837f-125">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="0837f-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="0837f-126">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="0837f-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="0837f-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0837f-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0837f-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0837f-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0837f-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0837f-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0837f-130">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0837f-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0837f-131">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0837f-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0837f-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0837f-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0837f-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0837f-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0837f-134">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0837f-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0837f-135">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0837f-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="0837f-136">GetDiscoverySearchConfiguration 操作要求の例: 保存された検索の探索検索構成を取得する</span><span class="sxs-lookup"><span data-stu-id="0837f-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="0837f-137">次の**Getdiscoverysearchconfiguration**操作要求の例は、"MyDiscSearchFor-sbrown" と呼ばれる保存済みの検索の構成を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0837f-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="0837f-138">[Expandgroupmembership](expandgroupmembership.md)要素と[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md)要素の引数は無視されます。</span><span class="sxs-lookup"><span data-stu-id="0837f-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="0837f-139">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0837f-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0837f-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0837f-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="0837f-141">SearchId</span><span class="sxs-lookup"><span data-stu-id="0837f-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="0837f-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="0837f-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="0837f-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="0837f-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="0837f-144">成功した GetDiscoverySearchConfiguration 操作応答: 1 つの保存済み検索の要求</span><span class="sxs-lookup"><span data-stu-id="0837f-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="0837f-145">次の例は、"MyDiscSearchFor-sbrown" と呼ばれる保存済みの検索の構成を取得するために、 **Getdiscoverysearchconfiguration**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0837f-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0837f-146">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0837f-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0837f-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0837f-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="0837f-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0837f-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0837f-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="0837f-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="0837f-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0837f-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="0837f-151">SearchId</span><span class="sxs-lookup"><span data-stu-id="0837f-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="0837f-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="0837f-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="0837f-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="0837f-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="0837f-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="0837f-155">Guid</span><span class="sxs-lookup"><span data-stu-id="0837f-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0837f-156">PrimarySmtpAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="0837f-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="0837f-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="0837f-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="0837f-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0837f-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="0837f-159">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="0837f-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="0837f-160">Isメンバーシップグループ</span><span class="sxs-lookup"><span data-stu-id="0837f-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="0837f-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="0837f-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="0837f-162">成功した GetDiscoverySearchConfiguration 操作応答: インプレース保持の要求</span><span class="sxs-lookup"><span data-stu-id="0837f-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="0837f-163">次の例は、インプレースホールドのみを取得する**Getdiscoverysearchconfiguration**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0837f-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0837f-164">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0837f-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0837f-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0837f-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="0837f-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0837f-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0837f-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="0837f-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="0837f-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0837f-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="0837f-169">SearchId</span><span class="sxs-lookup"><span data-stu-id="0837f-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="0837f-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="0837f-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="0837f-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="0837f-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="0837f-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="0837f-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="0837f-173">成功した GetDiscoverySearchConfiguration 操作応答: すべての保存された探索検索構成の要求</span><span class="sxs-lookup"><span data-stu-id="0837f-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="0837f-174">次の例は、保存されているすべての探索検索を取得するために、 **Getdiscoverysearchconfiguration**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0837f-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0837f-175">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0837f-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0837f-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0837f-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="0837f-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0837f-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0837f-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="0837f-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="0837f-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0837f-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="0837f-180">SearchId</span><span class="sxs-lookup"><span data-stu-id="0837f-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="0837f-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="0837f-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="0837f-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="0837f-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="0837f-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="0837f-184">Guid</span><span class="sxs-lookup"><span data-stu-id="0837f-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0837f-185">PrimarySmtpAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="0837f-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="0837f-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="0837f-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="0837f-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0837f-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="0837f-188">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="0837f-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="0837f-189">Isメンバーシップグループ</span><span class="sxs-lookup"><span data-stu-id="0837f-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="0837f-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="0837f-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="0837f-191">GetDiscoverySearchConfiguration 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="0837f-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="0837f-192">次の例は、 **Getdiscoverysearchconfiguration**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0837f-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="0837f-193">これは、サーバー上に存在しない保存済みの検索を取得する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="0837f-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0837f-194">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0837f-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0837f-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0837f-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="0837f-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="0837f-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0837f-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0837f-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0837f-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0837f-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0837f-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="0837f-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="0837f-200">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="0837f-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0837f-201">関連項目</span><span class="sxs-lookup"><span data-stu-id="0837f-201">See also</span></span>

- [<span data-ttu-id="0837f-202">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="0837f-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0837f-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="0837f-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="0837f-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="0837f-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0837f-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="0837f-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="0837f-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="0837f-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0837f-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

