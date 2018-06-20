---
title: UninstallApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: 操作 UninstallApp EWS についての情報を検索します。
ms.openlocfilehash: 4f44224651993023336eef5540ec29b7f6a6e32e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839784"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="ff921-103">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="ff921-103">UninstallApp operation</span></span>

<span data-ttu-id="ff921-104">**UninstallApp** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="ff921-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="ff921-105">**UninstallApp**操作は、Outlook のメール アプリケーションをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="ff921-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="ff921-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ff921-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="ff921-107">UninstallApp 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="ff921-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="ff921-108">**UninstallApp**操作では、アンインストールするのにはメール アプリケーションを識別する要求の 1 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="ff921-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="ff921-109">UninstallApp 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff921-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="ff921-110">**UninstallApp**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff921-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ff921-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="ff921-111">**Header name**</span></span>|<span data-ttu-id="ff921-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff921-112">**Element**</span></span>|<span data-ttu-id="ff921-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff921-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ff921-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ff921-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ff921-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ff921-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ff921-116">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff921-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ff921-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff921-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ff921-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ff921-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ff921-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ff921-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ff921-120">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff921-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ff921-121">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff921-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="ff921-122">UninstallApp 操作の要求の例: メールボックス内のメール アプリケーションをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="ff921-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="ff921-123">**UninstallApp**操作の次の使用例がどのように表示を要求、アプリケーション識別子を使用して、メール アプリケーションをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="ff921-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="ff921-124">アプリケーション識別子は、 [GetAppManifests 操作](getappmanifests-operation.md)によって返される、アプリケーション マニフェストを参照しています。</span><span class="sxs-lookup"><span data-stu-id="ff921-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ff921-125">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff921-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff921-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="ff921-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="ff921-127">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="ff921-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="ff921-128">UninstallApp 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="ff921-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="ff921-129">次の例では、メール アプリケーションをアンインストールするのには、 **UninstallApp**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="ff921-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ff921-130">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff921-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff921-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="ff921-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="ff921-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ff921-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="ff921-133">UninstallApp 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="ff921-133">UninstallApp operation error response</span></span>

<span data-ttu-id="ff921-134">**UninstallApp**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff921-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="ff921-135">これは、既にアンインストールされているメール アプリケーションをアンインストールするための要求への応答です。</span><span class="sxs-lookup"><span data-stu-id="ff921-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ff921-136">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff921-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff921-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="ff921-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="ff921-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="ff921-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ff921-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ff921-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ff921-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ff921-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="ff921-141">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff921-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ff921-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff921-142">See also</span></span>

- [<span data-ttu-id="ff921-143">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="ff921-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="ff921-144">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="ff921-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="ff921-145">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="ff921-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="ff921-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="ff921-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="ff921-147">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="ff921-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

