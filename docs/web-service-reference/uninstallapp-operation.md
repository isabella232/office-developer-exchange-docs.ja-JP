---
title: アン Installapp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: アン Installapp EWS 操作に関する情報を検索します。
ms.openlocfilehash: 27931636ee13a251fb03fe804987d7b01a325230
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467152"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="39e90-103">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="39e90-103">UninstallApp operation</span></span>

<span data-ttu-id="39e90-104">**アン Installapp** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="39e90-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="39e90-105">**アン installapp**操作は、Outlook 用のメールアプリをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="39e90-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="39e90-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="39e90-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="39e90-107">アン Installapp 操作の使用</span><span class="sxs-lookup"><span data-stu-id="39e90-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="39e90-108">**アン Installapp**操作は、アンインストールするメールアプリを識別する要求で1つの引数を取ります。</span><span class="sxs-lookup"><span data-stu-id="39e90-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="39e90-109">アン Installapp operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39e90-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="39e90-110">**アン Installapp**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="39e90-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="39e90-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="39e90-111">**Header name**</span></span>|<span data-ttu-id="39e90-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="39e90-112">**Element**</span></span>|<span data-ttu-id="39e90-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="39e90-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="39e90-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="39e90-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="39e90-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="39e90-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="39e90-116">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="39e90-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="39e90-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="39e90-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="39e90-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="39e90-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="39e90-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="39e90-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="39e90-120">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="39e90-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="39e90-121">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="39e90-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="39e90-122">アン Installapp 操作要求の例: メールボックス内のメールアプリをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="39e90-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="39e90-123">次の例の例では **、アプリ識別子**を使用してメールアプリをアンインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="39e90-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="39e90-124">アプリ識別子は、 [Getappmanifests 操作](getappmanifests-operation.md)によって返されるアプリマニフェストに含まれています。</span><span class="sxs-lookup"><span data-stu-id="39e90-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="39e90-125">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39e90-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="39e90-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="39e90-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="39e90-127">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="39e90-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="39e90-128">成功した Installapp 操作の応答</span><span class="sxs-lookup"><span data-stu-id="39e90-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="39e90-129">次の例は、メールアプリをアンインストールするための、**アン Installapp**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="39e90-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="39e90-130">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39e90-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="39e90-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="39e90-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="39e90-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="39e90-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="39e90-133">アン Installapp 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="39e90-133">UninstallApp operation error response</span></span>

<span data-ttu-id="39e90-134">次の例は、**アン Installapp**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="39e90-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="39e90-135">これは、既にアンインストールされているメールアプリをアンインストールする要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="39e90-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="39e90-136">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39e90-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="39e90-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="39e90-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="39e90-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="39e90-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="39e90-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="39e90-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="39e90-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="39e90-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="39e90-141">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="39e90-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="39e90-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="39e90-142">See also</span></span>

- [<span data-ttu-id="39e90-143">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="39e90-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="39e90-144">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="39e90-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="39e90-145">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="39e90-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="39e90-146">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="39e90-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="39e90-147">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="39e90-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

