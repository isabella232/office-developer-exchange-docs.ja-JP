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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458398"
---
# <a name="endpoint-soap"></a><span data-ttu-id="b7b18-103">エンドポイント (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7b18-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="b7b18-104">**Endpoint**要素は、security token service エンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7b18-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="b7b18-105">**xs: anyURI**</span><span class="sxs-lookup"><span data-stu-id="b7b18-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7b18-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b7b18-106">Attributes and elements</span></span>

<span data-ttu-id="b7b18-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b7b18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7b18-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7b18-108">Attributes</span></span>

<span data-ttu-id="b7b18-109">なし</span><span class="sxs-lookup"><span data-stu-id="b7b18-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7b18-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b7b18-110">Child elements</span></span>

<span data-ttu-id="b7b18-111">なし</span><span class="sxs-lookup"><span data-stu-id="b7b18-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7b18-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b7b18-112">Parent elements</span></span>

|<span data-ttu-id="b7b18-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7b18-113">**Element**</span></span>|<span data-ttu-id="b7b18-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7b18-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7b18-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7b18-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="b7b18-116">セキュリティトークンサービスの URI とエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7b18-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7b18-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b7b18-117">Text value</span></span>

<span data-ttu-id="b7b18-118">Text 値は、セキュリティトークン web サービスのエンドポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="b7b18-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7b18-119">注釈</span><span class="sxs-lookup"><span data-stu-id="b7b18-119">Remarks</span></span>

<span data-ttu-id="b7b18-120">エンドポイントは、セキュリティトークン web サービスとの通信に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b7b18-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7b18-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b7b18-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7b18-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="b7b18-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b7b18-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b7b18-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b7b18-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="b7b18-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b7b18-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b7b18-125">Validation File</span></span>  <br/> |<span data-ttu-id="b7b18-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b7b18-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7b18-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b7b18-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7b18-128">はい</span><span class="sxs-lookup"><span data-stu-id="b7b18-128">True</span></span>  <br/> |
   

