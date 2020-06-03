---
title: GetNonIndexableItemDetails 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: GetNonIndexableItemDetails EWS 操作についての情報を検索します。
ms.openlocfilehash: a443e04b0622ddbaaeb1bc8c04bfd05679c6207e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530212"
---
# <a name="getnonindexableitemdetails-operation"></a><span data-ttu-id="e94e8-103">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-103">GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="e94e8-104">**Getnonindexableitemdetails** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-104">Find information about the **GetNonIndexableItemDetails** EWS operation.</span></span> 
  
<span data-ttu-id="e94e8-105">**Getnonindexableitemdetails**操作は、インデックスを作成できないアイテムに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-105">The **GetNonIndexableItemDetails** operation retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="e94e8-106">これには、アイテム識別子、エラー コード、エラーの説明、アイテムのインデックス作成をしようとしたタイミング、ファイルに関する追加情報が含まれますが、これに限定されません。</span><span class="sxs-lookup"><span data-stu-id="e94e8-106">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e94e8-107">このスキーマは複数のメールボックスを検索できることを示していますが、Exchange 2013 の最初のリリースバージョンでは、サービスは単一のメールボックス内のインデックス付けされていないアイテムについてのみアイテムの詳細を取得することをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-107">Although the schema indicates that more than one mailbox can be searched, in the initial release version of Exchange 2013, the service only supports getting item details for nonindexable items in a single mailbox.</span></span> 
  
<span data-ttu-id="e94e8-108">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e94e8-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemdetails-operation"></a><span data-ttu-id="e94e8-109">GetNonIndexableItemDetails 操作の使用</span><span class="sxs-lookup"><span data-stu-id="e94e8-109">Using the GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="e94e8-110">**Getnonindexableitemdetails**操作は、インデックスを作成できないメールボックスアイテムを識別し、アイテムのインデックスを作成できない理由についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-110">The **GetNonIndexableItemDetails** operation identifies mailbox items that cannot be indexed and provides information about why the items cannot be indexed.</span></span> <span data-ttu-id="e94e8-111">インデックスを作成できないアイテムは、探索検索時に検索されません。</span><span class="sxs-lookup"><span data-stu-id="e94e8-111">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a><span data-ttu-id="e94e8-112">GetNonIndexableItemDetails 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e94e8-112">GetNonIndexableItemDetails operation SOAP headers</span></span>

<span data-ttu-id="e94e8-113">**Getnonindexableitemdetails**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e94e8-113">The **GetNonIndexableItemDetails** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e94e8-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="e94e8-114">**Header name**</span></span>|<span data-ttu-id="e94e8-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="e94e8-115">**Element**</span></span>|<span data-ttu-id="e94e8-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="e94e8-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e94e8-117">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="e94e8-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="e94e8-118">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="e94e8-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="e94e8-119">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="e94e8-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e94e8-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e94e8-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e94e8-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e94e8-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e94e8-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e94e8-123">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e94e8-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e94e8-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e94e8-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e94e8-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e94e8-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e94e8-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e94e8-127">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e94e8-128">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e94e8-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a><span data-ttu-id="e94e8-129">GetNonIndexableItemDetails 操作要求の例: インデックスを作成できないアイテムの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-129">GetNonIndexableItemDetails operation request example: Get the details of an item that cannot be indexed</span></span>

<span data-ttu-id="e94e8-130">次の**Getnonindexableitemdetails**操作要求の例は、単一のメールボックスに対してインデックスを作成できないアイテムの詳細を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-130">The following example of a **GetNonIndexableItemDetails** operation request shows how to request the details for items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="e94e8-131">検索は、プライマリメールボックスとアーカイブメールボックスの両方に対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="e94e8-131">The search is performed across both primary and archive mailboxes.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e94e8-132">この例の従来のドメイン名はすべて、読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-132">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="e94e8-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e94e8-134">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="e94e8-134">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="e94e8-135">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="e94e8-135">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="e94e8-136">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="e94e8-136">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="e94e8-137">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="e94e8-137">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a><span data-ttu-id="e94e8-138">成功した GetNonIndexableItemDetails 操作の応答</span><span class="sxs-lookup"><span data-stu-id="e94e8-138">Successful GetNonIndexableItemDetails operation response</span></span>

<span data-ttu-id="e94e8-139">次の例は、 **Getnonindexableitemdetails**操作要求に対する正常な応答を示しています。1つのメールボックスに対してインデックスを作成できないアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="e94e8-139">The following example shows a successful response to a **GetNonIndexableItemDetails** operation request to get items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="e94e8-140">この例のインデックス化できないアイテムは、バイナリファイル abc ファイルで、形式が不明です。</span><span class="sxs-lookup"><span data-stu-id="e94e8-140">The item in this example that cannot be indexed is the binaryfile.abc file, which is of an unknown format.</span></span> 
  
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
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="e94e8-141">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e94e8-142">Getnonindexableitem、Response</span><span class="sxs-lookup"><span data-stu-id="e94e8-142">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="e94e8-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e94e8-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e94e8-144">Nonindexableitemの取得結果</span><span class="sxs-lookup"><span data-stu-id="e94e8-144">NonIndexableItemDetailsResult</span></span>](nonindexableitemdetailsresult.md)
    
- [<span data-ttu-id="e94e8-145">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="e94e8-145">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
    
- [<span data-ttu-id="e94e8-146">ItemId</span><span class="sxs-lookup"><span data-stu-id="e94e8-146">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="e94e8-147">ErrorCode (ItemIndexErrorType)</span><span class="sxs-lookup"><span data-stu-id="e94e8-147">ErrorCode (ItemIndexErrorType)</span></span>](errorcode-itemindexerrortype.md)
    
- [<span data-ttu-id="e94e8-148">ErrorDescription</span><span class="sxs-lookup"><span data-stu-id="e94e8-148">ErrorDescription</span></span>](errordescription.md)
    
- [<span data-ttu-id="e94e8-149">Ispartiのインデックス付き</span><span class="sxs-lookup"><span data-stu-id="e94e8-149">IsPartiallyIndexed</span></span>](ispartiallyindexed.md)
    
- [<span data-ttu-id="e94e8-150">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="e94e8-150">IsPermanentFailure</span></span>](ispermanentfailure.md)
    
- [<span data-ttu-id="e94e8-151">SortValue</span><span class="sxs-lookup"><span data-stu-id="e94e8-151">SortValue</span></span>](sortvalue.md)
    
- [<span data-ttu-id="e94e8-152">AttemptCount</span><span class="sxs-lookup"><span data-stu-id="e94e8-152">AttemptCount</span></span>](attemptcount.md)
    
- [<span data-ttu-id="e94e8-153">LastAttemptTime</span><span class="sxs-lookup"><span data-stu-id="e94e8-153">LastAttemptTime</span></span>](lastattempttime.md)
    
- [<span data-ttu-id="e94e8-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="e94e8-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a><span data-ttu-id="e94e8-155">GetNonIndexableItemDetails 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="e94e8-155">GetNonIndexableItemDetails operation error response</span></span>

<span data-ttu-id="e94e8-156">次の例は、 **Getnonindexableitemdetails**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-156">The following example shows an error response to a **GetNonIndexableItemDetails** operation request.</span></span> <span data-ttu-id="e94e8-157">これは、複数のメールボックスからインデックスを作成できないアイテムのアイテムの詳細を取得する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="e94e8-157">This is a response to a request to get item details for items that cannot be indexed from more than one mailbox.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e94e8-158">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e94e8-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e94e8-159">Getnonindexableitem、Response</span><span class="sxs-lookup"><span data-stu-id="e94e8-159">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="e94e8-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="e94e8-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e94e8-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e94e8-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e94e8-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e94e8-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="e94e8-163">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="e94e8-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e94e8-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="e94e8-164">See also</span></span>

- [<span data-ttu-id="e94e8-165">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="e94e8-166">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="e94e8-167">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="e94e8-168">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="e94e8-169">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-169">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="e94e8-170">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-170">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="e94e8-171">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="e94e8-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

