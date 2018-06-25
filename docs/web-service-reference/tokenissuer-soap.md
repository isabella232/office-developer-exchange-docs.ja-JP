---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: TokenIssuer 要素は、セキュリティ トークン サービスの Uri (SOAP) または端点 (SOAP) を指定します。
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839708"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="626e9-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="626e9-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="626e9-104">**TokenIssuer**要素は、セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)または[端点 (SOAP)](endpoint-soap.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="626e9-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="626e9-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="626e9-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="626e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="626e9-106">Attributes and elements</span></span>

<span data-ttu-id="626e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="626e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="626e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="626e9-108">Attributes</span></span>

<span data-ttu-id="626e9-109">なし</span><span class="sxs-lookup"><span data-stu-id="626e9-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="626e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="626e9-110">Child elements</span></span>

|<span data-ttu-id="626e9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="626e9-111">**Element**</span></span>|<span data-ttu-id="626e9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="626e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="626e9-113">Uri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="626e9-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="626e9-114">セキュリティ トークンを発行したセキュリティ トークン サービスの URI。</span><span class="sxs-lookup"><span data-stu-id="626e9-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="626e9-115">エンドポイント (SOAP)</span><span class="sxs-lookup"><span data-stu-id="626e9-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="626e9-116">Web サービス エンドポイントの URI です。</span><span class="sxs-lookup"><span data-stu-id="626e9-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="626e9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="626e9-117">Parent elements</span></span>

|<span data-ttu-id="626e9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="626e9-118">**Element**</span></span>|<span data-ttu-id="626e9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="626e9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="626e9-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="626e9-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="626e9-121">[エンドポイント (SOAP)](endpoint-soap.md)セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="626e9-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="626e9-122">備考</span><span class="sxs-lookup"><span data-stu-id="626e9-122">Remarks</span></span>

<span data-ttu-id="626e9-123">**TokenIssuer**要素を使用して、セキュリティ トークンを使用する場合は、セキュリティ トークン サービスを指定します。</span><span class="sxs-lookup"><span data-stu-id="626e9-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="626e9-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="626e9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="626e9-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="626e9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="626e9-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="626e9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="626e9-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="626e9-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="626e9-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="626e9-128">Validation File</span></span>  <br/> |<span data-ttu-id="626e9-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="626e9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="626e9-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="626e9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="626e9-131">True</span><span class="sxs-lookup"><span data-stu-id="626e9-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="626e9-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="626e9-132">See also</span></span>



[<span data-ttu-id="626e9-133">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="626e9-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="626e9-134">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="626e9-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

