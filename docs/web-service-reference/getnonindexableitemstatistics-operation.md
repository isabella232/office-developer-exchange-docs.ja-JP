---
title: GetNonIndexableItemStatistics 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: GetNonIndexableItemStatistics EWS 操作についての情報を検索します。
ms.openlocfilehash: c7d49f9e0d7b4191c7403cb4d1a20e70a96c3882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452819"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="703c1-103">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="703c1-104">**Getnonindexableitemstatistics** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="703c1-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="703c1-105">**Getnonindexableitemstatistics**操作は、メールボックス内のインデックスを作成できないアイテムの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="703c1-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="703c1-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="703c1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="703c1-107">GetNonIndexableItemStatistics 操作の使用</span><span class="sxs-lookup"><span data-stu-id="703c1-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="703c1-108">**Getnonindexableitemstatistics**操作は、インデックスを作成できないメールボックスアイテムをカウントします。</span><span class="sxs-lookup"><span data-stu-id="703c1-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="703c1-109">インデックスを作成できないアイテムは、探索検索時に検索されません。</span><span class="sxs-lookup"><span data-stu-id="703c1-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="703c1-110">GetNonIndexableItemStatistics 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="703c1-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="703c1-111">**Getnonindexableitemstatistics**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="703c1-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="703c1-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="703c1-112">**Header name**</span></span>|<span data-ttu-id="703c1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="703c1-113">**Element**</span></span>|<span data-ttu-id="703c1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="703c1-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="703c1-115">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="703c1-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="703c1-116">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="703c1-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="703c1-117">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="703c1-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="703c1-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="703c1-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="703c1-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="703c1-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="703c1-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="703c1-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="703c1-121">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="703c1-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="703c1-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="703c1-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="703c1-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="703c1-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="703c1-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="703c1-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="703c1-125">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="703c1-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="703c1-126">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="703c1-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="703c1-127">GetNonIndexableItemStatistics 操作要求の例: メールボックス内にインデックスを作成できないアイテムの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="703c1-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="703c1-128">次の**Getnonindexableitemstatistics**操作要求の例は、メールボックス内にインデックスを作成できないアイテムの数を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="703c1-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="703c1-129">この例の従来のドメイン名はすべて、読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="703c1-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemStatistics>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIDLT)/cn=Recipients/cn=3518cf-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemStatistics>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="703c1-130">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="703c1-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="703c1-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="703c1-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="703c1-132">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="703c1-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="703c1-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="703c1-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="703c1-134">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="703c1-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="703c1-135">GetNonIndexableItemStatistics 操作の応答が正常に行われる</span><span class="sxs-lookup"><span data-stu-id="703c1-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="703c1-136">次の例は、メールボックス内にインデックスを作成できないアイテムの数を取得する**Getnonindexableitemstatistics**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="703c1-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="703c1-137">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="703c1-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="703c1-138">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="703c1-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="703c1-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="703c1-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="703c1-140">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="703c1-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="703c1-141">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="703c1-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="703c1-142">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="703c1-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="703c1-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="703c1-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="703c1-144">GetNonIndexableItemStatistics 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="703c1-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="703c1-145">次の例は、 **Getnonindexableitemstatistics**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="703c1-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="703c1-146">これは、複数のメールボックスからインデックスを作成できないアイテムの数を取得する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="703c1-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="703c1-147">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="703c1-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="703c1-148">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="703c1-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="703c1-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="703c1-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="703c1-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="703c1-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="703c1-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="703c1-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="703c1-152">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="703c1-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="703c1-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="703c1-153">See also</span></span>

- [<span data-ttu-id="703c1-154">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="703c1-155">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="703c1-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="703c1-156">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="703c1-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="703c1-157">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="703c1-158">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="703c1-159">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="703c1-160">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="703c1-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

