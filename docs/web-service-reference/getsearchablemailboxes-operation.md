---
title: Getsearchablemailemail箱操作
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Getsearchablemailemailbyews 操作についての情報を検索します。
ms.openlocfilehash: e893a66eb1b638479eeccc6bd7548cb020f37243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530840"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="db192-103">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="db192-103">GetSearchableMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="db192-104">2020年4月1日以降、GetSearchableMailboxes 操作は、Exchange Online では使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="db192-104">Starting on April 1, 2020, the GetSearchableMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="db192-105">この操作は、Exchange Server のオンプレミスバージョンでは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="db192-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="db192-106">詳細については、「 [Exchange Online の従来の電子情報開示ツールの廃止](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db192-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="db192-107">**Getsearchablemailemailbyews**操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="db192-107">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="db192-108">**Getsearchablemailbyoperation**は、検索検索用の検索可能な検索可能なメールボックスのスコープセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="db192-108">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="db192-109">応答で返される検索可能なメールボックスの範囲は、検索フィルターと、配布グループのメンバーシップが展開されているかどうかによって決まります。</span><span class="sxs-lookup"><span data-stu-id="db192-109">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 

> [!NOTE] 
> <span data-ttu-id="db192-110">この操作は、検索フィルターで使用され、最初の数千のみを取得することを目的としています。これは、網羅的な取得を目的としたものではありません。</span><span class="sxs-lookup"><span data-stu-id="db192-110">This operation is intended to be used with the search filter and to retrieve only the first few thousands; it's not intended for exhaustive retrieval.</span></span>
  
<span data-ttu-id="db192-111">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db192-111">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="db192-112">Getsearchablemailemailthe 操作の使用</span><span class="sxs-lookup"><span data-stu-id="db192-112">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="db192-113">**Getsearchablemailemail箱**操作は、検索可能なメールボックスに関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="db192-113">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="db192-114">要求では、次の引数を渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="db192-114">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="db192-115">[Searchfilter](searchfilter.md) -単一の電子メールエイリアスを引数として受け入れます。</span><span class="sxs-lookup"><span data-stu-id="db192-115">[SearchFilter](searchfilter.md) - Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="db192-116">[Expandgroupmembership](expandgroupmembership.md) -応答で返された結果で配布グループのメンバーシップが展開されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db192-116">[ExpandGroupMembership](expandgroupmembership.md) - Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="db192-117">検索フィルターに設定されている電子メールエイリアスが配布グループであり、配布グループのメンバーシップが展開されていない場合、応答には配布グループのメールボックス情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="db192-117">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="db192-118">検索フィルターに設定されている電子メールエイリアスが配布グループであり、配布グループのメンバーシップが展開されている場合、応答には、配布グループのメンバーである各メールボックスのメールボックス情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="db192-118">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="db192-119">検索フィルターに1人のユーザーのエイリアスが含まれている場合、応答には1人のユーザーのメールボックス情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="db192-119">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="db192-120">[Getsearchablemailboxes](getsearchablemailboxes.md)要素が空の場合、応答には検索可能なすべてのメールボックスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="db192-120">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="db192-121">これは、空の[Searchfilter](searchfilter.md)要素を持ち、 [expandgroupmembership](expandgroupmembership.md)要素が**false**に設定されているのと同じです。</span><span class="sxs-lookup"><span data-stu-id="db192-121">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="db192-122">GetSearchableMailboxes ボックス操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db192-122">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="db192-123">**Getsearchablemailemail箱**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="db192-123">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="db192-124">ヘッダー名</span><span class="sxs-lookup"><span data-stu-id="db192-124">Header name</span></span>|<span data-ttu-id="db192-125">要素</span><span class="sxs-lookup"><span data-stu-id="db192-125">Element</span></span>|<span data-ttu-id="db192-126">説明</span><span class="sxs-lookup"><span data-stu-id="db192-126">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="db192-127">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="db192-127">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="db192-128">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="db192-128">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="db192-129">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="db192-129">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="db192-130">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="db192-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="db192-131">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="db192-131">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="db192-132">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="db192-132">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="db192-133">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="db192-133">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="db192-134">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="db192-134">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="db192-135">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="db192-135">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="db192-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="db192-136">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="db192-137">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="db192-137">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="db192-138">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="db192-138">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="db192-139">Getsearchablemailemailoperation 要求の例: 配布グループに関する情報を要求します。</span><span class="sxs-lookup"><span data-stu-id="db192-139">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="db192-140">次の**Getsearchablemailboxes**操作要求の例は、lolgroup 配布グループのメールボックス情報を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="db192-140">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="db192-141">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="db192-141">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="db192-142">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="db192-142">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)   
- [<span data-ttu-id="db192-143">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="db192-143">SearchFilter</span></span>](searchfilter.md)    
- [<span data-ttu-id="db192-144">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="db192-144">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="db192-145">Successful Getsearchablemailbyoperation response: 配布グループに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="db192-145">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="db192-146">次の例は、lolgroup 配布グループの検出情報を取得するための**Getsearchablemailboxes**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="db192-146">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="db192-147">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="db192-147">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="db192-148">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="db192-148">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)   
- [<span data-ttu-id="db192-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db192-149">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="db192-150">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="db192-150">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="db192-151">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="db192-151">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="db192-152">Guid</span><span class="sxs-lookup"><span data-stu-id="db192-152">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="db192-153">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="db192-153">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="db192-154">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="db192-154">IsExternalMailbox</span></span>](isexternalmailbox.md)   
- [<span data-ttu-id="db192-155">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="db192-155">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="db192-156">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="db192-156">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="db192-157">Isメンバーシップグループ</span><span class="sxs-lookup"><span data-stu-id="db192-157">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="db192-158">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="db192-158">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="db192-159">Successful Getsearchablemailaddressoperation response: 展開された配布グループに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="db192-159">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="db192-160">次の例は、拡張された lolgroup 配布グループのメンバーに関する検出情報を取得するために、 **Getsearchablemailboxes**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="db192-160">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="db192-161">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="db192-161">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="db192-162">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="db192-162">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)    
- [<span data-ttu-id="db192-163">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db192-163">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="db192-164">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="db192-164">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="db192-165">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="db192-165">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="db192-166">Guid</span><span class="sxs-lookup"><span data-stu-id="db192-166">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="db192-167">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="db192-167">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="db192-168">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="db192-168">IsExternalMailbox</span></span>](isexternalmailbox.md)    
- [<span data-ttu-id="db192-169">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="db192-169">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="db192-170">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="db192-170">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="db192-171">Isメンバーシップグループ</span><span class="sxs-lookup"><span data-stu-id="db192-171">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="db192-172">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="db192-172">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="db192-173">GetSearchableMailboxes ボックス操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="db192-173">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="db192-174">次の例は、 **Getsearchablemailaddressoperation**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="db192-174">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="db192-175">これは、 **Expandgroupmembership**引数が**true**に設定されている場合に、検索可能なメールボックスをすべて取得する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="db192-175">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="db192-176">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="db192-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="db192-177">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="db192-177">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)  
- [<span data-ttu-id="db192-178">MessageText</span><span class="sxs-lookup"><span data-stu-id="db192-178">MessageText</span></span>](messagetext.md)   
- [<span data-ttu-id="db192-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db192-179">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="db192-180">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="db192-180">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) 
- [<span data-ttu-id="db192-181">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="db192-181">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="db192-182">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="db192-182">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="db192-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="db192-183">See also</span></span>

- [<span data-ttu-id="db192-184">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="db192-184">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="db192-185">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="db192-185">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)   
- [<span data-ttu-id="db192-186">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="db192-186">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)   
- [<span data-ttu-id="db192-187">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="db192-187">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)    
- [<span data-ttu-id="db192-188">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="db192-188">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)   
- [<span data-ttu-id="db192-189">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="db192-189">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)   
- [<span data-ttu-id="db192-190">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="db192-190">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

