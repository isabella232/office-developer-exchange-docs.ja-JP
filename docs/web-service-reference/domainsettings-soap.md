---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: DomainSettings 要素は、自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。
ms.openlocfilehash: 67e3753b0cf5c7c653664ff087f697ce7ae2b7a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530699"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="0d222-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d222-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="0d222-104">**Domainsettings**要素は、自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0d222-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="0d222-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="0d222-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d222-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0d222-106">Attributes and elements</span></span>

<span data-ttu-id="0d222-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0d222-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d222-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d222-108">Attributes</span></span>

<span data-ttu-id="0d222-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0d222-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d222-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0d222-110">Child elements</span></span>

|<span data-ttu-id="0d222-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0d222-111">**Element**</span></span>|<span data-ttu-id="0d222-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0d222-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d222-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d222-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="0d222-114">[Getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)要求によって返されるドメイン設定が保存されています。</span><span class="sxs-lookup"><span data-stu-id="0d222-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d222-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0d222-115">Parent elements</span></span>

|<span data-ttu-id="0d222-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="0d222-116">**Element**</span></span>|<span data-ttu-id="0d222-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0d222-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d222-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d222-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="0d222-119">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0d222-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d222-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0d222-120">Text value</span></span>

<span data-ttu-id="0d222-121">なし。</span><span class="sxs-lookup"><span data-stu-id="0d222-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d222-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0d222-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d222-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d222-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0d222-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0d222-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0d222-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="0d222-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0d222-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0d222-126">Validation File</span></span>  <br/> |<span data-ttu-id="0d222-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0d222-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d222-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0d222-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d222-129">正しい</span><span class="sxs-lookup"><span data-stu-id="0d222-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d222-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="0d222-130">See also</span></span>

- [<span data-ttu-id="0d222-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d222-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

