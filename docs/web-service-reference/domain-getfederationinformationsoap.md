---
title: ドメイン (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 56aeb659-8309-47a6-8c41-9f8b0436438c
description: ドメイン要素は、フェデレーションの信頼されているドメインを識別します。
ms.openlocfilehash: 240c0b7cc13257ee36833625125691d4e51a103d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760151"
---
# <a name="domain-getfederationinformation-soap"></a><span data-ttu-id="eeb48-103">ドメイン (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eeb48-103">Domain (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="eeb48-104">**ドメイン**要素は、フェデレーションの信頼されているドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="eeb48-104">The **Domain** element identifies the domain that has a federation trust.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="eeb48-105">**string**</span><span class="sxs-lookup"><span data-stu-id="eeb48-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eeb48-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eeb48-106">Attributes and elements</span></span>

<span data-ttu-id="eeb48-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eeb48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eeb48-108">属性</span><span class="sxs-lookup"><span data-stu-id="eeb48-108">Attributes</span></span>

<span data-ttu-id="eeb48-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eeb48-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eeb48-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eeb48-110">Child elements</span></span>

<span data-ttu-id="eeb48-111">なし。</span><span class="sxs-lookup"><span data-stu-id="eeb48-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eeb48-112">親要素</span><span class="sxs-lookup"><span data-stu-id="eeb48-112">Parent elements</span></span>

|<span data-ttu-id="eeb48-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="eeb48-113">**Element**</span></span>|<span data-ttu-id="eeb48-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="eeb48-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eeb48-115">要求 (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eeb48-115">Request (GetFederationInformation) (SOAP)</span></span>](request-getfederationinformationsoap.md) <br/> |<span data-ttu-id="eeb48-116">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="eeb48-116">Represents a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eeb48-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eeb48-117">Text value</span></span>

<span data-ttu-id="eeb48-118">テキスト値は、フェデレーションの信頼を含むドメインのドメイン名を表します。</span><span class="sxs-lookup"><span data-stu-id="eeb48-118">The text value represents the domain name of the domain that contains the federation trust.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eeb48-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="eeb48-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eeb48-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="eeb48-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="eeb48-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eeb48-121">Schema Name</span></span>  <br/> |<span data-ttu-id="eeb48-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="eeb48-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="eeb48-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eeb48-123">Validation File</span></span>  <br/> |<span data-ttu-id="eeb48-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eeb48-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eeb48-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eeb48-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="eeb48-126">True</span><span class="sxs-lookup"><span data-stu-id="eeb48-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eeb48-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="eeb48-127">See also</span></span>

- [<span data-ttu-id="eeb48-128">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eeb48-128">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

