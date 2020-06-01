---
title: GetAppManifests 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: GetAppManifests EWS 操作に関する情報を検索します。
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463007"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="bf911-103">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-103">GetAppManifests operation</span></span>

<span data-ttu-id="bf911-104">**Getappmanifests** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="bf911-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="bf911-105">**Getappmanifests**操作は、アプリマニフェストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf911-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="bf911-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bf911-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="bf911-107">GetAppManifests 操作の使用</span><span class="sxs-lookup"><span data-stu-id="bf911-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="bf911-108">**Getappmanifests**操作は、メールボックスのアプリマニフェストを要求するための引数を受け取りません。</span><span class="sxs-lookup"><span data-stu-id="bf911-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="bf911-109">応答には、メールボックスにインストールされているアプリごとに、base64 でエンコードされた XML マニフェストファイルが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bf911-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="bf911-110">GetAppManifests 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf911-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="bf911-111">**Getappmanifests**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf911-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bf911-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="bf911-112">**Header name**</span></span>|<span data-ttu-id="bf911-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bf911-113">**Element**</span></span>|<span data-ttu-id="bf911-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf911-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bf911-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="bf911-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bf911-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="bf911-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bf911-117">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bf911-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bf911-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="bf911-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bf911-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="bf911-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bf911-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bf911-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bf911-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bf911-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bf911-122">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="bf911-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="bf911-123">GetAppManifests 操作要求の例: メールボックスのアプリマニフェストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf911-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="bf911-124">次の**Getappmanifests**操作要求の例は、メールボックスのアプリマニフェストを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bf911-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="bf911-125">[Apiversionsupported](apiversionsupported.md)要素と[SchemaVersionSupported](schemaversionsupported.md)要素は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="bf911-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bf911-126">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf911-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="bf911-127">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="bf911-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="bf911-128">サポートされている apiversion</span><span class="sxs-lookup"><span data-stu-id="bf911-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="bf911-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="bf911-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="bf911-130">成功した GetAppManifests 操作の応答</span><span class="sxs-lookup"><span data-stu-id="bf911-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="bf911-131">次の例は、 **Getappmanifests**操作要求に対する正常な応答を示しています。メールボックスのアプリマニフェストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf911-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bf911-132">読みやすくするために、すべての base64 アプリのマニフェストは任意に切り捨てられています。</span><span class="sxs-lookup"><span data-stu-id="bf911-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="bf911-133">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf911-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bf911-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="bf911-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="bf911-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf911-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bf911-136">アプリ</span><span class="sxs-lookup"><span data-stu-id="bf911-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="bf911-137">App</span><span class="sxs-lookup"><span data-stu-id="bf911-137">App</span></span>](app.md)
    
- [<span data-ttu-id="bf911-138">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="bf911-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="bf911-139">応答 SOAP 本文には、次の要素も含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bf911-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="bf911-140">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="bf911-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="bf911-141">GetAppManifests 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="bf911-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="bf911-142">この操作によって返されるエラーは、入力パラメーターの無効な形式に関連するか、または一般的な EWS エラーです。</span><span class="sxs-lookup"><span data-stu-id="bf911-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="bf911-143">EWS で汎用的で、この操作に固有のエラーコードについては、「応答」を[参照して](responsecode.md)ください。</span><span class="sxs-lookup"><span data-stu-id="bf911-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="bf911-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="bf911-144">See also</span></span>

- [<span data-ttu-id="bf911-145">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bf911-146">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="bf911-147">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="bf911-148">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="bf911-149">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="bf911-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

