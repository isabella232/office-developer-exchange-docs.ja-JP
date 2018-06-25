---
title: POX の自動検出要求の交換
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: 自動検出要求には、ユーザーのクライアント アクセスの構成のクエリが含まれています。
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832865"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="e4f61-103">POX の自動検出要求の交換</span><span class="sxs-lookup"><span data-stu-id="e4f61-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="e4f61-104">自動検出要求には、ユーザーのクライアント アクセスの構成のクエリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4f61-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="e4f61-105">自動検出要求の例</span><span class="sxs-lookup"><span data-stu-id="e4f61-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="e4f61-106">説明</span><span class="sxs-lookup"><span data-stu-id="e4f61-106">Description</span></span>

<span data-ttu-id="e4f61-107">次の XML の例では、自動検出の要求の本体を示します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4f61-108">コード</span><span class="sxs-lookup"><span data-stu-id="e4f61-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="e4f61-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4f61-109">Request Headers</span></span>

<span data-ttu-id="e4f61-110">自動検出要求を送信するとき、次の HTTP ヘッダーはオプションです。</span><span class="sxs-lookup"><span data-stu-id="e4f61-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="e4f61-111">**表 1 です。HTTP 要求のヘッダー**</span><span class="sxs-lookup"><span data-stu-id="e4f61-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="e4f61-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="e4f61-112">**Header**</span></span>|<span data-ttu-id="e4f61-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4f61-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4f61-114">X MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="e4f61-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="e4f61-115">場合は存在し、設定を「1」に、クライアントが MAPI または HTTP プロトコルを使用してサーバーに接続するために使用する情報を要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="e4f61-116">このヘッダーは、MAPI または HTTP プロトコルを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="e4f61-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="e4f61-117">X ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="e4f61-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="e4f61-118">このヘッダーには、クライアントをサポートする機能のコンマ区切りのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4f61-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="e4f61-119">表 2 には、使用可能な値が指定されています。</span><span class="sxs-lookup"><span data-stu-id="e4f61-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="e4f61-120">**表 2 になります。X ClientCanHandle ヘッダー値**</span><span class="sxs-lookup"><span data-stu-id="e4f61-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="e4f61-121">**X ClientCanHandle の値 (大文字)**</span><span class="sxs-lookup"><span data-stu-id="e4f61-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="e4f61-122">**サーバーの最小バージョン**</span><span class="sxs-lookup"><span data-stu-id="e4f61-122">**Minimum server version**</span></span>|<span data-ttu-id="e4f61-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4f61-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e4f61-124">交渉</span><span class="sxs-lookup"><span data-stu-id="e4f61-124">Negotiate</span></span>  <br/> |<span data-ttu-id="e4f61-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="e4f61-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="e4f61-126">この値が存在する場合、サーバーは、サーバーは、ネゴシエート認証を受け付けるように構成されている場合[AuthPackage (POX)](authpackage-pox.md)の要素で"Negotiate"の値を返すは。</span><span class="sxs-lookup"><span data-stu-id="e4f61-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="e4f61-127">この値が存在しない場合は、サーバーでは、 **AuthPackage**要素では、"Negotiate"の値は返しません。</span><span class="sxs-lookup"><span data-stu-id="e4f61-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="e4f61-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="e4f61-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="e4f61-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="e4f61-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="e4f61-130">この値が存在する場合、サーバーはサーバーが RPC または HTTP 接続を受け付けるように構成されている場合は、"EXHTTP"に設定[の種類 (POX)](type-pox.md)要素を持つ[プロトコル (POX)](protocol-pox.md)の要素を返します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="e4f61-131">この値が存在しない場合は、サーバーには、"EXHTTP"に設定**の種類**の要素の**プロトコル**要素は返されません。</span><span class="sxs-lookup"><span data-stu-id="e4f61-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="e4f61-132">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-132">Request elements</span></span>

<span data-ttu-id="e4f61-133">次の要素は、要求の本体で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4f61-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="e4f61-134">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="e4f61-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="e4f61-135">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="e4f61-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="e4f61-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="e4f61-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="e4f61-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="e4f61-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="e4f61-138">[LegacyDN (POX)](legacydn-pox.md)要素は、 [EMailAddress (POX)](emailaddress-pox.md)要素の代わりに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e4f61-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="e4f61-139">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="e4f61-139">Version differences</span></span>

<span data-ttu-id="e4f61-140">X MapiHttpCapability ヘッダーは、Exchange Online では、Office 365 で利用可能なとオンプレミスから Exchange のバージョンが 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="e4f61-141">X ClientCanHandle ヘッダーは、Exchange Online では、Office 365 で利用可能なとオンプレミスから Exchange のバージョンが 15.00.0995.014 を構築します。</span><span class="sxs-lookup"><span data-stu-id="e4f61-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e4f61-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4f61-142">See also</span></span>



[<span data-ttu-id="e4f61-143">POX Exchange の自動検出の応答</span><span class="sxs-lookup"><span data-stu-id="e4f61-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="e4f61-144">Exchange の POX の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e4f61-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="e4f61-145">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4f61-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

