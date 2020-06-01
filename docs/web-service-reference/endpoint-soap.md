---
title: エンドポイント (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: Endpoint 要素は、security token service エンドポイントを指定します。
ms.openlocfilehash: 93659bbefa4a95063304cf3abad81cb61767070a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458398"
---
# <a name="endpoint-soap"></a><span data-ttu-id="62a8f-103">エンドポイント (SOAP)</span><span class="sxs-lookup"><span data-stu-id="62a8f-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="62a8f-104">**Endpoint**要素は、security token service エンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="62a8f-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="62a8f-105">**xs: anyURI**</span><span class="sxs-lookup"><span data-stu-id="62a8f-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62a8f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="62a8f-106">Attributes and elements</span></span>

<span data-ttu-id="62a8f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="62a8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62a8f-108">属性</span><span class="sxs-lookup"><span data-stu-id="62a8f-108">Attributes</span></span>

<span data-ttu-id="62a8f-109">なし</span><span class="sxs-lookup"><span data-stu-id="62a8f-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62a8f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="62a8f-110">Child elements</span></span>

<span data-ttu-id="62a8f-111">なし</span><span class="sxs-lookup"><span data-stu-id="62a8f-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="62a8f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="62a8f-112">Parent elements</span></span>

|<span data-ttu-id="62a8f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="62a8f-113">**Element**</span></span>|<span data-ttu-id="62a8f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="62a8f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62a8f-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="62a8f-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="62a8f-116">セキュリティトークンサービスの URI とエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="62a8f-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="62a8f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="62a8f-117">Text value</span></span>

<span data-ttu-id="62a8f-118">Text 値は、セキュリティトークン web サービスのエンドポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="62a8f-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="62a8f-119">注釈</span><span class="sxs-lookup"><span data-stu-id="62a8f-119">Remarks</span></span>

<span data-ttu-id="62a8f-120">エンドポイントは、セキュリティトークン web サービスとの通信に使用されます。</span><span class="sxs-lookup"><span data-stu-id="62a8f-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62a8f-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="62a8f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62a8f-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="62a8f-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="62a8f-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="62a8f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="62a8f-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="62a8f-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="62a8f-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="62a8f-125">Validation File</span></span>  <br/> |<span data-ttu-id="62a8f-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="62a8f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="62a8f-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="62a8f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="62a8f-128">はい</span><span class="sxs-lookup"><span data-stu-id="62a8f-128">True</span></span>  <br/> |
   

