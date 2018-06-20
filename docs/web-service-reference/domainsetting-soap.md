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
description: DomainSetting 要素には、GetDomainSettings (SOAP) の操作の操作要求によって返されるドメインの設定が含まれています。
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760161"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="73e1c-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73e1c-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="73e1c-104">**DomainSetting**要素には、 [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)操作の要求によって返されるドメインの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="73e1c-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="73e1c-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="73e1c-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73e1c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="73e1c-106">Attributes and elements</span></span>

<span data-ttu-id="73e1c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73e1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73e1c-108">属性</span><span class="sxs-lookup"><span data-stu-id="73e1c-108">Attributes</span></span>

<span data-ttu-id="73e1c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="73e1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73e1c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="73e1c-110">Child elements</span></span>

|<span data-ttu-id="73e1c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="73e1c-111">**Element**</span></span>|<span data-ttu-id="73e1c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="73e1c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73e1c-113">名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73e1c-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="73e1c-114">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="73e1c-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73e1c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="73e1c-115">Parent elements</span></span>

|<span data-ttu-id="73e1c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="73e1c-116">**Element**</span></span>|<span data-ttu-id="73e1c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="73e1c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73e1c-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73e1c-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="73e1c-119">自動検出要求の送信、または、自動検出応答によって返されるドメインの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="73e1c-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73e1c-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="73e1c-120">Text value</span></span>

<span data-ttu-id="73e1c-121">なし。</span><span class="sxs-lookup"><span data-stu-id="73e1c-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73e1c-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="73e1c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73e1c-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="73e1c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="73e1c-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73e1c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="73e1c-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="73e1c-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="73e1c-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73e1c-126">Validation File</span></span>  <br/> |<span data-ttu-id="73e1c-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73e1c-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73e1c-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73e1c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="73e1c-129">True</span><span class="sxs-lookup"><span data-stu-id="73e1c-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73e1c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="73e1c-130">See also</span></span>

- [<span data-ttu-id="73e1c-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73e1c-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

