---
title: GetHoldOnMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: 操作 GetHoldOnMailboxes EWS についての情報を検索します。
ms.openlocfilehash: 1d0bc2f9d26e11d8d2710693d67843ad2f339a5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760748"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="e8adb-103">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-103">GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="e8adb-104">**GetHoldOnMailboxes** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-104">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="e8adb-105">**GetHoldOnMailboxes**操作は、特定の保留中のメールボックスを取得し、それに関連付けられたクエリを保持します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-105">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="e8adb-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8adb-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="e8adb-107">GetHoldOnMailboxes 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-107">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="e8adb-108">**GetHoldOnMailboxes**操作は、クライアントの情報については、メールボックスは、[保留中の特定、該当する場合に、各保留リストに関連付けられている保留中のクエリについての情報と各メールボックスの保留中の状態に関する情報を示します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-108">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="e8adb-109">メールボックスの保留、保留リストのクエリ ベースのなどの詳細については TechNet の[インプレース保持](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8adb-109">For more information about mailbox holds, including query-based holds, see [In-Place Hold](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="e8adb-110">GetHoldOnMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8adb-110">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="e8adb-111">**GetHoldOnMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8adb-111">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e8adb-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="e8adb-112">**Header name**</span></span>|<span data-ttu-id="e8adb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8adb-113">**Element**</span></span>|<span data-ttu-id="e8adb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8adb-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e8adb-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="e8adb-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="e8adb-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="e8adb-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="e8adb-117">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="e8adb-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e8adb-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e8adb-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e8adb-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e8adb-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e8adb-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e8adb-121">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e8adb-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e8adb-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e8adb-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e8adb-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e8adb-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e8adb-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e8adb-125">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e8adb-126">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e8adb-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="e8adb-127">GetHoldOnMailboxes 操作の要求の例: メールボックスの保留中の情報を取得</span><span class="sxs-lookup"><span data-stu-id="e8adb-127">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="e8adb-128">**GetHoldOnMailboxes**操作要求の次の例では、HoldId2 メールボックスの保留中のメールボックスの保持情報を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-128">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="e8adb-129">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8adb-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e8adb-130">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="e8adb-130">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="e8adb-131">HoldId</span><span class="sxs-lookup"><span data-stu-id="e8adb-131">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="e8adb-132">GetHoldOnMailboxes 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="e8adb-132">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="e8adb-133">**GetHoldOnMailboxes**操作を正常な応答を要求、メールボックスを取得するのには次の例では、HoldId2 メールボックスの保留中の情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-133">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="e8adb-134">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8adb-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e8adb-135">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="e8adb-135">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="e8adb-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e8adb-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e8adb-137">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="e8adb-137">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="e8adb-138">HoldId</span><span class="sxs-lookup"><span data-stu-id="e8adb-138">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="e8adb-139">Query</span><span class="sxs-lookup"><span data-stu-id="e8adb-139">Query</span></span>](query.md)
    
- [<span data-ttu-id="e8adb-140">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="e8adb-140">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="e8adb-141">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="e8adb-141">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="e8adb-142">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="e8adb-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="e8adb-143">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="e8adb-143">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="e8adb-144">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="e8adb-144">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="e8adb-145">GetHoldOnMailboxes 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="e8adb-145">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="e8adb-146">**GetHoldOnMailboxes**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-146">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="e8adb-147">これは、削除された保留リストを取得する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="e8adb-147">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="e8adb-148">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8adb-148">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e8adb-149">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="e8adb-149">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="e8adb-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="e8adb-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e8adb-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e8adb-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e8adb-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e8adb-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="e8adb-153">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8adb-153">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e8adb-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8adb-154">See also</span></span>

- [<span data-ttu-id="e8adb-155">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="e8adb-156">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-156">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="e8adb-157">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-157">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="e8adb-158">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="e8adb-159">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="e8adb-160">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="e8adb-161">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="e8adb-161">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

