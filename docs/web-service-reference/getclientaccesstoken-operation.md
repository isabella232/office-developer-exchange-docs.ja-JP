---
title: GetClientAccessToken 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: 操作 GetClientAccessToken EWS についての情報を検索します。
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760655"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="ac5e4-103">GetClientAccessToken 操作</span><span class="sxs-lookup"><span data-stu-id="ac5e4-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="ac5e4-104">**GetClientAccessToken** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="ac5e4-105">**GetClientAccessToken**操作では、Outlook のメール アプリケーションにクライアントのアクセスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="ac5e4-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="ac5e4-107">GetClientAccessToken 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="ac5e4-108">**GetClientAccessToken**操作の要求は、2 つの必要な引数: アプリケーション、およびトークンの種類の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="ac5e4-109">[GetAppManifests 操作](getappmanifests-operation.md)を使用するアプリケーション id を要求します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="ac5e4-110">GetClientAccessToken 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac5e4-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="ac5e4-111">**GetClientAccessToken**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ac5e4-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="ac5e4-112">**Header name**</span></span>|<span data-ttu-id="ac5e4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac5e4-113">**Element**</span></span>|<span data-ttu-id="ac5e4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac5e4-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ac5e4-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ac5e4-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ac5e4-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ac5e4-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ac5e4-117">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ac5e4-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ac5e4-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ac5e4-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ac5e4-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ac5e4-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ac5e4-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ac5e4-122">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="ac5e4-123">GetClientAccessToken 操作の要求の例: 呼び出し元 id のトークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="ac5e4-124">**GetClientAccessToken**操作要求の次の例では、アプリケーションの呼び出し元 id のトークンを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="ac5e4-125">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ac5e4-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="ac5e4-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="ac5e4-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="ac5e4-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="ac5e4-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="ac5e4-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="ac5e4-129">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="ac5e4-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="ac5e4-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="ac5e4-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="ac5e4-131">GetClientAccessToken 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="ac5e4-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="ac5e4-132">次の例では、アプリケーションの呼び出し元 id のトークンを取得するのには、 **GetClientAccessToken**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ac5e4-133">この資料では、トークンの値は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="ac5e4-134">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ac5e4-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="ac5e4-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="ac5e4-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ac5e4-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ac5e4-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ac5e4-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="ac5e4-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ac5e4-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ac5e4-139">トークン (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="ac5e4-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="ac5e4-140">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="ac5e4-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="ac5e4-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="ac5e4-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="ac5e4-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="ac5e4-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="ac5e4-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="ac5e4-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="ac5e4-144">GetClientAccessToken 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="ac5e4-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="ac5e4-145">**GetClientAccessToken**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="ac5e4-146">これは、適切なアクセス許可のないトークン、拡張子コールバックを取得する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ac5e4-147">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ac5e4-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="ac5e4-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="ac5e4-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ac5e4-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ac5e4-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ac5e4-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="ac5e4-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="ac5e4-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ac5e4-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ac5e4-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ac5e4-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ac5e4-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="ac5e4-154">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac5e4-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ac5e4-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac5e4-155">See also</span></span>

- [<span data-ttu-id="ac5e4-156">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="ac5e4-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="ac5e4-157">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="ac5e4-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="ac5e4-158">Outlook アドイン</span><span class="sxs-lookup"><span data-stu-id="ac5e4-158">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

