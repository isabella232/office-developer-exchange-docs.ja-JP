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
description: GetDomainSettingsRequest 要素は、GetDomainSettings operation (SOAP) 操作要求を表します。
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460961"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="efef2-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efef2-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="efef2-104">**Getdomainsettingsrequest**要素は、 [getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)操作要求を表します。</span><span class="sxs-lookup"><span data-stu-id="efef2-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="efef2-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="efef2-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efef2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="efef2-106">Attributes and elements</span></span>

<span data-ttu-id="efef2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efef2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efef2-108">属性</span><span class="sxs-lookup"><span data-stu-id="efef2-108">Attributes</span></span>

<span data-ttu-id="efef2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="efef2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efef2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="efef2-110">Child elements</span></span>

|<span data-ttu-id="efef2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="efef2-111">**Element**</span></span>|<span data-ttu-id="efef2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="efef2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efef2-113">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efef2-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="efef2-114">ドメイン識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="efef2-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="efef2-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efef2-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="efef2-116">要求されたドメイン構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="efef2-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="efef2-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efef2-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="efef2-118">プロバイダーが使用するサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="efef2-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="efef2-119">親要素</span><span class="sxs-lookup"><span data-stu-id="efef2-119">Parent elements</span></span>

<span data-ttu-id="efef2-120">なし。</span><span class="sxs-lookup"><span data-stu-id="efef2-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="efef2-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="efef2-121">Text value</span></span>

<span data-ttu-id="efef2-122">なし。</span><span class="sxs-lookup"><span data-stu-id="efef2-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efef2-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="efef2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efef2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="efef2-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="efef2-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efef2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="efef2-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="efef2-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="efef2-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efef2-127">Validation File</span></span>  <br/> |<span data-ttu-id="efef2-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="efef2-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efef2-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efef2-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="efef2-130">正しい</span><span class="sxs-lookup"><span data-stu-id="efef2-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efef2-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="efef2-131">See also</span></span>



[<span data-ttu-id="efef2-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efef2-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

