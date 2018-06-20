---
title: GetAppManifests 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: 操作 GetAppManifests EWS についての情報を検索します。
ms.openlocfilehash: 9c919bac9ac0042890d1c439454b37e6b7c60876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760625"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="d728f-103">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="d728f-103">GetAppManifests operation</span></span>

<span data-ttu-id="d728f-104">**GetAppManifests** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d728f-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="d728f-105">**GetAppManifests**操作は、アプリケーション マニフェストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d728f-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="d728f-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d728f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="d728f-107">GetAppManifests 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="d728f-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="d728f-108">**GetAppManifests**操作には、メールボックスのアプリケーション マニフェストを要求するすべての引数になりません。</span><span class="sxs-lookup"><span data-stu-id="d728f-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="d728f-109">Base64 でエンコードされた XML マニフェスト ファイル、メールボックスにインストールされている各アプリケーションの応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d728f-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="d728f-110">GetAppManifests 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d728f-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="d728f-111">**GetAppManifests**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d728f-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d728f-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="d728f-112">**Header name**</span></span>|<span data-ttu-id="d728f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d728f-113">**Element**</span></span>|<span data-ttu-id="d728f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d728f-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d728f-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d728f-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d728f-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d728f-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d728f-117">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d728f-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d728f-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d728f-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d728f-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d728f-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d728f-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d728f-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d728f-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d728f-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d728f-122">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d728f-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="d728f-123">GetAppManifests 操作の要求の例: メールボックスのアプリケーション マニフェストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d728f-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="d728f-124">**GetAppManifests**操作要求の次の使用例では、メールボックスのアプリケーション マニフェストを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d728f-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="d728f-125">[ApiVersionSupported](apiversionsupported.md)要素と、 [SchemaVersionSupported](schemaversionsupported.md)はオプションです。</span><span class="sxs-lookup"><span data-stu-id="d728f-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="d728f-126">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d728f-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="d728f-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d728f-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="d728f-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d728f-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="d728f-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d728f-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="d728f-130">GetAppManifests 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="d728f-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="d728f-131">メールボックスのアプリケーション マニフェストを取得する**GetAppManifests**操作要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d728f-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d728f-132">すべて base64 形式のアプリケーション マニフェストは、読みやすさを保持するために任意に切り捨てられました。</span><span class="sxs-lookup"><span data-stu-id="d728f-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d728f-133">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d728f-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d728f-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="d728f-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="d728f-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d728f-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d728f-136">アプリ</span><span class="sxs-lookup"><span data-stu-id="d728f-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="d728f-137">App</span><span class="sxs-lookup"><span data-stu-id="d728f-137">App</span></span>](app.md)
    
- [<span data-ttu-id="d728f-138">Manifest</span><span class="sxs-lookup"><span data-stu-id="d728f-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="d728f-139">応答 SOAP 本文には、次の要素を含めることも。</span><span class="sxs-lookup"><span data-stu-id="d728f-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="d728f-140">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="d728f-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="d728f-141">GetAppManifests 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="d728f-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="d728f-142">この操作で返されるエラーは無効な形式の入力パラメーターに関連付けられているまたは EWS の一般的なエラーです。</span><span class="sxs-lookup"><span data-stu-id="d728f-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="d728f-143">EWS にジェネリックとこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d728f-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="d728f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="d728f-144">See also</span></span>

- [<span data-ttu-id="d728f-145">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="d728f-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d728f-146">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="d728f-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="d728f-147">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="d728f-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="d728f-148">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="d728f-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="d728f-149">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="d728f-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

