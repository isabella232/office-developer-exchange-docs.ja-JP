---
title: TokenIssuers 者 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Tokenissuers 要素は、Tokenissuers (SOAP) コレクションを表します。
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457075"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="7578c-103">TokenIssuers 者 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7578c-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="7578c-104">**Tokenissuers**要素は、 [TOKENISSUERS (SOAP)](tokenissuer-soap.md)コレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7578c-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="7578c-105">**TokenIssuers 者**</span><span class="sxs-lookup"><span data-stu-id="7578c-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7578c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7578c-106">Attributes and elements</span></span>

<span data-ttu-id="7578c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7578c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7578c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7578c-108">Attributes</span></span>

<span data-ttu-id="7578c-109">なし</span><span class="sxs-lookup"><span data-stu-id="7578c-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7578c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7578c-110">Child elements</span></span>

|<span data-ttu-id="7578c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7578c-111">**Element**</span></span>|<span data-ttu-id="7578c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7578c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7578c-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7578c-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="7578c-114">セキュリティトークンサービスの[Uri (soap)](uri-soap.md)と[エンドポイント (soap)](endpoint-soap.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="7578c-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7578c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7578c-115">Parent elements</span></span>

|<span data-ttu-id="7578c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7578c-116">**Element**</span></span>|<span data-ttu-id="7578c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7578c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7578c-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7578c-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="7578c-119">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="7578c-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7578c-120">注釈</span><span class="sxs-lookup"><span data-stu-id="7578c-120">Remarks</span></span>

<span data-ttu-id="7578c-121">**Tokenissuers**は、Autodiscovery で使用される[TOKENISSUERS (SOAP)](tokenissuer-soap.md)要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7578c-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7578c-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7578c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7578c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="7578c-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7578c-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7578c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7578c-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="7578c-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7578c-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7578c-126">Validation File</span></span>  <br/> |<span data-ttu-id="7578c-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7578c-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7578c-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7578c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7578c-129">正しい</span><span class="sxs-lookup"><span data-stu-id="7578c-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7578c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7578c-130">See also</span></span>



[<span data-ttu-id="7578c-131">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="7578c-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="7578c-132">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="7578c-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

