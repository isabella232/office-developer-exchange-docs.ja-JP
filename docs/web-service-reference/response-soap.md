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
description: Response 要素には、GetUserSettings 操作 (SOAP)、GetDomainSettings operation (SOAP)、または GetFederationInformation operation (SOAP) 要求への応答が含まれています。
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456417"
---
# <a name="response-soap"></a><span data-ttu-id="3493b-103">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-103">Response (SOAP)</span></span>

<span data-ttu-id="3493b-104">**Response**要素には、 [getusersettings 操作 (soap)](getusersettings-operation-soap.md)、 [GETDOMAINSETTINGS operation (Soap)](getdomainsettings-operation-soap.md)、または[GetFederationInformation operation (soap)](getfederationinformation-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3493b-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="3493b-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="3493b-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3493b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3493b-106">Attributes and elements</span></span>

<span data-ttu-id="3493b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3493b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3493b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3493b-108">Attributes</span></span>

<span data-ttu-id="3493b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3493b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3493b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3493b-110">Child elements</span></span>

|<span data-ttu-id="3493b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3493b-111">**Element**</span></span>|<span data-ttu-id="3493b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3493b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3493b-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3493b-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="3493b-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3493b-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3493b-116">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3493b-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3493b-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="3493b-118">要求された各ユーザーの構成設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3493b-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3493b-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3493b-119">Parent elements</span></span>

|<span data-ttu-id="3493b-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="3493b-120">**Element**</span></span>|<span data-ttu-id="3493b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3493b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3493b-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="3493b-123">[Getusersettingsrequest (SOAP)](getusersettingsrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3493b-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="3493b-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="3493b-125">[Getdomainsettingsrequest (SOAP)](getdomainsettingsrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3493b-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="3493b-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="3493b-127">[GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3493b-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3493b-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3493b-128">Text value</span></span>

<span data-ttu-id="3493b-129">なし。</span><span class="sxs-lookup"><span data-stu-id="3493b-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3493b-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3493b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3493b-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="3493b-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3493b-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3493b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="3493b-133">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="3493b-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3493b-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3493b-134">Validation File</span></span>  <br/> |<span data-ttu-id="3493b-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3493b-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3493b-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3493b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="3493b-137">正しい</span><span class="sxs-lookup"><span data-stu-id="3493b-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3493b-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="3493b-138">See also</span></span>



[<span data-ttu-id="3493b-139">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3493b-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="3493b-140">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="3493b-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="3493b-141">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="3493b-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

