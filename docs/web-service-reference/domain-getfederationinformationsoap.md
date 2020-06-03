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
description: Domain 要素は、フェデレーション信頼があるドメインを識別します。
ms.openlocfilehash: 2fcb51154d2eb9a2eeaf8b13e67aa0bd8769c53a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457033"
---
# <a name="domain-getfederationinformation-soap"></a><span data-ttu-id="4a9c9-103">ドメイン (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a9c9-103">Domain (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="4a9c9-104">**Domain**要素は、フェデレーション信頼があるドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-104">The **Domain** element identifies the domain that has a federation trust.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="4a9c9-105">**string**</span><span class="sxs-lookup"><span data-stu-id="4a9c9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a9c9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4a9c9-106">Attributes and elements</span></span>

<span data-ttu-id="4a9c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a9c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a9c9-108">Attributes</span></span>

<span data-ttu-id="4a9c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a9c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4a9c9-110">Child elements</span></span>

<span data-ttu-id="4a9c9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a9c9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4a9c9-112">Parent elements</span></span>

|<span data-ttu-id="4a9c9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a9c9-113">**Element**</span></span>|<span data-ttu-id="4a9c9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a9c9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a9c9-115">Request (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a9c9-115">Request (GetFederationInformation) (SOAP)</span></span>](request-getfederationinformationsoap.md) <br/> |<span data-ttu-id="4a9c9-116">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-116">Represents a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a9c9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a9c9-117">Text value</span></span>

<span data-ttu-id="4a9c9-118">Text 値は、フェデレーション信頼を含むドメインのドメイン名を表します。</span><span class="sxs-lookup"><span data-stu-id="4a9c9-118">The text value represents the domain name of the domain that contains the federation trust.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a9c9-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4a9c9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a9c9-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="4a9c9-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4a9c9-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a9c9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="4a9c9-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="4a9c9-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4a9c9-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a9c9-123">Validation File</span></span>  <br/> |<span data-ttu-id="4a9c9-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4a9c9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a9c9-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4a9c9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a9c9-126">正しい</span><span class="sxs-lookup"><span data-stu-id="4a9c9-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a9c9-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a9c9-127">See also</span></span>

- [<span data-ttu-id="4a9c9-128">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a9c9-128">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

