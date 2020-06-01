---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: ErrorCode 要素は、自動検出サービスによって返されるエラーコードを表します。
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460093"
---
# <a name="errorcode-soap"></a><span data-ttu-id="e6334-103">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="e6334-104">**ErrorCode**要素は、自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="e6334-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="e6334-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e6334-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6334-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e6334-106">Attributes and elements</span></span>

<span data-ttu-id="e6334-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e6334-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6334-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6334-108">Attributes</span></span>

<span data-ttu-id="e6334-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e6334-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6334-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e6334-110">Child elements</span></span>

<span data-ttu-id="e6334-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e6334-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6334-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e6334-112">Parent elements</span></span>

|<span data-ttu-id="e6334-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6334-113">**Element**</span></span>|<span data-ttu-id="e6334-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6334-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6334-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="e6334-116">自動検出サービスによって返されるすべての応答の基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="e6334-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="e6334-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="e6334-118">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e6334-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="e6334-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="e6334-120">個々のドメインに対する[Getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="e6334-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="e6334-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="e6334-122">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="e6334-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="e6334-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="e6334-124">[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="e6334-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="e6334-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="e6334-126">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6334-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="e6334-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="e6334-128">個々のユーザーの[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="e6334-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6334-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e6334-129">Text value</span></span>

<span data-ttu-id="e6334-130">Text 値は、自動検出エラー応答のエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="e6334-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="e6334-131">次の表に、 **ErrorCode**要素に使用できるテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="e6334-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="e6334-132">**エラーコードテキスト値**</span><span class="sxs-lookup"><span data-stu-id="e6334-132">**Error code text value**</span></span>|<span data-ttu-id="e6334-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6334-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e6334-134">NoError</span><span class="sxs-lookup"><span data-stu-id="e6334-134">NoError</span></span>  <br/> |<span data-ttu-id="e6334-135">エラーはありませんでした。</span><span class="sxs-lookup"><span data-stu-id="e6334-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="e6334-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="e6334-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="e6334-137">発信者は、自動検出によって返された電子メールアドレスリダイレクトに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6334-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="e6334-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="e6334-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="e6334-139">発信者は、自動検出によって返された URL リダイレクトに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6334-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="e6334-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="e6334-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="e6334-141">要求で渡されたユーザーが無効です。</span><span class="sxs-lookup"><span data-stu-id="e6334-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="e6334-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="e6334-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="e6334-143">要求が無効です。</span><span class="sxs-lookup"><span data-stu-id="e6334-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="e6334-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="e6334-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="e6334-145">指定した設定は無効です。</span><span class="sxs-lookup"><span data-stu-id="e6334-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="e6334-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="e6334-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="e6334-147">指定した設定は使用できません。</span><span class="sxs-lookup"><span data-stu-id="e6334-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="e6334-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="e6334-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="e6334-149">サーバーがビジー状態であるため、要求を処理できません。</span><span class="sxs-lookup"><span data-stu-id="e6334-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="e6334-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="e6334-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="e6334-151">要求されたドメインが無効です。</span><span class="sxs-lookup"><span data-stu-id="e6334-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="e6334-152">NotFederated</span><span class="sxs-lookup"><span data-stu-id="e6334-152">NotFederated</span></span>  <br/> |<span data-ttu-id="e6334-153">組織はフェデレーションされていません。</span><span class="sxs-lookup"><span data-stu-id="e6334-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="e6334-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="e6334-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="e6334-155">内部サーバーエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="e6334-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="e6334-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e6334-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6334-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="e6334-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e6334-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e6334-158">Schema Name</span></span>  <br/> |<span data-ttu-id="e6334-159">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="e6334-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e6334-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e6334-160">Validation File</span></span>  <br/> |<span data-ttu-id="e6334-161">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e6334-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6334-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e6334-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6334-163">正しい</span><span class="sxs-lookup"><span data-stu-id="e6334-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6334-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6334-164">See also</span></span>



[<span data-ttu-id="e6334-165">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="e6334-166">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="e6334-167">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e6334-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

