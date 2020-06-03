---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: ErrorMessage 要素は、自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。
ms.openlocfilehash: 4ebaf91fe26083cf241826e1fc16ac184fddf57c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530643"
---
# <a name="errormessage-soap"></a><span data-ttu-id="36d96-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="36d96-104">**ErrorMessage**要素は、自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="36d96-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="36d96-105">**string**</span><span class="sxs-lookup"><span data-stu-id="36d96-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36d96-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36d96-106">Attributes and elements</span></span>

<span data-ttu-id="36d96-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36d96-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36d96-108">属性</span><span class="sxs-lookup"><span data-stu-id="36d96-108">Attributes</span></span>

<span data-ttu-id="36d96-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36d96-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36d96-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36d96-110">Child elements</span></span>

<span data-ttu-id="36d96-111">なし。</span><span class="sxs-lookup"><span data-stu-id="36d96-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36d96-112">親要素</span><span class="sxs-lookup"><span data-stu-id="36d96-112">Parent elements</span></span>

|<span data-ttu-id="36d96-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="36d96-113">**Element**</span></span>|<span data-ttu-id="36d96-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="36d96-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36d96-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="36d96-116">自動検出サービスによって返されるすべての応答の基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="36d96-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="36d96-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="36d96-118">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="36d96-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="36d96-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="36d96-120">個々のドメインに対する[Getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="36d96-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="36d96-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="36d96-122">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="36d96-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="36d96-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="36d96-124">[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="36d96-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="36d96-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="36d96-126">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="36d96-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="36d96-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="36d96-128">個々のユーザーの[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="36d96-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36d96-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="36d96-129">Text value</span></span>

<span data-ttu-id="36d96-130">テキスト値は、エラーメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="36d96-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36d96-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36d96-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36d96-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="36d96-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="36d96-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36d96-133">Schema Name</span></span>  <br/> |<span data-ttu-id="36d96-134">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="36d96-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="36d96-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36d96-135">Validation File</span></span>  <br/> |<span data-ttu-id="36d96-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="36d96-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36d96-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36d96-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="36d96-138">正しい</span><span class="sxs-lookup"><span data-stu-id="36d96-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36d96-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="36d96-139">See also</span></span>



[<span data-ttu-id="36d96-140">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="36d96-141">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="36d96-142">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="36d96-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

