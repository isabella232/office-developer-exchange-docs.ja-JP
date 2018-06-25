---
title: エンドポイント (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: エンドポイント要素は、セキュリティ トークン サービスのエンドポイントを指定します。
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760295"
---
# <a name="endpoint-soap"></a><span data-ttu-id="8aee9-103">エンドポイント (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8aee9-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="8aee9-104">**エンドポイント**要素は、セキュリティ トークン サービスのエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="8aee9-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="8aee9-105">**xs:anyURI**</span><span class="sxs-lookup"><span data-stu-id="8aee9-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8aee9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8aee9-106">Attributes and elements</span></span>

<span data-ttu-id="8aee9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8aee9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8aee9-108">属性</span><span class="sxs-lookup"><span data-stu-id="8aee9-108">Attributes</span></span>

<span data-ttu-id="8aee9-109">なし</span><span class="sxs-lookup"><span data-stu-id="8aee9-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8aee9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8aee9-110">Child elements</span></span>

<span data-ttu-id="8aee9-111">なし</span><span class="sxs-lookup"><span data-stu-id="8aee9-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8aee9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8aee9-112">Parent elements</span></span>

|<span data-ttu-id="8aee9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8aee9-113">**Element**</span></span>|<span data-ttu-id="8aee9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8aee9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8aee9-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8aee9-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="8aee9-116">セキュリティ トークン サービスの URI のエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="8aee9-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8aee9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8aee9-117">Text value</span></span>

<span data-ttu-id="8aee9-118">テキスト値は、セキュリティ トークンの web サービスのエンドポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="8aee9-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8aee9-119">備考</span><span class="sxs-lookup"><span data-stu-id="8aee9-119">Remarks</span></span>

<span data-ttu-id="8aee9-120">エンドポイントは、セキュリティ トークンの web サービスと通信するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8aee9-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8aee9-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="8aee9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8aee9-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="8aee9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8aee9-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8aee9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8aee9-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="8aee9-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8aee9-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8aee9-125">Validation File</span></span>  <br/> |<span data-ttu-id="8aee9-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8aee9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8aee9-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8aee9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8aee9-128">True</span><span class="sxs-lookup"><span data-stu-id="8aee9-128">True</span></span>  <br/> |
   

