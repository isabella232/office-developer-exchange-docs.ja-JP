---
title: GetSearchableMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: 操作 GetSearchableMailboxes EWS についての情報を検索します。
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760852"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="97c8c-103">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-103">GetSearchableMailboxes operation</span></span>

<span data-ttu-id="97c8c-104">**GetSearchableMailboxes** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-104">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="97c8c-105">**GetSearchableMailboxes**操作は、スコープ指定された検索の検索可能なメールボックスのセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-105">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="97c8c-106">応答で返されるメールボックスを検索可能なスコープは、検索フィルターと配布グループのメンバーシップを展開するかどうかによって決まります。</span><span class="sxs-lookup"><span data-stu-id="97c8c-106">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 
  
<span data-ttu-id="97c8c-107">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="97c8c-107">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="97c8c-108">GetSearchableMailboxes 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-108">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="97c8c-109">**GetSearchableMailboxes**操作は、検索可能なメールボックスに関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-109">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="97c8c-110">要求では、次の引数を渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-110">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="97c8c-111">[SearchFilter](searchfilter.md) : 引数として 1 つの電子メールのエイリアスを受け入れます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-111">[SearchFilter](searchfilter.md) —Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="97c8c-112">[ExpandGroupMembership](expandgroupmembership.md)応答で返される結果の配布グループのメンバーシップを展開するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="97c8c-113">検索フィルターに設定する電子メール エイリアスは、配布グループと配布グループのメンバーシップは展開されませんが、応答には、配布グループのメールボックスの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-113">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="97c8c-114">検索フィルターに設定する電子メール エイリアスは、配布グループと配布グループのメンバーシップが展開されている、応答には、配布グループのメンバーである各メールボックスのメールボックスの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-114">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="97c8c-115">検索フィルターには、単一のユーザーのエイリアスが含まれています、応答で 1 つのユーザーのメールボックス情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-115">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="97c8c-116">[GetSearchableMailboxes](getsearchablemailboxes.md)要素が空の場合、応答は検索可能なすべてのメールボックスに格納されます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-116">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="97c8c-117">これは、空の[SearchFilter](searchfilter.md)要素と[ExpandGroupMembership](expandgroupmembership.md)要素が**false**に設定することと同じです。</span><span class="sxs-lookup"><span data-stu-id="97c8c-117">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="97c8c-118">GetSearchableMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97c8c-118">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="97c8c-119">**GetSearchableMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-119">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="97c8c-120">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="97c8c-120">**Header name**</span></span>|<span data-ttu-id="97c8c-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="97c8c-121">**Element**</span></span>|<span data-ttu-id="97c8c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="97c8c-122">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="97c8c-123">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="97c8c-123">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="97c8c-124">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="97c8c-124">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="97c8c-125">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-125">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="97c8c-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="97c8c-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="97c8c-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="97c8c-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="97c8c-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="97c8c-129">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="97c8c-130">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="97c8c-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="97c8c-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="97c8c-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="97c8c-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="97c8c-133">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="97c8c-134">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="97c8c-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="97c8c-135">GetSearchableMailboxes 操作の要求の例: 配布グループに関する情報を要求</span><span class="sxs-lookup"><span data-stu-id="97c8c-135">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="97c8c-136">**GetSearchableMailboxes**操作要求の次の例では、lolgroup の配布グループのメールボックス情報を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-136">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="97c8c-137">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97c8c-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="97c8c-138">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97c8c-138">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="97c8c-139">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="97c8c-139">SearchFilter</span></span>](searchfilter.md)
    
- [<span data-ttu-id="97c8c-140">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="97c8c-140">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="97c8c-141">GetSearchableMailboxes 操作の成功の応答: 配布グループに関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-141">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="97c8c-142">Lolgroup の配布グループの検出情報を取得する**GetSearchableMailboxes**操作要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-142">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="97c8c-143">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97c8c-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="97c8c-144">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="97c8c-144">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="97c8c-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="97c8c-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="97c8c-146">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97c8c-146">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="97c8c-147">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="97c8c-147">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="97c8c-148">Guid</span><span class="sxs-lookup"><span data-stu-id="97c8c-148">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="97c8c-149">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="97c8c-149">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="97c8c-150">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="97c8c-150">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="97c8c-151">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="97c8c-151">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="97c8c-152">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="97c8c-152">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="97c8c-153">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="97c8c-153">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="97c8c-154">参照 id が</span><span class="sxs-lookup"><span data-stu-id="97c8c-154">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="97c8c-155">GetSearchableMailboxes 操作の成功の応答: 展開された配布グループに関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-155">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="97c8c-156">検出の lolgroup が展開された配布グループのメンバー情報を取得する**GetSearchableMailboxes**操作の要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-156">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="97c8c-157">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97c8c-157">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="97c8c-158">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="97c8c-158">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="97c8c-159">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="97c8c-159">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="97c8c-160">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97c8c-160">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="97c8c-161">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="97c8c-161">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="97c8c-162">Guid</span><span class="sxs-lookup"><span data-stu-id="97c8c-162">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="97c8c-163">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="97c8c-163">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="97c8c-164">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="97c8c-164">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="97c8c-165">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="97c8c-165">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="97c8c-166">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="97c8c-166">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="97c8c-167">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="97c8c-167">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="97c8c-168">参照 id が</span><span class="sxs-lookup"><span data-stu-id="97c8c-168">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="97c8c-169">GetSearchableMailboxes 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="97c8c-169">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="97c8c-170">**GetSearchableMailboxes**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-170">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="97c8c-171">これは、 **ExpandGroupMembership**引数が**true**に設定すると、検索可能なすべてのメールボックスを取得する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="97c8c-171">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="97c8c-172">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97c8c-172">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="97c8c-173">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="97c8c-173">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="97c8c-174">MessageText</span><span class="sxs-lookup"><span data-stu-id="97c8c-174">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="97c8c-175">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="97c8c-175">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="97c8c-176">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="97c8c-176">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="97c8c-177">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97c8c-177">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="97c8c-178">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97c8c-178">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="97c8c-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="97c8c-179">See also</span></span>

- [<span data-ttu-id="97c8c-180">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-180">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="97c8c-181">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-181">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="97c8c-182">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-182">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="97c8c-183">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-183">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="97c8c-184">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-184">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="97c8c-185">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-185">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="97c8c-186">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="97c8c-186">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

