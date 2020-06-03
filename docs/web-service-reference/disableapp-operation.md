---
title: DisableApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: DisableApp EWS 操作に関する情報を検索します。
ms.openlocfilehash: 8e1f3a257a70c042a01ed70da97cfa0573a2d454
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462067"
---
# <a name="disableapp-operation"></a><span data-ttu-id="5d22a-103">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="5d22a-103">DisableApp operation</span></span>

<span data-ttu-id="5d22a-104">**Disableapp** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="5d22a-104">Find information about the **DisableApp** EWS operation.</span></span> 
  
<span data-ttu-id="5d22a-105">**Disableapp**操作は、Outlook 用のメールアプリを無効にします。</span><span class="sxs-lookup"><span data-stu-id="5d22a-105">The **DisableApp** operation disables a mail app for Outlook.</span></span> 
  
<span data-ttu-id="5d22a-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5d22a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-disableapp-operation"></a><span data-ttu-id="5d22a-107">DisableApp 操作の使用</span><span class="sxs-lookup"><span data-stu-id="5d22a-107">Using the DisableApp operation</span></span>

<span data-ttu-id="5d22a-108">**Disableapp**操作は、要求で2つの引数を受け取り、無効にするメールアプリと、無効にされた理由を識別します。</span><span class="sxs-lookup"><span data-stu-id="5d22a-108">The **DisableApp** operation takes two arguments in the request that identify the mail app to disable and the reason why it was disabled.</span></span> 
  
### <a name="disableapp-operation-soap-headers"></a><span data-ttu-id="5d22a-109">DisableApp operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d22a-109">DisableApp operation SOAP headers</span></span>

<span data-ttu-id="5d22a-110">**Disableapp**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5d22a-110">The **DisableApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5d22a-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="5d22a-111">**Header name**</span></span>|<span data-ttu-id="5d22a-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d22a-112">**Element**</span></span>|<span data-ttu-id="5d22a-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d22a-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5d22a-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5d22a-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5d22a-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5d22a-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5d22a-116">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5d22a-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5d22a-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5d22a-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5d22a-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5d22a-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5d22a-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5d22a-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5d22a-120">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5d22a-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5d22a-121">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5d22a-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a><span data-ttu-id="5d22a-122">DisableApp 操作要求の例: メールボックスにインストールされたメールアプリを無効にする</span><span class="sxs-lookup"><span data-stu-id="5d22a-122">DisableApp operation request example: Disable a mail app installed in a mailbox</span></span>

<span data-ttu-id="5d22a-123">次の**Disableapp** operation 要求の例は、メールアプリを無効にする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-123">The following example of a **DisableApp** operation request shows how to a disable a mail app.</span></span> <span data-ttu-id="5d22a-124">アプリ識別子は、 [Getappmanifests 操作](getappmanifests-operation.md)の応答で返されるアプリマニフェストにあります。</span><span class="sxs-lookup"><span data-stu-id="5d22a-124">The app identifier can be found in the app manifest that is returned in a [GetAppManifests operation](getappmanifests-operation.md) response.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="5d22a-125">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d22a-126">DisableApp</span><span class="sxs-lookup"><span data-stu-id="5d22a-126">DisableApp</span></span>](disableapp.md)
    
- [<span data-ttu-id="5d22a-127">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="5d22a-127">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="5d22a-128">DisableReason</span><span class="sxs-lookup"><span data-stu-id="5d22a-128">DisableReason</span></span>](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a><span data-ttu-id="5d22a-129">正常な DisableApp 操作応答</span><span class="sxs-lookup"><span data-stu-id="5d22a-129">Successful DisableApp operation response</span></span>

<span data-ttu-id="5d22a-130">次の例は、メールアプリを無効にするための**Disableapp**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-130">The following example shows a successful response to a **DisableApp** operation request to disable a mail app.</span></span> 
  
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
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5d22a-131">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d22a-132">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="5d22a-132">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="5d22a-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5d22a-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a><span data-ttu-id="5d22a-134">DisableApp 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="5d22a-134">DisableApp operation error response</span></span>

<span data-ttu-id="5d22a-135">次の例は、 **Disableapp**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-135">The following example shows an error response to a **DisableApp** operation request.</span></span> <span data-ttu-id="5d22a-136">これは、メールボックスにインストールされていないメールアプリを無効にする要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="5d22a-136">This is a response to a request to disable a mail app that is not installed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5d22a-137">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d22a-137">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d22a-138">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="5d22a-138">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="5d22a-139">MessageText</span><span class="sxs-lookup"><span data-stu-id="5d22a-139">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5d22a-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5d22a-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5d22a-141">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5d22a-141">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="5d22a-142">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="5d22a-142">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5d22a-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d22a-143">See also</span></span>

- [<span data-ttu-id="5d22a-144">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="5d22a-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="5d22a-145">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="5d22a-145">InstallApp operation</span></span>](installapp-operation.md)   
- [<span data-ttu-id="5d22a-146">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="5d22a-146">UninstallApp operation</span></span>](uninstallapp-operation.md)   
- [<span data-ttu-id="5d22a-147">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="5d22a-147">GetAppManifests</span></span>](getappmanifests.md)   
- [<span data-ttu-id="5d22a-148">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="5d22a-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)   
- [<span data-ttu-id="5d22a-149">Outlook アドイン</span><span class="sxs-lookup"><span data-stu-id="5d22a-149">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

