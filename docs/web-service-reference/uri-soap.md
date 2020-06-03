---
title: Uri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4a82162a-716d-4002-820e-5bbcfb4a9696
description: URI 要素は、セキュリティトークンを発行したセキュリティトークンサービスを指定します。
ms.openlocfilehash: f4b22551eebcc318b2063feb70799839acd62c17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526572"
---
# <a name="uri-soap"></a><span data-ttu-id="15111-103">Uri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15111-103">Uri (SOAP)</span></span>

<span data-ttu-id="15111-104">**URI**要素は、セキュリティトークンを発行したセキュリティトークンサービスを指定します。</span><span class="sxs-lookup"><span data-stu-id="15111-104">The **URI** element specifies the security token service that issued the security token.</span></span> 
  
```XML
<Uri/>
```

 <span data-ttu-id="15111-105">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="15111-105">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15111-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="15111-106">Attributes and elements</span></span>

<span data-ttu-id="15111-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15111-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15111-108">属性</span><span class="sxs-lookup"><span data-stu-id="15111-108">Attributes</span></span>

<span data-ttu-id="15111-109">なし</span><span class="sxs-lookup"><span data-stu-id="15111-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15111-110">子要素</span><span class="sxs-lookup"><span data-stu-id="15111-110">Child elements</span></span>

<span data-ttu-id="15111-111">なし</span><span class="sxs-lookup"><span data-stu-id="15111-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15111-112">親要素</span><span class="sxs-lookup"><span data-stu-id="15111-112">Parent elements</span></span>

|<span data-ttu-id="15111-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="15111-113">**Element**</span></span>|<span data-ttu-id="15111-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="15111-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15111-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15111-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="15111-116">セキュリティトークンサービスの URI とエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="15111-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15111-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="15111-117">Text value</span></span>

<span data-ttu-id="15111-118">Text 値は、security token service の URI を表します。</span><span class="sxs-lookup"><span data-stu-id="15111-118">The text value represents the URI of the security token service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15111-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="15111-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15111-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="15111-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="15111-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15111-121">Schema Name</span></span>  <br/> |<span data-ttu-id="15111-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="15111-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="15111-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15111-123">Validation File</span></span>  <br/> |<span data-ttu-id="15111-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="15111-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15111-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="15111-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="15111-126">はい</span><span class="sxs-lookup"><span data-stu-id="15111-126">True</span></span>  <br/> |
   

