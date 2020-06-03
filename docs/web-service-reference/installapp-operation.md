---
title: InstallApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: InstallApp EWS 操作に関する情報を検索します。
ms.openlocfilehash: ae6aab7f7176aa827bafa9abf1aa67d458d309d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465689"
---
# <a name="installapp-operation"></a><span data-ttu-id="5978b-103">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="5978b-103">InstallApp operation</span></span>

<span data-ttu-id="5978b-104">**Installapp** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="5978b-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="5978b-105">**Installapp**操作は、メールボックスに Outlook 用のメールアプリをインストールします。</span><span class="sxs-lookup"><span data-stu-id="5978b-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="5978b-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5978b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="5978b-107">InstallApp 操作の使用</span><span class="sxs-lookup"><span data-stu-id="5978b-107">Using the InstallApp operation</span></span>

<span data-ttu-id="5978b-108">**Installapp**操作は、インストールするメールアプリを識別する1つの引数を取ります。</span><span class="sxs-lookup"><span data-stu-id="5978b-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="5978b-109">引数には、メールアプリ用の base64 でエンコードされたマニフェストを指定します。</span><span class="sxs-lookup"><span data-stu-id="5978b-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="5978b-110">InstallApp operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5978b-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="5978b-111">**Installapp**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5978b-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5978b-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="5978b-112">**Header name**</span></span>|<span data-ttu-id="5978b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5978b-113">**Element**</span></span>|<span data-ttu-id="5978b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5978b-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5978b-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5978b-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5978b-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5978b-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5978b-117">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5978b-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5978b-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5978b-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5978b-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5978b-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5978b-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5978b-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5978b-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5978b-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5978b-122">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5978b-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="5978b-123">InstallApp 操作要求の例: メールアプリをメールボックスにインストールする</span><span class="sxs-lookup"><span data-stu-id="5978b-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="5978b-124">次の**Installapp**操作要求の例は、Outlook 用メールアプリをインストールする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5978b-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="5978b-125">アプリマニフェストは、 [Getappmanifests 操作](getappmanifests-operation.md)を使用して見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="5978b-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="5978b-126">Base64 でエンコードされたアプリマニフェストは読みやすさを維持するために任意に切り捨てられ、有効なマニフェストを表すものではありません。</span><span class="sxs-lookup"><span data-stu-id="5978b-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="5978b-127">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5978b-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5978b-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="5978b-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="5978b-129">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="5978b-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="5978b-130">正常な InstallApp 操作の応答</span><span class="sxs-lookup"><span data-stu-id="5978b-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="5978b-131">次の例は、メールアプリをインストールするための**Installapp**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5978b-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
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
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5978b-132">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5978b-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5978b-133">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="5978b-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="5978b-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5978b-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="5978b-135">InstallApp 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="5978b-135">InstallApp operation error response</span></span>

<span data-ttu-id="5978b-136">次の例は、 **Installapp**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5978b-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="5978b-137">これは、無効なマニフェストを含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="5978b-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
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
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="5978b-138">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5978b-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5978b-139">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="5978b-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="5978b-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="5978b-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5978b-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5978b-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5978b-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5978b-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="5978b-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="5978b-143">See also</span></span>

- [<span data-ttu-id="5978b-144">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="5978b-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5978b-145">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="5978b-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="5978b-146">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="5978b-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="5978b-147">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="5978b-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="5978b-148">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="5978b-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

