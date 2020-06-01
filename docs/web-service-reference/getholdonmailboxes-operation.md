---
title: GetHoldOnMailboxes 操作
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: GetHoldOnMailboxes EWS 操作についての情報を検索します。
ms.openlocfilehash: 867f38be87e60af8708eeb0b9d0e3ac8eee6ff64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457733"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="cbcd5-103">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-103">GetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cbcd5-104">2020年4月1日以降、Exchange Online では GetHoldOnMailboxes 操作が使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-104">Starting on April 1, 2020, the GetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="cbcd5-105">この操作は、Exchange Server のオンプレミスバージョンでは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="cbcd5-106">詳細については、「 [Exchange Online の従来の電子情報開示ツールの廃止](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="cbcd5-107">**GetHoldOnMailboxes** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-107">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="cbcd5-108">**GetHoldOnMailboxes**操作は、特定の保留中のメールボックスと、それに関連付けられている保留クエリを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-108">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="cbcd5-109">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="cbcd5-110">GetHoldOnMailboxes 操作の使用</span><span class="sxs-lookup"><span data-stu-id="cbcd5-110">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="cbcd5-111">**GetHoldOnMailboxes**操作は、特定のホールドの下に配置されるメールボックス、各保留リストに関連付けられた保留クエリに関する情報、各メールボックスの保留状態に関する情報をクライアントに提供します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-111">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="cbcd5-112">クエリベースの保持を含む、メールボックス保持の詳細については、TechNet の「[インプレースホールド](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-112">For more information about mailbox holds, including query-based holds, see [In-Place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="cbcd5-113">GetHoldOnMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbcd5-113">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="cbcd5-114">**GetHoldOnMailboxes**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-114">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cbcd5-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-115">**Header name**</span></span>|<span data-ttu-id="cbcd5-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-116">**Element**</span></span>|<span data-ttu-id="cbcd5-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cbcd5-118">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-118">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="cbcd5-119">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="cbcd5-119">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="cbcd5-120">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-120">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="cbcd5-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cbcd5-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cbcd5-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cbcd5-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cbcd5-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cbcd5-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cbcd5-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cbcd5-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cbcd5-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cbcd5-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cbcd5-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cbcd5-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="cbcd5-130">GetHoldOnMailboxes 操作要求の例: メールボックスの保持情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-130">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="cbcd5-131">次の**GetHoldOnMailboxes**操作要求の例は、HoldId2 メールボックスホールドのメールボックス保持情報を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-131">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="cbcd5-132">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbcd5-133">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="cbcd5-133">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="cbcd5-134">HoldId</span><span class="sxs-lookup"><span data-stu-id="cbcd5-134">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="cbcd5-135">成功した GetHoldOnMailboxes 操作の応答</span><span class="sxs-lookup"><span data-stu-id="cbcd5-135">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="cbcd5-136">次の例は、HoldId2 メールボックスホールドのメールボックス保持情報を取得するための**GetHoldOnMailboxes**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-136">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="cbcd5-137">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbcd5-138">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="cbcd5-138">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="cbcd5-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cbcd5-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cbcd5-140">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="cbcd5-140">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="cbcd5-141">HoldId</span><span class="sxs-lookup"><span data-stu-id="cbcd5-141">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="cbcd5-142">Query</span><span class="sxs-lookup"><span data-stu-id="cbcd5-142">Query</span></span>](query.md)
    
- [<span data-ttu-id="cbcd5-143">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="cbcd5-143">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="cbcd5-144">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="cbcd5-144">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="cbcd5-145">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cbcd5-145">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cbcd5-146">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="cbcd5-146">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="cbcd5-147">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="cbcd5-147">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="cbcd5-148">GetHoldOnMailboxes 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="cbcd5-148">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="cbcd5-149">次の例は、 **GetHoldOnMailboxes**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-149">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="cbcd5-150">これは、削除された保留リストを取得するための要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-150">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="cbcd5-151">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbcd5-151">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbcd5-152">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="cbcd5-152">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="cbcd5-153">MessageText</span><span class="sxs-lookup"><span data-stu-id="cbcd5-153">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cbcd5-154">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cbcd5-154">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cbcd5-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cbcd5-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="cbcd5-156">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="cbcd5-156">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cbcd5-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbcd5-157">See also</span></span>

- [<span data-ttu-id="cbcd5-158">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="cbcd5-159">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-159">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="cbcd5-160">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-160">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="cbcd5-161">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-161">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="cbcd5-162">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-162">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="cbcd5-163">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-163">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="cbcd5-164">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="cbcd5-164">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

