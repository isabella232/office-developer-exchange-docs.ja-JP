---
title: InstallApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: 操作 InstallApp EWS についての情報を検索します。
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831951"
---
# <a name="installapp-operation"></a><span data-ttu-id="01cb0-103">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="01cb0-103">InstallApp operation</span></span>

<span data-ttu-id="01cb0-104">**InstallApp** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="01cb0-105">**InstallApp**操作は、Outlook のメールボックスでのメール アプリケーションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="01cb0-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="01cb0-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="01cb0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="01cb0-107">InstallApp 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-107">Using the InstallApp operation</span></span>

<span data-ttu-id="01cb0-108">**InstallApp**操作では、インストールするのには、メール アプリケーションを識別する 1 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="01cb0-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="01cb0-109">引数には、base64 でエンコードされたメール アプリケーションのマニフェストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="01cb0-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="01cb0-110">InstallApp 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01cb0-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="01cb0-111">**InstallApp**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="01cb0-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="01cb0-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="01cb0-112">**Header name**</span></span>|<span data-ttu-id="01cb0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="01cb0-113">**Element**</span></span>|<span data-ttu-id="01cb0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="01cb0-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="01cb0-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="01cb0-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="01cb0-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="01cb0-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="01cb0-117">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="01cb0-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="01cb0-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="01cb0-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="01cb0-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="01cb0-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="01cb0-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="01cb0-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="01cb0-122">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="01cb0-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="01cb0-123">InstallApp 操作の要求の例: メールボックスにメール アプリケーションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="01cb0-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="01cb0-124">**InstallApp**操作要求の次の例では、Outlook のメール アプリケーションをインストールする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="01cb0-125">[GetAppManifests 操作](getappmanifests-operation.md)を使用してアプリケーション マニフェストをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="01cb0-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="01cb0-126">Base64 でエンコードされたアプリケーション マニフェストは、読みやすさを保持するために任意には切り捨てられましたし、有効なマニフェストではありません。</span><span class="sxs-lookup"><span data-stu-id="01cb0-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="01cb0-127">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01cb0-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01cb0-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="01cb0-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="01cb0-129">Manifest</span><span class="sxs-lookup"><span data-stu-id="01cb0-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="01cb0-130">InstallApp 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="01cb0-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="01cb0-131">次の例では、メール アプリケーションをインストールするのには、 **InstallApp**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="01cb0-132">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01cb0-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01cb0-133">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="01cb0-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="01cb0-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01cb0-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="01cb0-135">InstallApp 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="01cb0-135">InstallApp operation error response</span></span>

<span data-ttu-id="01cb0-136">**InstallApp**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01cb0-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="01cb0-137">これは、無効なマニフェストが含まれている要求への応答です。</span><span class="sxs-lookup"><span data-stu-id="01cb0-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="01cb0-138">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01cb0-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01cb0-139">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="01cb0-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="01cb0-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="01cb0-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="01cb0-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01cb0-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="01cb0-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="01cb0-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="01cb0-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="01cb0-143">See also</span></span>

- [<span data-ttu-id="01cb0-144">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="01cb0-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="01cb0-145">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="01cb0-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="01cb0-146">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="01cb0-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="01cb0-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="01cb0-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="01cb0-148">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="01cb0-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

