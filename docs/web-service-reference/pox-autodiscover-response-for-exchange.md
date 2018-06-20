---
title: POX Exchange の自動検出の応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: 自動検出の応答には、Exchange Web サービス (EWS) でのバインドを確立するために使用する Url の一覧を含む自動検出の要求に対する応答が含まれています。
ms.openlocfilehash: d9f8a5cc86efaa4dceda7385164872ecc5409252
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832863"
---
# <a name="pox-autodiscover-response-for-exchange"></a><span data-ttu-id="1ae60-103">POX Exchange の自動検出の応答</span><span class="sxs-lookup"><span data-stu-id="1ae60-103">POX Autodiscover response for Exchange</span></span>

<span data-ttu-id="1ae60-104">自動検出の応答には、Exchange Web サービス (EWS) でのバインドを確立するために使用する Url の一覧を含む自動検出の要求に対する応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ae60-104">The Autodiscover response contains a response to an Autodiscover request that includes a list of URLs that are used to establish a binding with Exchange Web Services (EWS).</span></span>
  
## <a name="autodiscover-response-example"></a><span data-ttu-id="1ae60-105">自動検出応答の例</span><span class="sxs-lookup"><span data-stu-id="1ae60-105">Autodiscover response example</span></span>

### <a name="description"></a><span data-ttu-id="1ae60-106">説明</span><span class="sxs-lookup"><span data-stu-id="1ae60-106">Description</span></span>

<span data-ttu-id="1ae60-107">正常な自動検出応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ae60-107">The following example shows a successful Autodiscover response.</span></span>
  
### <a name="code"></a><span data-ttu-id="1ae60-108">コード</span><span class="sxs-lookup"><span data-stu-id="1ae60-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>First Last</DisplayName>
      <LegacyDN>/o=contoso/ou=First Administrative Group/cn=Recipients/cn=iuser885646</LegacyDN>
      <DeploymentId>644560b8-a1ce-429c-8ace-23395843f701</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>MBX-SERVER.mail.internal.contoso.com</Server>
        <ServerDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER</ServerDN>
        <ServerVersion>72008287</ServerVersion>
        <MdbDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER/cn=Microsoft Private MDB</MdbDN>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>Exchange.contoso.com</Server>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-01-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-02-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Basic">https://cas-04-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-05-server.mail.internal.contoso.com/owa</OWAUrl>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

### <a name="comments"></a><span data-ttu-id="1ae60-109">コメント</span><span class="sxs-lookup"><span data-stu-id="1ae60-109">Comments</span></span>

<span data-ttu-id="1ae60-110">Exchange Web サービスにバインドするには、 [ASUrl (POX)](asurl-pox.md)要素で指定された URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="1ae60-110">To bind to Exchange Web Services, use the URL identified by the [ASUrl (POX)](asurl-pox.md) element.</span></span> 
  
### <a name="response-element"></a><span data-ttu-id="1ae60-111">Response 要素</span><span class="sxs-lookup"><span data-stu-id="1ae60-111">Response Element</span></span>

<span data-ttu-id="1ae60-112">応答の本体では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ae60-112">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="1ae60-113">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="1ae60-113">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="1ae60-114">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-114">Response (POX)</span></span>](response-pox.md)
    
- [<span data-ttu-id="1ae60-115">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-115">User (POX)</span></span>](user-pox.md)
    
- [<span data-ttu-id="1ae60-116">DisplayName (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-116">DisplayName (POX)</span></span>](displayname-pox.md)
    
- [<span data-ttu-id="1ae60-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-117">LegacyDN (POX)</span></span>](legacydn-pox.md)
    
- [<span data-ttu-id="1ae60-118">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-118">DeploymentId (POX)</span></span>](deploymentid-pox.md)
    
- [<span data-ttu-id="1ae60-119">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-119">Account (POX)</span></span>](account-pox.md)
    
- [<span data-ttu-id="1ae60-120">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-120">AccountType (POX)</span></span>](accounttype-pox.md)
    
- [<span data-ttu-id="1ae60-121">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-121">Action (POX)</span></span>](action-pox.md)
    
- [<span data-ttu-id="1ae60-122">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-122">Protocol (POX)</span></span>](protocol-pox.md)
    
- [<span data-ttu-id="1ae60-123">(POX) の種類</span><span class="sxs-lookup"><span data-stu-id="1ae60-123">Type (POX)</span></span>](type-pox.md)
    
- [<span data-ttu-id="1ae60-124">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-124">Server (POX)</span></span>](server-pox.md)
    
- [<span data-ttu-id="1ae60-125">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-125">ServerDN (POX)</span></span>](serverdn-pox.md)
    
- [<span data-ttu-id="1ae60-126">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-126">ServerVersion (POX)</span></span>](serverversion-pox.md)
    
- [<span data-ttu-id="1ae60-127">MdbDN (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-127">MdbDN (POX)</span></span>](mdbdn-pox.md)
    
- [<span data-ttu-id="1ae60-128">ASUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-128">ASUrl (POX)</span></span>](asurl-pox.md)
    
- [<span data-ttu-id="1ae60-129">OOFUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-129">OOFUrl (POX)</span></span>](oofurl-pox.md)
    
- [<span data-ttu-id="1ae60-130">UMUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-130">UMUrl (POX)</span></span>](umurl-pox.md)
    
- [<span data-ttu-id="1ae60-131">OABUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-131">OABUrl (POX)</span></span>](oaburl-pox.md)
    
- [<span data-ttu-id="1ae60-132">内部 (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-132">Internal (POX)</span></span>](internal-pox.md)
    
- [<span data-ttu-id="1ae60-133">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-133">OWAUrl (POX)</span></span>](owaurl-pox.md)
    
## <a name="autodiscover-error-response-example"></a><span data-ttu-id="1ae60-134">自動検出エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="1ae60-134">Autodiscover Error response example</span></span>

### <a name="description"></a><span data-ttu-id="1ae60-135">説明</span><span class="sxs-lookup"><span data-stu-id="1ae60-135">Description</span></span>

<span data-ttu-id="1ae60-136">自動検出エラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ae60-136">The following example shows an Autodiscover error response.</span></span>
  
### <a name="code"></a><span data-ttu-id="1ae60-137">コード</span><span class="sxs-lookup"><span data-stu-id="1ae60-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a><span data-ttu-id="1ae60-138">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="1ae60-138">Error response element</span></span>

<span data-ttu-id="1ae60-139">応答の本体では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ae60-139">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="1ae60-140">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="1ae60-140">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="1ae60-141">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-141">Response (POX)</span></span>](response-pox.md)
    
- [<span data-ttu-id="1ae60-142">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-142">Error (POX)</span></span>](error-pox.md)
    
- [<span data-ttu-id="1ae60-143">エラー コード (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-143">ErrorCode (POX)</span></span>](errorcode-pox.md)
    
- [<span data-ttu-id="1ae60-144">メッセージ (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-144">Message (POX)</span></span>](message-pox.md)
    
- [<span data-ttu-id="1ae60-145">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="1ae60-145">DebugData (POX)</span></span>](debugdata-pox.md)
    
## <a name="see-also"></a><span data-ttu-id="1ae60-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ae60-146">See also</span></span>

- [<span data-ttu-id="1ae60-147">POX の自動検出要求の交換</span><span class="sxs-lookup"><span data-stu-id="1ae60-147">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
- [<span data-ttu-id="1ae60-148">Exchange の POX の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="1ae60-148">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md) 
- [<span data-ttu-id="1ae60-149">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ae60-149">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

