---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: TokenIssuers 要素は、TokenIssuer (SOAP) のコレクションを表します。
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839720"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="e28fd-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e28fd-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="e28fd-104">**TokenIssuers**要素は、 [TokenIssuer (SOAP)](tokenissuer-soap.md)のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e28fd-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="e28fd-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="e28fd-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e28fd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e28fd-106">Attributes and elements</span></span>

<span data-ttu-id="e28fd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e28fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e28fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="e28fd-108">Attributes</span></span>

<span data-ttu-id="e28fd-109">なし</span><span class="sxs-lookup"><span data-stu-id="e28fd-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e28fd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e28fd-110">Child elements</span></span>

|<span data-ttu-id="e28fd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e28fd-111">**Element**</span></span>|<span data-ttu-id="e28fd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e28fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e28fd-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e28fd-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="e28fd-114">セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)または[端点 (SOAP)](endpoint-soap.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="e28fd-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e28fd-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e28fd-115">Parent elements</span></span>

|<span data-ttu-id="e28fd-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e28fd-116">**Element**</span></span>|<span data-ttu-id="e28fd-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e28fd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e28fd-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e28fd-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="e28fd-119">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e28fd-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e28fd-120">備考</span><span class="sxs-lookup"><span data-stu-id="e28fd-120">Remarks</span></span>

<span data-ttu-id="e28fd-121">**TokenIssuers**は、自動検出で使用される[TokenIssuer (SOAP)](tokenissuer-soap.md)要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e28fd-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e28fd-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e28fd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e28fd-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e28fd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e28fd-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e28fd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e28fd-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e28fd-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e28fd-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e28fd-126">Validation File</span></span>  <br/> |<span data-ttu-id="e28fd-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e28fd-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e28fd-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e28fd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e28fd-129">True</span><span class="sxs-lookup"><span data-stu-id="e28fd-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e28fd-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e28fd-130">See also</span></span>



[<span data-ttu-id="e28fd-131">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e28fd-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="e28fd-132">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="e28fd-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

