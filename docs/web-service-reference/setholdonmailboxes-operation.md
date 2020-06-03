---
title: SetHoldOnMailboxes 操作
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: SetHoldOnMailboxes EWS 操作についての情報を検索します。
ms.openlocfilehash: 4d79ba9f616974b9415ae9eae23b8f5fdb0ab205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448395"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="00c9e-103">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-103">SetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="00c9e-104">2020年4月1日以降、Exchange Online では SetHoldOnMailboxes 操作が使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="00c9e-104">Starting on April 1, 2020, the SetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="00c9e-105">この操作は、Exchange Server のオンプレミスバージョンでは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="00c9e-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="00c9e-106">詳細については、「 [Exchange Online の従来の電子情報開示ツールの廃止](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00c9e-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="00c9e-107">**SetHoldOnMailboxes** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-107">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="00c9e-108">**SetHoldOnMailboxes**操作は、メールボックスのメールボックス保持ポリシーを設定します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-108">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="00c9e-109">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="00c9e-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="00c9e-110">SetHoldOnMailboxes 操作の使用</span><span class="sxs-lookup"><span data-stu-id="00c9e-110">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="00c9e-111">**SetHoldOnMailboxes**操作では、メールボックスホールドを1つ以上のメールボックスに設定します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-111">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="00c9e-112">SetHoldOnMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00c9e-112">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="00c9e-113">**SetHoldOnMailboxes**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="00c9e-113">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="00c9e-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="00c9e-114">**Header name**</span></span>|<span data-ttu-id="00c9e-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="00c9e-115">**Element**</span></span>|<span data-ttu-id="00c9e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="00c9e-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00c9e-117">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="00c9e-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="00c9e-118">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="00c9e-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="00c9e-119">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="00c9e-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="00c9e-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="00c9e-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="00c9e-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="00c9e-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="00c9e-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="00c9e-123">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="00c9e-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="00c9e-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="00c9e-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="00c9e-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="00c9e-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="00c9e-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="00c9e-127">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="00c9e-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="00c9e-128">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="00c9e-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="00c9e-129">SetHoldOnMailboxes 操作要求の例: メールボックスに保留を適用する</span><span class="sxs-lookup"><span data-stu-id="00c9e-129">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="00c9e-130">次の**SetHoldOnMailboxes**操作要求の例は、2つのメールボックスに保留を適用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-130">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="00c9e-131">メールボックスの保持は、 [get-mailboxsearch](https://technet.microsoft.com/library/dd298064.aspx)コマンドを使用して作成されました。</span><span class="sxs-lookup"><span data-stu-id="00c9e-131">The mailbox hold was created by using the [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="00c9e-132">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="00c9e-133">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="00c9e-133">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="00c9e-134">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="00c9e-134">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="00c9e-135">HoldId</span><span class="sxs-lookup"><span data-stu-id="00c9e-135">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="00c9e-136">Query</span><span class="sxs-lookup"><span data-stu-id="00c9e-136">Query</span></span>](query.md)
    
- [<span data-ttu-id="00c9e-137">メールボックス (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="00c9e-137">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="00c9e-138">String</span><span class="sxs-lookup"><span data-stu-id="00c9e-138">String</span></span>](string.md)
    
- [<span data-ttu-id="00c9e-139">Language</span><span class="sxs-lookup"><span data-stu-id="00c9e-139">Language</span></span>](language.md)
    
- [<span data-ttu-id="00c9e-140">追加アイテム</span><span class="sxs-lookup"><span data-stu-id="00c9e-140">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="00c9e-141">防止</span><span class="sxs-lookup"><span data-stu-id="00c9e-141">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="00c9e-142">成功した SetHoldOnMailboxes 操作の応答</span><span class="sxs-lookup"><span data-stu-id="00c9e-142">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="00c9e-143">次の例は、2つのメールボックスを保持するための**SetHoldOnMailboxes**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-143">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="00c9e-144">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="00c9e-145">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="00c9e-145">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="00c9e-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00c9e-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="00c9e-147">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="00c9e-147">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="00c9e-148">HoldId</span><span class="sxs-lookup"><span data-stu-id="00c9e-148">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="00c9e-149">Query</span><span class="sxs-lookup"><span data-stu-id="00c9e-149">Query</span></span>](query.md)
    
- [<span data-ttu-id="00c9e-150">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="00c9e-150">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="00c9e-151">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="00c9e-151">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="00c9e-152">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="00c9e-152">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="00c9e-153">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="00c9e-153">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="00c9e-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="00c9e-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="00c9e-155">SetHoldOnMailboxes 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="00c9e-155">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="00c9e-156">次の例は、 **SetHoldOnMailboxes**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-156">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="00c9e-157">これは、正しく指定されていないメールボックス識別子を含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="00c9e-157">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="00c9e-158">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="00c9e-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="00c9e-159">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="00c9e-159">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="00c9e-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="00c9e-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="00c9e-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00c9e-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="00c9e-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="00c9e-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="00c9e-163">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="00c9e-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="00c9e-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="00c9e-164">See also</span></span>

- [<span data-ttu-id="00c9e-165">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="00c9e-166">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="00c9e-167">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="00c9e-168">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="00c9e-169">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-169">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="00c9e-170">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-170">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="00c9e-171">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="00c9e-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

