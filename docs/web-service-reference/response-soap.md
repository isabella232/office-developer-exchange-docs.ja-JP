---
title: 応答 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: 応答要素には、GetUserSettings 操作 (SOAP)、GetDomainSettings の操作 (SOAP)、または GetFederationInformation の操作 (SOAP) 要求への応答が含まれています。
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833179"
---
# <a name="response-soap"></a><span data-ttu-id="02137-103">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-103">Response (SOAP)</span></span>

<span data-ttu-id="02137-104">**応答**要素には、 [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)、 [GetDomainSettings の操作 (SOAP)](getdomainsettings-operation-soap.md)、または[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="02137-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="02137-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="02137-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02137-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="02137-106">Attributes and elements</span></span>

<span data-ttu-id="02137-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="02137-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02137-108">属性</span><span class="sxs-lookup"><span data-stu-id="02137-108">Attributes</span></span>

<span data-ttu-id="02137-109">なし。</span><span class="sxs-lookup"><span data-stu-id="02137-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02137-110">子要素</span><span class="sxs-lookup"><span data-stu-id="02137-110">Child elements</span></span>

|<span data-ttu-id="02137-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="02137-111">**Element**</span></span>|<span data-ttu-id="02137-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="02137-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02137-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="02137-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="02137-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="02137-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="02137-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="02137-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="02137-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="02137-118">要求された各ユーザーの構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="02137-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02137-119">親要素</span><span class="sxs-lookup"><span data-stu-id="02137-119">Parent elements</span></span>

|<span data-ttu-id="02137-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="02137-120">**Element**</span></span>|<span data-ttu-id="02137-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="02137-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02137-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="02137-123">[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="02137-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="02137-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="02137-125">[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="02137-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="02137-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="02137-127">[GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="02137-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02137-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="02137-128">Text value</span></span>

<span data-ttu-id="02137-129">なし。</span><span class="sxs-lookup"><span data-stu-id="02137-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02137-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="02137-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02137-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="02137-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="02137-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="02137-132">Schema Name</span></span>  <br/> |<span data-ttu-id="02137-133">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="02137-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="02137-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="02137-134">Validation File</span></span>  <br/> |<span data-ttu-id="02137-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02137-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02137-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="02137-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="02137-137">True</span><span class="sxs-lookup"><span data-stu-id="02137-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02137-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="02137-138">See also</span></span>



[<span data-ttu-id="02137-139">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02137-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="02137-140">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="02137-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="02137-141">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="02137-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

