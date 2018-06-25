---
title: GetAppMarketplaceUrl 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: 操作 GetAppMarketplaceUrl EWS についての情報を検索します。
ms.openlocfilehash: 616e7f571ba5283a773e51d611cd18bb37b5bc8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760631"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="d9d73-103">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="d9d73-104">**GetAppMarketplaceUrl** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="d9d73-105">**GetAppMarketplaceUrl**操作は、クライアントがメールボックスにインストールするアプリケーションを取得するためにアクセスしてアプリケーション市場の URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="d9d73-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d9d73-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="d9d73-107">GetAppMarketplaceUrl 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="d9d73-108">**GetAppMarketplaceUrl**操作には、クライアントがアプリケーションのインストール時に元となる市場の URL を要求するすべての引数になりません。</span><span class="sxs-lookup"><span data-stu-id="d9d73-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="d9d73-109">応答は、アプリケーション市場への URL が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9d73-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="d9d73-110">GetAppMarketplaceUrl 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9d73-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="d9d73-111">**GetAppMarketplaceUrl**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d9d73-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d9d73-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="d9d73-112">**Header name**</span></span>|<span data-ttu-id="d9d73-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9d73-113">**Element**</span></span>|<span data-ttu-id="d9d73-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9d73-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d9d73-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d9d73-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d9d73-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d9d73-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d9d73-117">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d9d73-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d9d73-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d9d73-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d9d73-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d9d73-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d9d73-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d9d73-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d9d73-122">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d9d73-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="d9d73-123">GetAppMarketplaceUrl 操作の要求の例: メールボックスのアプリケーション市場の URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="d9d73-124">**GetAppMarketplaceUrl**操作要求の次の例では、メールボックスのアプリケーション市場の URL を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="d9d73-125">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9d73-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d9d73-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d9d73-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="d9d73-127">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d9d73-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="d9d73-128">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d9d73-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="d9d73-129">GetAppMarketplaceUrl 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="d9d73-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="d9d73-130">**GetAppMarketplaceUrl**操作の要求、アプリケーション市場の URL を取得するメールボックスに正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d9d73-131">読みやすさを保持するためにアプリケーション市場の URL が変更されました。</span><span class="sxs-lookup"><span data-stu-id="d9d73-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="d9d73-132">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9d73-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d9d73-133">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="d9d73-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="d9d73-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d9d73-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d9d73-135">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d9d73-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="d9d73-136">GetAppMarketPlaceUrl 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="d9d73-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="d9d73-137">この操作で返されるエラーは、不適切なサービスの構成に関連するか、または EWS の一般的なエラーです。</span><span class="sxs-lookup"><span data-stu-id="d9d73-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="d9d73-138">EWS にジェネリックとこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9d73-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="d9d73-139">外部 Exchange コントロール パネル (ECP) が構成されていない場合に返されるエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9d73-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d9d73-140">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9d73-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d9d73-141">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="d9d73-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="d9d73-142">MessageText</span><span class="sxs-lookup"><span data-stu-id="d9d73-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d9d73-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d9d73-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d9d73-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d9d73-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d9d73-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9d73-145">See also</span></span>

- [<span data-ttu-id="d9d73-146">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d9d73-147">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="d9d73-148">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="d9d73-149">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="d9d73-150">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="d9d73-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

