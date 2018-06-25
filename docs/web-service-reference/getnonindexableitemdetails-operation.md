---
title: GetNonIndexableItemDetails 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: 操作 GetNonIndexableItemDetails EWS についての情報を検索します。
ms.openlocfilehash: 6b0c5afd54ac98f89bc6c5199300c20862c6f207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760799"
---
# <a name="getnonindexableitemdetails-operation"></a><span data-ttu-id="faada-103">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="faada-103">GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="faada-104">**GetNonIndexableItemDetails** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="faada-104">Find information about the **GetNonIndexableItemDetails** EWS operation.</span></span> 
  
<span data-ttu-id="faada-105">**GetNonIndexableItemDetails**操作は、インデックスを作成できないアイテムの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="faada-105">The **GetNonIndexableItemDetails** operation retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="faada-106">これが含まれているが、項目、およびファイルに関する追加情報のインデックスを作成しようとしたときに、項目 id、エラー コード、エラーの説明ではありません。</span><span class="sxs-lookup"><span data-stu-id="faada-106">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="faada-107">スキーマを示していますが、複数のメールボックスで検索できる、Exchange 2013 年の最初のリリース版サービスはのみ 1 つのメールボックス内の nonindexable の項目の項目詳細の取得をサポートします。</span><span class="sxs-lookup"><span data-stu-id="faada-107">Although the schema indicates that more than one mailbox can be searched, in the initial release version of Exchange 2013, the service only supports getting item details for nonindexable items in a single mailbox.</span></span> 
  
<span data-ttu-id="faada-108">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="faada-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemdetails-operation"></a><span data-ttu-id="faada-109">GetNonIndexableItemDetails 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="faada-109">Using the GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="faada-110">**GetNonIndexableItemDetails**操作は、インデックスを作成することはできませんメールボックス アイテムを識別し、項目のインデックスを作成できない理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="faada-110">The **GetNonIndexableItemDetails** operation identifies mailbox items that cannot be indexed and provides information about why the items cannot be indexed.</span></span> <span data-ttu-id="faada-111">探索検索時にインデックスを作成できないアイテムは検索されません。</span><span class="sxs-lookup"><span data-stu-id="faada-111">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a><span data-ttu-id="faada-112">GetNonIndexableItemDetails 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faada-112">GetNonIndexableItemDetails operation SOAP headers</span></span>

<span data-ttu-id="faada-113">**GetNonIndexableItemDetails**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="faada-113">The **GetNonIndexableItemDetails** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="faada-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="faada-114">**Header name**</span></span>|<span data-ttu-id="faada-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="faada-115">**Element**</span></span>|<span data-ttu-id="faada-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="faada-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="faada-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="faada-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="faada-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="faada-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="faada-119">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="faada-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="faada-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="faada-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="faada-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="faada-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="faada-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="faada-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="faada-123">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="faada-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="faada-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="faada-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="faada-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="faada-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="faada-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="faada-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="faada-127">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="faada-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="faada-128">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="faada-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a><span data-ttu-id="faada-129">GetNonIndexableItemDetails 操作の要求の例: インデックスを作成することはできませんが、項目の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="faada-129">GetNonIndexableItemDetails operation request example: Get the details of an item that cannot be indexed</span></span>

<span data-ttu-id="faada-130">**GetNonIndexableItemDetails**操作要求の次の使用例は、1 つのメールボックスに対してインデックスを作成できないアイテムの詳細を要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="faada-130">The following example of a **GetNonIndexableItemDetails** operation request shows how to request the details for items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="faada-131">プライマリの両方で検索を実行し、メールボックスのアーカイブです。</span><span class="sxs-lookup"><span data-stu-id="faada-131">The search is performed across both primary and archive mailboxes.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="faada-132">読みやすさを保持するのには、この例ではすべての以前のドメイン名が短縮されます。</span><span class="sxs-lookup"><span data-stu-id="faada-132">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="faada-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faada-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="faada-134">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="faada-134">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="faada-135">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="faada-135">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="faada-136">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="faada-136">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="faada-137">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="faada-137">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a><span data-ttu-id="faada-138">GetNonIndexableItemDetails 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="faada-138">Successful GetNonIndexableItemDetails operation response</span></span>

<span data-ttu-id="faada-139">次の例では、1 つのメールボックスのインデックスを作成できないアイテムを取得する**GetNonIndexableItemDetails**操作要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="faada-139">The following example shows a successful response to a **GetNonIndexableItemDetails** operation request to get items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="faada-140">この例ではインデックスを作成できないアイテムは、形式が不明なは、binaryfile.abc ファイルです。</span><span class="sxs-lookup"><span data-stu-id="faada-140">The item in this example that cannot be indexed is the binaryfile.abc file, which is of an unknown format.</span></span> 
  
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
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="faada-141">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faada-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="faada-142">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="faada-142">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="faada-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="faada-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="faada-144">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="faada-144">NonIndexableItemDetailsResult</span></span>](nonindexableitemdetailsresult.md)
    
- [<span data-ttu-id="faada-145">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="faada-145">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
    
- [<span data-ttu-id="faada-146">ItemId</span><span class="sxs-lookup"><span data-stu-id="faada-146">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="faada-147">エラー コード (ItemIndexErrorType)</span><span class="sxs-lookup"><span data-stu-id="faada-147">ErrorCode (ItemIndexErrorType)</span></span>](errorcode-itemindexerrortype.md)
    
- [<span data-ttu-id="faada-148">ErrorDescription</span><span class="sxs-lookup"><span data-stu-id="faada-148">ErrorDescription</span></span>](errordescription.md)
    
- [<span data-ttu-id="faada-149">IsPartiallyIndexed</span><span class="sxs-lookup"><span data-stu-id="faada-149">IsPartiallyIndexed</span></span>](ispartiallyindexed.md)
    
- [<span data-ttu-id="faada-150">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="faada-150">IsPermanentFailure</span></span>](ispermanentfailure.md)
    
- [<span data-ttu-id="faada-151">SortValue</span><span class="sxs-lookup"><span data-stu-id="faada-151">SortValue</span></span>](sortvalue.md)
    
- [<span data-ttu-id="faada-152">AttemptCount</span><span class="sxs-lookup"><span data-stu-id="faada-152">AttemptCount</span></span>](attemptcount.md)
    
- [<span data-ttu-id="faada-153">LastAttemptTime</span><span class="sxs-lookup"><span data-stu-id="faada-153">LastAttemptTime</span></span>](lastattempttime.md)
    
- [<span data-ttu-id="faada-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="faada-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a><span data-ttu-id="faada-155">GetNonIndexableItemDetails 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="faada-155">GetNonIndexableItemDetails operation error response</span></span>

<span data-ttu-id="faada-156">**GetNonIndexableItemDetails**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="faada-156">The following example shows an error response to a **GetNonIndexableItemDetails** operation request.</span></span> <span data-ttu-id="faada-157">これは、複数のメールボックスからインデックスを作成できないアイテムの項目の詳細を取得する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="faada-157">This is a response to a request to get item details for items that cannot be indexed from more than one mailbox.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="faada-158">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faada-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="faada-159">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="faada-159">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="faada-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="faada-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="faada-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="faada-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="faada-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="faada-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="faada-163">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faada-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="faada-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="faada-164">See also</span></span>

- [<span data-ttu-id="faada-165">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="faada-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="faada-166">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="faada-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="faada-167">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="faada-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="faada-168">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="faada-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="faada-169">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="faada-169">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="faada-170">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="faada-170">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="faada-171">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="faada-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

