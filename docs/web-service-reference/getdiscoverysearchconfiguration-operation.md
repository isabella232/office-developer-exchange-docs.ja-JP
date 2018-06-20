---
title: GetDiscoverySearchConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: 操作 GetDiscoverySearchConfiguration EWS についての情報を検索します。
ms.openlocfilehash: a50463e575bf5a4ffdafc357d91563b0ca0486f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760689"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="fd5d1-103">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="fd5d1-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="fd5d1-104">**GetDiscoverySearchConfiguration** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="fd5d1-105">**GetDiscoverySearchConfiguration**操作では、インプレースの構成情報を保持している保存、検索、および検索が有効になっているメールボックスを返します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="fd5d1-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="fd5d1-107">GetDiscoverySearchConfiguration 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="fd5d1-108">**GetDiscoverySearchConfiguration**操作は、検索の構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="fd5d1-109">要求は、次の引数の 1 つ以上含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="fd5d1-110">[SearchId](searchid.md) : 保存された検索を識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="fd5d1-111">この引数を要求で送信する場合、他の引数の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="fd5d1-112">[ExpandGroupMembership](expandgroupmembership.md) -応答のグループのメンバーシップは展開するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="fd5d1-113">**True**の場合は、検索可能なすべてのメールボックスが応答で返されるように、グループ メンバーシップが展開されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="fd5d1-114">**False**の値は、グループのみが応答で返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="fd5d1-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) -埋め込み保留中の構成だけでなく、検索可能なすべてのメールボックスが返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="fd5d1-116">**True**の場合は、埋め込み先の保留中の構成のみが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="fd5d1-117">**False**の値は、埋め込み先の保留中の識別子だけでなく、検索可能なメールボックスのすべての識別子が返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="fd5d1-118">この要素が存在しない場合は、既定の動作は、値**false を指定**した場合と同じにします。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="fd5d1-119">GetDiscoverySearchConfiguration 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd5d1-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="fd5d1-120">**GetDiscoverySearchConfiguration**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="fd5d1-121">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-121">**Header name**</span></span>|<span data-ttu-id="fd5d1-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-122">**Element**</span></span>|<span data-ttu-id="fd5d1-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fd5d1-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="fd5d1-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="fd5d1-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="fd5d1-126">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="fd5d1-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fd5d1-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="fd5d1-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="fd5d1-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="fd5d1-130">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="fd5d1-131">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fd5d1-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="fd5d1-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="fd5d1-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fd5d1-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="fd5d1-134">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="fd5d1-135">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="fd5d1-136">GetDiscoverySearchConfiguration 操作の要求の例: 保存された検索の検索検索の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="fd5d1-137">**GetDiscoverySearchConfiguration**操作要求の次の使用例は、「MyDiscSearchFor sbrown」と呼ばれる、保存された検索の構成を要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="fd5d1-138">[ExpandGroupMembership](expandgroupmembership.md)と[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md)の要素の引数は無視されます。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="fd5d1-139">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd5d1-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd5d1-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="fd5d1-141">SearchId</span><span class="sxs-lookup"><span data-stu-id="fd5d1-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="fd5d1-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="fd5d1-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="fd5d1-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="fd5d1-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="fd5d1-144">GetDiscoverySearchConfiguration 操作の成功の応答: 1 つの保存された検索のための要求</span><span class="sxs-lookup"><span data-stu-id="fd5d1-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="fd5d1-145">「MyDiscSearchFor sbrown」と呼ばれる、保存された検索の構成を取得するのには、 **GetDiscoverySearchConfiguration**操作の要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="fd5d1-146">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd5d1-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="fd5d1-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="fd5d1-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd5d1-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd5d1-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="fd5d1-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="fd5d1-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd5d1-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="fd5d1-151">SearchId</span><span class="sxs-lookup"><span data-stu-id="fd5d1-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="fd5d1-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="fd5d1-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="fd5d1-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="fd5d1-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="fd5d1-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="fd5d1-155">Guid</span><span class="sxs-lookup"><span data-stu-id="fd5d1-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fd5d1-156">PrimarySmtpAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="fd5d1-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="fd5d1-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="fd5d1-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="fd5d1-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fd5d1-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="fd5d1-159">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="fd5d1-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="fd5d1-160">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="fd5d1-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="fd5d1-161">参照 id が</span><span class="sxs-lookup"><span data-stu-id="fd5d1-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="fd5d1-162">GetDiscoverySearchConfiguration 操作の成功の応答: 要求を保持する場所で</span><span class="sxs-lookup"><span data-stu-id="fd5d1-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="fd5d1-163">のみ埋め込みを取得する**GetDiscoverySearchConfiguration**操作要求に正常な応答を保持するは、次の例です。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="fd5d1-164">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd5d1-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="fd5d1-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="fd5d1-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd5d1-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd5d1-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="fd5d1-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="fd5d1-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd5d1-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="fd5d1-169">SearchId</span><span class="sxs-lookup"><span data-stu-id="fd5d1-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="fd5d1-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="fd5d1-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="fd5d1-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="fd5d1-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="fd5d1-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="fd5d1-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="fd5d1-173">GetDiscoverySearchConfiguration 操作の成功の応答: 検出の検索設定を保存すべての要求</span><span class="sxs-lookup"><span data-stu-id="fd5d1-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="fd5d1-174">次の例では、すべての保存された検索を取得する**GetDiscoverySearchConfiguration**操作要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="fd5d1-175">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd5d1-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="fd5d1-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="fd5d1-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd5d1-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd5d1-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="fd5d1-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="fd5d1-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd5d1-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="fd5d1-180">SearchId</span><span class="sxs-lookup"><span data-stu-id="fd5d1-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="fd5d1-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="fd5d1-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="fd5d1-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="fd5d1-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="fd5d1-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="fd5d1-184">Guid</span><span class="sxs-lookup"><span data-stu-id="fd5d1-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fd5d1-185">PrimarySmtpAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="fd5d1-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="fd5d1-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="fd5d1-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="fd5d1-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fd5d1-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="fd5d1-188">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="fd5d1-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="fd5d1-189">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="fd5d1-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="fd5d1-190">参照 id が</span><span class="sxs-lookup"><span data-stu-id="fd5d1-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="fd5d1-191">GetDiscoverySearchConfiguration 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="fd5d1-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="fd5d1-192">**GetDiscoverySearchConfiguration**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="fd5d1-193">これは、サーバー上で含まれていない保存済みサーチを取得する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="fd5d1-194">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd5d1-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="fd5d1-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="fd5d1-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="fd5d1-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fd5d1-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd5d1-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd5d1-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fd5d1-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fd5d1-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="fd5d1-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="fd5d1-200">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd5d1-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="fd5d1-201">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd5d1-201">See also</span></span>

- [<span data-ttu-id="fd5d1-202">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="fd5d1-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="fd5d1-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="fd5d1-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="fd5d1-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="fd5d1-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fd5d1-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="fd5d1-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="fd5d1-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="fd5d1-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="fd5d1-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

