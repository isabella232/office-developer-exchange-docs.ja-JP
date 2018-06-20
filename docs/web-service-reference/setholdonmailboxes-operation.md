---
title: SetHoldOnMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: 操作 SetHoldOnMailboxes EWS についての情報を検索します。
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833412"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="17cf1-103">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-103">SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="17cf1-104">**SetHoldOnMailboxes** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-104">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="17cf1-105">**SetHoldOnMailboxes**操作では、メールボックスのメールボックスの保持ポリシーを設定します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-105">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="17cf1-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="17cf1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="17cf1-107">SetHoldOnMailboxes 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-107">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="17cf1-108">**SetHoldOnMailboxes**操作は、1 つまたは複数のメールボックスへのメールボックスの保持を設定します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-108">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="17cf1-109">SetHoldOnMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17cf1-109">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="17cf1-110">**SetHoldOnMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="17cf1-110">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="17cf1-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="17cf1-111">**Header name**</span></span>|<span data-ttu-id="17cf1-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="17cf1-112">**Element**</span></span>|<span data-ttu-id="17cf1-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="17cf1-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="17cf1-114">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="17cf1-114">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="17cf1-115">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="17cf1-115">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="17cf1-116">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-116">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="17cf1-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="17cf1-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="17cf1-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="17cf1-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="17cf1-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="17cf1-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="17cf1-120">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="17cf1-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="17cf1-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="17cf1-122">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="17cf1-122">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="17cf1-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="17cf1-123">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="17cf1-124">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-124">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="17cf1-125">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="17cf1-125">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="17cf1-126">SetHoldOnMailboxes 操作の要求の例: メールボックスの保留リストを適用</span><span class="sxs-lookup"><span data-stu-id="17cf1-126">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="17cf1-127">**SetHoldOnMailboxes**操作要求の次の例では、2 つのメールボックスに保留を適用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-127">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="17cf1-128">メールボックスの保留リストは、[新しい MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx)コマンドを使用して作成されました。</span><span class="sxs-lookup"><span data-stu-id="17cf1-128">The mailbox hold was created by using the [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="17cf1-129">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17cf1-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="17cf1-130">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="17cf1-130">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="17cf1-131">ファイアウォール (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="17cf1-131">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="17cf1-132">HoldId</span><span class="sxs-lookup"><span data-stu-id="17cf1-132">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="17cf1-133">Query</span><span class="sxs-lookup"><span data-stu-id="17cf1-133">Query</span></span>](query.md)
    
- [<span data-ttu-id="17cf1-134">メールボックス (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="17cf1-134">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="17cf1-135">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="17cf1-135">String</span></span>](string.md)
    
- [<span data-ttu-id="17cf1-136">Language</span><span class="sxs-lookup"><span data-stu-id="17cf1-136">Language</span></span>](language.md)
    
- [<span data-ttu-id="17cf1-137">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="17cf1-137">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="17cf1-138">重複除外</span><span class="sxs-lookup"><span data-stu-id="17cf1-138">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="17cf1-139">SetHoldOnMailboxes 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="17cf1-139">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="17cf1-140">**SetHoldOnMailboxes**操作に 2 つのメールボックスを配置する要求に正常な応答を保持は、次の例です。</span><span class="sxs-lookup"><span data-stu-id="17cf1-140">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="17cf1-141">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17cf1-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="17cf1-142">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="17cf1-142">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="17cf1-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="17cf1-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="17cf1-144">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="17cf1-144">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="17cf1-145">HoldId</span><span class="sxs-lookup"><span data-stu-id="17cf1-145">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="17cf1-146">Query</span><span class="sxs-lookup"><span data-stu-id="17cf1-146">Query</span></span>](query.md)
    
- [<span data-ttu-id="17cf1-147">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="17cf1-147">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="17cf1-148">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="17cf1-148">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="17cf1-149">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="17cf1-149">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="17cf1-150">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="17cf1-150">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="17cf1-151">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="17cf1-151">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="17cf1-152">SetHoldOnMailboxes 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="17cf1-152">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="17cf1-153">**SetHoldOnMailboxes**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="17cf1-153">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="17cf1-154">これは、メールボックスが正しく指定された識別子を含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="17cf1-154">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="17cf1-155">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17cf1-155">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="17cf1-156">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="17cf1-156">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="17cf1-157">MessageText</span><span class="sxs-lookup"><span data-stu-id="17cf1-157">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="17cf1-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="17cf1-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="17cf1-159">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="17cf1-159">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="17cf1-160">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17cf1-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="17cf1-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="17cf1-161">See also</span></span>

- [<span data-ttu-id="17cf1-162">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="17cf1-163">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-163">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="17cf1-164">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-164">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="17cf1-165">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-165">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="17cf1-166">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-166">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="17cf1-167">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-167">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="17cf1-168">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="17cf1-168">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

