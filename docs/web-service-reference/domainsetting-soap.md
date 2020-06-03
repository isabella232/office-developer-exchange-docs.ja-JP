---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: DomainSetting 要素には、GetDomainSettings operation (SOAP) 操作要求によって返されるドメイン設定が含まれています。
ms.openlocfilehash: 54441dd7cfcf7372807a1e6bfd8ea5d26805bffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526299"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="7cec4-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7cec4-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="7cec4-104">**Domainsetting**要素には、 [getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)操作要求によって返されるドメイン設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7cec4-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="7cec4-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="7cec4-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cec4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7cec4-106">Attributes and elements</span></span>

<span data-ttu-id="7cec4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7cec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cec4-108">属性</span><span class="sxs-lookup"><span data-stu-id="7cec4-108">Attributes</span></span>

<span data-ttu-id="7cec4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7cec4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cec4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7cec4-110">Child elements</span></span>

|<span data-ttu-id="7cec4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7cec4-111">**Element**</span></span>|<span data-ttu-id="7cec4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cec4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cec4-113">Name (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7cec4-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="7cec4-114">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="7cec4-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cec4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7cec4-115">Parent elements</span></span>

|<span data-ttu-id="7cec4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cec4-116">**Element**</span></span>|<span data-ttu-id="7cec4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cec4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cec4-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7cec4-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="7cec4-119">自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。</span><span class="sxs-lookup"><span data-stu-id="7cec4-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cec4-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7cec4-120">Text value</span></span>

<span data-ttu-id="7cec4-121">なし。</span><span class="sxs-lookup"><span data-stu-id="7cec4-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cec4-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7cec4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cec4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="7cec4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7cec4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7cec4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7cec4-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="7cec4-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7cec4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7cec4-126">Validation File</span></span>  <br/> |<span data-ttu-id="7cec4-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7cec4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7cec4-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7cec4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cec4-129">正しい</span><span class="sxs-lookup"><span data-stu-id="7cec4-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cec4-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7cec4-130">See also</span></span>

- [<span data-ttu-id="7cec4-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7cec4-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

