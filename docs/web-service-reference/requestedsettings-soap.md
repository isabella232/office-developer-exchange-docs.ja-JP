---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: RequestedSettings 要素には、要求された構成設定の名前が含まれています。
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833136"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="96f3e-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="96f3e-104">**RequestedSettings**要素には、要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="96f3e-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="96f3e-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="96f3e-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96f3e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="96f3e-106">Attributes and elements</span></span>

<span data-ttu-id="96f3e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96f3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96f3e-108">属性</span><span class="sxs-lookup"><span data-stu-id="96f3e-108">Attributes</span></span>

<span data-ttu-id="96f3e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="96f3e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96f3e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="96f3e-110">Child elements</span></span>

|<span data-ttu-id="96f3e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="96f3e-111">**Element**</span></span>|<span data-ttu-id="96f3e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="96f3e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96f3e-113">(SOAP) の設定</span><span class="sxs-lookup"><span data-stu-id="96f3e-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="96f3e-114">返される構成設定を表します。</span><span class="sxs-lookup"><span data-stu-id="96f3e-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96f3e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="96f3e-115">Parent elements</span></span>

|<span data-ttu-id="96f3e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="96f3e-116">**Element**</span></span>|<span data-ttu-id="96f3e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="96f3e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96f3e-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="96f3e-119">1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="96f3e-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="96f3e-120">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="96f3e-121">要求された構成設定とユーザーを対象に含まれています。</span><span class="sxs-lookup"><span data-stu-id="96f3e-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="96f3e-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="96f3e-123">[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="96f3e-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="96f3e-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="96f3e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96f3e-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="96f3e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="96f3e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96f3e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="96f3e-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="96f3e-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="96f3e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96f3e-128">Validation File</span></span>  <br/> |<span data-ttu-id="96f3e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96f3e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96f3e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="96f3e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="96f3e-131">True</span><span class="sxs-lookup"><span data-stu-id="96f3e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96f3e-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="96f3e-132">See also</span></span>



[<span data-ttu-id="96f3e-133">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="96f3e-134">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="96f3e-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

