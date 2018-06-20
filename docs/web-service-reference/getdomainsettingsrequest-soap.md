---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: GetDomainSettingsRequest 要素は、GetDomainSettings 操作 (SOAP) 操作要求を表します。
ms.openlocfilehash: 4de525a9ba47a0d9afb0d6db9200fe32845f31d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760697"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="a882f-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a882f-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="a882f-104">**GetDomainSettingsRequest**要素は、 [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)操作要求を表します。</span><span class="sxs-lookup"><span data-stu-id="a882f-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="a882f-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="a882f-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a882f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a882f-106">Attributes and elements</span></span>

<span data-ttu-id="a882f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a882f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a882f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a882f-108">Attributes</span></span>

<span data-ttu-id="a882f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a882f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a882f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a882f-110">Child elements</span></span>

|<span data-ttu-id="a882f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a882f-111">**Element**</span></span>|<span data-ttu-id="a882f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a882f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a882f-113">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a882f-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="a882f-114">ドメイン識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a882f-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="a882f-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a882f-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="a882f-116">要求されたドメインの構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a882f-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="a882f-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a882f-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="a882f-118">プロバイダーを使用するサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="a882f-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a882f-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a882f-119">Parent elements</span></span>

<span data-ttu-id="a882f-120">なし。</span><span class="sxs-lookup"><span data-stu-id="a882f-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a882f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a882f-121">Text value</span></span>

<span data-ttu-id="a882f-122">なし。</span><span class="sxs-lookup"><span data-stu-id="a882f-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a882f-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="a882f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a882f-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="a882f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a882f-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a882f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a882f-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="a882f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a882f-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a882f-127">Validation File</span></span>  <br/> |<span data-ttu-id="a882f-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a882f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a882f-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a882f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a882f-130">True</span><span class="sxs-lookup"><span data-stu-id="a882f-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a882f-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="a882f-131">See also</span></span>



[<span data-ttu-id="a882f-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a882f-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

