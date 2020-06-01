---
title: GetAppMarketplaceUrl 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: GetAppMarketplaceUrl EWS 操作についての情報を検索します。
ms.openlocfilehash: 6797af44c3aaa6653c440b3d53a282d8c90a4381
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459526"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="dccc2-103">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="dccc2-104">**GetAppMarketplaceUrl** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="dccc2-105">**GetAppMarketplaceUrl**操作は、メールボックスにインストールするアプリを取得するためにクライアントがアクセスできるアプリケーションマーケットプレースの URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="dccc2-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dccc2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="dccc2-107">GetAppMarketplaceUrl 操作の使用</span><span class="sxs-lookup"><span data-stu-id="dccc2-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="dccc2-108">**GetAppMarketplaceUrl**操作では、クライアントがアプリをインストールできる MARKETPLACE の URL を要求する引数はありません。</span><span class="sxs-lookup"><span data-stu-id="dccc2-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="dccc2-109">応答には、アプリマーケットプレースへの URL が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dccc2-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="dccc2-110">GetAppMarketplaceUrl 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dccc2-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="dccc2-111">**GetAppMarketplaceUrl**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="dccc2-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="dccc2-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="dccc2-112">**Header name**</span></span>|<span data-ttu-id="dccc2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dccc2-113">**Element**</span></span>|<span data-ttu-id="dccc2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dccc2-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dccc2-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="dccc2-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="dccc2-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="dccc2-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="dccc2-117">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="dccc2-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="dccc2-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="dccc2-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="dccc2-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="dccc2-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="dccc2-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="dccc2-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="dccc2-122">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="dccc2-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="dccc2-123">GetAppMarketplaceUrl 操作要求の例: メールボックスのアプリマーケットプレース URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="dccc2-124">次の**GetAppMarketplaceUrl**操作要求の例は、メールボックスのアプリマーケットプレース URL を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="dccc2-125">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dccc2-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="dccc2-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="dccc2-127">サポートされている apiversion</span><span class="sxs-lookup"><span data-stu-id="dccc2-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="dccc2-128">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="dccc2-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="dccc2-129">成功した GetAppMarketplaceUrl 操作の応答</span><span class="sxs-lookup"><span data-stu-id="dccc2-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="dccc2-130">次の例は、 **GetAppMarketplaceUrl**操作要求に対する正常な応答を示しています。メールボックスのアプリマーケットプレース URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="dccc2-131">アプリケーションマーケットプレース URL は、読みやすくするために変更されています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="dccc2-132">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dccc2-133">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="dccc2-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="dccc2-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dccc2-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dccc2-135">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="dccc2-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="dccc2-136">GetAppMarketPlaceUrl 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="dccc2-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="dccc2-137">この操作に対して返されたエラーは、正しくないサービス構成に関連付けられているか、または一般的な EWS エラーであることを示します。</span><span class="sxs-lookup"><span data-stu-id="dccc2-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="dccc2-138">EWS で汎用的で、この操作に固有のエラーコードについては、「応答」を[参照して](responsecode.md)ください。</span><span class="sxs-lookup"><span data-stu-id="dccc2-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="dccc2-139">次の例は、外部の Exchange コントロールパネル (ECP) が構成されていない場合に返されるエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="dccc2-140">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dccc2-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dccc2-141">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="dccc2-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="dccc2-142">MessageText</span><span class="sxs-lookup"><span data-stu-id="dccc2-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="dccc2-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dccc2-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dccc2-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dccc2-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="dccc2-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="dccc2-145">See also</span></span>

- [<span data-ttu-id="dccc2-146">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="dccc2-147">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="dccc2-148">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="dccc2-149">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="dccc2-150">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="dccc2-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

