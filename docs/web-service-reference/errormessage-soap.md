---
title: エラー メッセージ (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: エラー メッセージ要素は、自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760330"
---
# <a name="errormessage-soap"></a><span data-ttu-id="af1c0-103">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="af1c0-104">**エラー メッセージ**要素は、自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="af1c0-105">**string**</span><span class="sxs-lookup"><span data-stu-id="af1c0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af1c0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af1c0-106">Attributes and elements</span></span>

<span data-ttu-id="af1c0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af1c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="af1c0-108">Attributes</span></span>

<span data-ttu-id="af1c0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="af1c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af1c0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="af1c0-110">Child elements</span></span>

<span data-ttu-id="af1c0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="af1c0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af1c0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="af1c0-112">Parent elements</span></span>

|<span data-ttu-id="af1c0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="af1c0-113">**Element**</span></span>|<span data-ttu-id="af1c0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="af1c0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af1c0-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="af1c0-116">自動検出サービスによって返されるすべての応答の基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="af1c0-118">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af1c0-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="af1c0-120">個々 のドメインの[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af1c0-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="af1c0-122">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af1c0-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="af1c0-124">[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af1c0-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="af1c0-126">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="af1c0-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="af1c0-128">個々 のユーザーに対して[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af1c0-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="af1c0-129">Text value</span></span>

<span data-ttu-id="af1c0-130">テキスト値は、エラー メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="af1c0-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af1c0-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="af1c0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af1c0-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="af1c0-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="af1c0-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af1c0-133">Schema Name</span></span>  <br/> |<span data-ttu-id="af1c0-134">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="af1c0-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="af1c0-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af1c0-135">Validation File</span></span>  <br/> |<span data-ttu-id="af1c0-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af1c0-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af1c0-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af1c0-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="af1c0-138">True</span><span class="sxs-lookup"><span data-stu-id="af1c0-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af1c0-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="af1c0-139">See also</span></span>



[<span data-ttu-id="af1c0-140">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="af1c0-141">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="af1c0-142">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="af1c0-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

