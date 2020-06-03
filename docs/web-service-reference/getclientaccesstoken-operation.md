---
title: GetClientAccessToken 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: GetClientAccessToken EWS 操作についての情報を検索します。
ms.openlocfilehash: 2d49d675fcedb0e7e8312a9715f095c47fcf3d77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462039"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="c33ed-103">GetClientAccessToken 操作</span><span class="sxs-lookup"><span data-stu-id="c33ed-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="c33ed-104">**GetClientAccessToken** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="c33ed-105">**GetClientAccessToken**操作は、Outlook 用メールアプリのクライアントアクセストークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="c33ed-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c33ed-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="c33ed-107">GetClientAccessToken 操作の使用</span><span class="sxs-lookup"><span data-stu-id="c33ed-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="c33ed-108">**GetClientAccessToken**操作要求は、次の2つの必要な引数を受け取ります。アプリの識別子とトークンの種類。</span><span class="sxs-lookup"><span data-stu-id="c33ed-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="c33ed-109">[Getappmanifests 操作](getappmanifests-operation.md)を使用して、アプリ識別子を要求できます。</span><span class="sxs-lookup"><span data-stu-id="c33ed-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="c33ed-110">GetClientAccessToken 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c33ed-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="c33ed-111">**GetClientAccessToken**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c33ed-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c33ed-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="c33ed-112">**Header name**</span></span>|<span data-ttu-id="c33ed-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c33ed-113">**Element**</span></span>|<span data-ttu-id="c33ed-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c33ed-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c33ed-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c33ed-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c33ed-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c33ed-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c33ed-117">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c33ed-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c33ed-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c33ed-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c33ed-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c33ed-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c33ed-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c33ed-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c33ed-122">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c33ed-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="c33ed-123">GetClientAccessToken 操作要求の例: 発信者 id トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="c33ed-124">次の**GetClientAccessToken**操作要求の例は、アプリの発信者番号トークンを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="c33ed-125">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c33ed-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="c33ed-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="c33ed-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="c33ed-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="c33ed-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="c33ed-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="c33ed-129">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="c33ed-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="c33ed-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="c33ed-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="c33ed-131">成功した GetClientAccessToken 操作の応答</span><span class="sxs-lookup"><span data-stu-id="c33ed-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="c33ed-132">次の例は、 **GetClientAccessToken**操作要求に対する正常な応答を示しています。アプリの発信者番号トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="c33ed-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c33ed-133">この記事のトークンの値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="c33ed-134">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c33ed-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="c33ed-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="c33ed-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c33ed-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c33ed-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c33ed-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="c33ed-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c33ed-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c33ed-139">トークン (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="c33ed-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="c33ed-140">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="c33ed-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="c33ed-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="c33ed-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="c33ed-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="c33ed-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="c33ed-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="c33ed-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="c33ed-144">GetClientAccessToken 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="c33ed-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="c33ed-145">次の例は、 **GetClientAccessToken**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="c33ed-146">これは、適切なアクセス許可を持たない拡張コールバックトークンを取得する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="c33ed-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="c33ed-147">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c33ed-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c33ed-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="c33ed-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="c33ed-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c33ed-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c33ed-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c33ed-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="c33ed-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="c33ed-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c33ed-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c33ed-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c33ed-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c33ed-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="c33ed-154">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="c33ed-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c33ed-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="c33ed-155">See also</span></span>

- [<span data-ttu-id="c33ed-156">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="c33ed-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="c33ed-157">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="c33ed-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="c33ed-158">Outlook アドイン</span><span class="sxs-lookup"><span data-stu-id="c33ed-158">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

