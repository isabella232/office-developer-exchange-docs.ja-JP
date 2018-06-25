---
title: DisableApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: 操作 DisableApp EWS についての情報を検索します。
ms.openlocfilehash: be9e124d7464012ffa797a69192893d85804a004
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760056"
---
# <a name="disableapp-operation"></a><span data-ttu-id="9dc03-103">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="9dc03-103">DisableApp operation</span></span>

<span data-ttu-id="9dc03-104">**DisableApp** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-104">Find information about the **DisableApp** EWS operation.</span></span> 
  
<span data-ttu-id="9dc03-105">**DisableApp**操作は、Outlook 用メール アプリを無効にします。</span><span class="sxs-lookup"><span data-stu-id="9dc03-105">The **DisableApp** operation disables a mail app for Outlook.</span></span> 
  
<span data-ttu-id="9dc03-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9dc03-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-disableapp-operation"></a><span data-ttu-id="9dc03-107">DisableApp 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-107">Using the DisableApp operation</span></span>

<span data-ttu-id="9dc03-108">**DisableApp**操作は、要求を無効にするメール アプリケーションを識別して無効にされた理由のための 2 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="9dc03-108">The **DisableApp** operation takes two arguments in the request that identify the mail app to disable and the reason why it was disabled.</span></span> 
  
### <a name="disableapp-operation-soap-headers"></a><span data-ttu-id="9dc03-109">DisableApp 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9dc03-109">DisableApp operation SOAP headers</span></span>

<span data-ttu-id="9dc03-110">**DisableApp**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9dc03-110">The **DisableApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="9dc03-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="9dc03-111">**Header name**</span></span>|<span data-ttu-id="9dc03-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="9dc03-112">**Element**</span></span>|<span data-ttu-id="9dc03-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="9dc03-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9dc03-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="9dc03-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="9dc03-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="9dc03-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="9dc03-116">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="9dc03-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9dc03-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9dc03-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="9dc03-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="9dc03-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9dc03-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="9dc03-120">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="9dc03-121">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9dc03-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a><span data-ttu-id="9dc03-122">DisableApp 操作の要求の例: メールボックスにインストールされているメールのアプリケーションを無効にします。</span><span class="sxs-lookup"><span data-stu-id="9dc03-122">DisableApp operation request example: Disable a mail app installed in a mailbox</span></span>

<span data-ttu-id="9dc03-123">**DisableApp**操作の次の使用例がどのように表示を要求するメール アプリケーションを無効にします。</span><span class="sxs-lookup"><span data-stu-id="9dc03-123">The following example of a **DisableApp** operation request shows how to a disable a mail app.</span></span> <span data-ttu-id="9dc03-124">アプリケーション識別子は、 [GetAppManifests 操作](getappmanifests-operation.md)の応答で返される、アプリケーション マニフェストを参照しています。</span><span class="sxs-lookup"><span data-stu-id="9dc03-124">The app identifier can be found in the app manifest that is returned in a [GetAppManifests operation](getappmanifests-operation.md) response.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9dc03-125">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9dc03-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9dc03-126">DisableApp</span><span class="sxs-lookup"><span data-stu-id="9dc03-126">DisableApp</span></span>](disableapp.md)
    
- [<span data-ttu-id="9dc03-127">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="9dc03-127">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="9dc03-128">DisableReason</span><span class="sxs-lookup"><span data-stu-id="9dc03-128">DisableReason</span></span>](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a><span data-ttu-id="9dc03-129">DisableApp 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="9dc03-129">Successful DisableApp operation response</span></span>

<span data-ttu-id="9dc03-130">次の例では、メール アプリケーションを無効にする**DisableApp**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-130">The following example shows a successful response to a **DisableApp** operation request to disable a mail app.</span></span> 
  
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
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9dc03-131">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9dc03-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9dc03-132">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="9dc03-132">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="9dc03-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9dc03-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a><span data-ttu-id="9dc03-134">DisableApp 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="9dc03-134">DisableApp operation error response</span></span>

<span data-ttu-id="9dc03-135">**DisableApp**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-135">The following example shows an error response to a **DisableApp** operation request.</span></span> <span data-ttu-id="9dc03-136">これは、メールボックス内にインストールされていないメール アプリケーションを無効にする要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="9dc03-136">This is a response to a request to disable a mail app that is not installed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9dc03-137">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9dc03-137">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9dc03-138">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="9dc03-138">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="9dc03-139">MessageText</span><span class="sxs-lookup"><span data-stu-id="9dc03-139">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9dc03-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9dc03-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9dc03-141">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9dc03-141">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="9dc03-142">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9dc03-142">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9dc03-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="9dc03-143">See also</span></span>

- [<span data-ttu-id="9dc03-144">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="9dc03-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="9dc03-145">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="9dc03-145">InstallApp operation</span></span>](installapp-operation.md)   
- [<span data-ttu-id="9dc03-146">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="9dc03-146">UninstallApp operation</span></span>](uninstallapp-operation.md)   
- [<span data-ttu-id="9dc03-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="9dc03-147">GetAppManifests</span></span>](getappmanifests.md)   
- [<span data-ttu-id="9dc03-148">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="9dc03-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)   
- [<span data-ttu-id="9dc03-149">Outlook アドイン</span><span class="sxs-lookup"><span data-stu-id="9dc03-149">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

