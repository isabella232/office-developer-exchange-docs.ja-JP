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
ms.openlocfilehash: e94c02d8f92d7aaac619c58f093c536cc1a098bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465297"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="06100-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="06100-104">**Requestedsettings**要素には、要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="06100-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="06100-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="06100-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06100-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06100-106">Attributes and elements</span></span>

<span data-ttu-id="06100-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06100-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06100-108">属性</span><span class="sxs-lookup"><span data-stu-id="06100-108">Attributes</span></span>

<span data-ttu-id="06100-109">なし。</span><span class="sxs-lookup"><span data-stu-id="06100-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06100-110">子要素</span><span class="sxs-lookup"><span data-stu-id="06100-110">Child elements</span></span>

|<span data-ttu-id="06100-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="06100-111">**Element**</span></span>|<span data-ttu-id="06100-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="06100-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06100-113">Setting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="06100-114">返される構成設定を表します。</span><span class="sxs-lookup"><span data-stu-id="06100-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06100-115">親要素</span><span class="sxs-lookup"><span data-stu-id="06100-115">Parent elements</span></span>

|<span data-ttu-id="06100-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="06100-116">**Element**</span></span>|<span data-ttu-id="06100-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="06100-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06100-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="06100-119">1人または複数のユーザーに対して指定された設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="06100-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="06100-120">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="06100-121">要求された構成設定と対象ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="06100-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="06100-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="06100-123">[Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="06100-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="06100-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06100-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06100-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="06100-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="06100-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06100-126">Schema Name</span></span>  <br/> |<span data-ttu-id="06100-127">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="06100-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="06100-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06100-128">Validation File</span></span>  <br/> |<span data-ttu-id="06100-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="06100-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06100-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="06100-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="06100-131">正しい</span><span class="sxs-lookup"><span data-stu-id="06100-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06100-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="06100-132">See also</span></span>



[<span data-ttu-id="06100-133">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="06100-134">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06100-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

