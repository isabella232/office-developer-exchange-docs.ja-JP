---
title: POX Exchange の自動検出要求
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: 自動検出要求には、ユーザーのクライアントアクセス構成に対するクエリが含まれています。
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461668"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="26f02-103">POX Exchange の自動検出要求</span><span class="sxs-lookup"><span data-stu-id="26f02-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="26f02-104">自動検出要求には、ユーザーのクライアントアクセス構成に対するクエリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="26f02-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="26f02-105">自動検出要求の例</span><span class="sxs-lookup"><span data-stu-id="26f02-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="26f02-106">Description</span><span class="sxs-lookup"><span data-stu-id="26f02-106">Description</span></span>

<span data-ttu-id="26f02-107">次の XML の例は、自動検出要求本文を示しています。</span><span class="sxs-lookup"><span data-stu-id="26f02-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="26f02-108">コード</span><span class="sxs-lookup"><span data-stu-id="26f02-108">Code</span></span>

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="26f02-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26f02-109">Request Headers</span></span>

<span data-ttu-id="26f02-110">次の HTTP ヘッダーは、自動検出要求を送信するときにオプションです。</span><span class="sxs-lookup"><span data-stu-id="26f02-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="26f02-111">**表1HTTP 要求ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="26f02-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="26f02-112">**ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="26f02-112">**Header**</span></span>|<span data-ttu-id="26f02-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="26f02-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="26f02-114">MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="26f02-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="26f02-115">"1" に設定されている場合は、MAPI/HTTP プロトコルを使用してサーバーへの接続に使用できる情報をクライアントが要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="26f02-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="26f02-116">このヘッダーは、MAPI/HTTP プロトコルを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="26f02-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="26f02-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="26f02-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="26f02-118">このヘッダーには、クライアントがサポートする機能のコンマ区切りリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="26f02-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="26f02-119">使用可能な値は表2で指定されています。</span><span class="sxs-lookup"><span data-stu-id="26f02-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="26f02-120">**表2X-ClientCanHandle ヘッダー値**</span><span class="sxs-lookup"><span data-stu-id="26f02-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="26f02-121">**X-ClientCanHandle 値 (大文字と小文字を区別しない)**</span><span class="sxs-lookup"><span data-stu-id="26f02-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="26f02-122">**最小サーバーバージョン**</span><span class="sxs-lookup"><span data-stu-id="26f02-122">**Minimum server version**</span></span>|<span data-ttu-id="26f02-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="26f02-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="26f02-124">取り決め</span><span class="sxs-lookup"><span data-stu-id="26f02-124">Negotiate</span></span>  <br/> |<span data-ttu-id="26f02-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="26f02-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="26f02-126">この値が存在する場合、サーバーがネゴシエート認証を受け入れるように構成されている場合、サーバーは[Authpackage (POX)](authpackage-pox.md)要素で値 "Negotiate" を返します。</span><span class="sxs-lookup"><span data-stu-id="26f02-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="26f02-127">この値が指定されていない場合、サーバーは**Authpackage**要素に "Negotiate" という値を返しません。</span><span class="sxs-lookup"><span data-stu-id="26f02-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="26f02-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="26f02-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="26f02-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="26f02-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="26f02-130">この値が存在する場合、サーバーは RPC/HTTP 接続を受け入れるように構成されている場合は、 [Type (POX)](type-pox.md)要素が "exhttp" に設定された[プロトコル (POX)](protocol-pox.md)要素を返します。</span><span class="sxs-lookup"><span data-stu-id="26f02-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="26f02-131">この値が指定されていない場合、サーバーは**Type**要素が "exhttp" に設定されている**Protocol**要素を返しません。</span><span class="sxs-lookup"><span data-stu-id="26f02-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="26f02-132">Request 要素</span><span class="sxs-lookup"><span data-stu-id="26f02-132">Request elements</span></span>

<span data-ttu-id="26f02-133">要求本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="26f02-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="26f02-134">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="26f02-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="26f02-135">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="26f02-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="26f02-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="26f02-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="26f02-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="26f02-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="26f02-138">[LegacyDN (POX)](legacydn-pox.md)要素は、 [EMailAddress (POX)](emailaddress-pox.md)要素の代わりに使用できます。</span><span class="sxs-lookup"><span data-stu-id="26f02-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="26f02-139">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="26f02-139">Version differences</span></span>

<span data-ttu-id="26f02-140">MapiHttpCapability ヘッダーは、Office 365、Exchange Online、およびオンプレミスバージョンの Exchange (build 15.00.0847.032 (Exchange Server 2013 SP1) 以降で利用できます。</span><span class="sxs-lookup"><span data-stu-id="26f02-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="26f02-141">X-ClientCanHandle ヘッダーは、Office 365、Exchange Online、およびオンプレミスバージョンの Exchange で使用できます。これは、build 15.00.0995.014 から始まります。</span><span class="sxs-lookup"><span data-stu-id="26f02-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="26f02-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="26f02-142">See also</span></span>



[<span data-ttu-id="26f02-143">POX Exchange の自動検出応答</span><span class="sxs-lookup"><span data-stu-id="26f02-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="26f02-144">Exchange 用 POX 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="26f02-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="26f02-145">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="26f02-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

