---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: TokenIssuer 要素は、security token service の Uri (SOAP) とエンドポイント (SOAP) を指定します。
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526327"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="5d16a-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d16a-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="5d16a-104">**Tokenissuer**要素は、security token Service の[Uri (Soap)](uri-soap.md)と[エンドポイント (soap)](endpoint-soap.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d16a-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="5d16a-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="5d16a-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d16a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5d16a-106">Attributes and elements</span></span>

<span data-ttu-id="5d16a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d16a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d16a-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d16a-108">Attributes</span></span>

<span data-ttu-id="5d16a-109">なし</span><span class="sxs-lookup"><span data-stu-id="5d16a-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d16a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d16a-110">Child elements</span></span>

|<span data-ttu-id="5d16a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5d16a-111">**Element**</span></span>|<span data-ttu-id="5d16a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d16a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d16a-113">Uri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d16a-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="5d16a-114">セキュリティトークンを発行したセキュリティトークンサービスの URI。</span><span class="sxs-lookup"><span data-stu-id="5d16a-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="5d16a-115">エンドポイント (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d16a-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="5d16a-116">Web サービスエンドポイント URI。</span><span class="sxs-lookup"><span data-stu-id="5d16a-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d16a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5d16a-117">Parent elements</span></span>

|<span data-ttu-id="5d16a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d16a-118">**Element**</span></span>|<span data-ttu-id="5d16a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d16a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d16a-120">TokenIssuers 者 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d16a-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="5d16a-121">セキュリティトークンサービス[Uri (soap)](uri-soap.md)と[エンドポイント (soap)](endpoint-soap.md)のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5d16a-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d16a-122">注釈</span><span class="sxs-lookup"><span data-stu-id="5d16a-122">Remarks</span></span>

<span data-ttu-id="5d16a-123">**Tokenissuer**要素を使用して、セキュリティトークンを使用するときにセキュリティトークンサービスを指定します。</span><span class="sxs-lookup"><span data-stu-id="5d16a-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5d16a-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5d16a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d16a-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d16a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5d16a-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d16a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5d16a-127">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d16a-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5d16a-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d16a-128">Validation File</span></span>  <br/> |<span data-ttu-id="5d16a-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5d16a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d16a-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d16a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d16a-131">正しい</span><span class="sxs-lookup"><span data-stu-id="5d16a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d16a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d16a-132">See also</span></span>



[<span data-ttu-id="5d16a-133">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="5d16a-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="5d16a-134">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d16a-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

