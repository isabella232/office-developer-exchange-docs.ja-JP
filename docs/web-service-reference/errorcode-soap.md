---
title: エラー コード (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: エラー コード要素は、自動検出サービスによって返されるエラー コードを表します。
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760320"
---
# <a name="errorcode-soap"></a><span data-ttu-id="2078e-103">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="2078e-104">**エラー コード**要素は、自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="2078e-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="2078e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="2078e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2078e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2078e-106">Attributes and elements</span></span>

<span data-ttu-id="2078e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2078e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2078e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2078e-108">Attributes</span></span>

<span data-ttu-id="2078e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2078e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2078e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2078e-110">Child elements</span></span>

<span data-ttu-id="2078e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2078e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2078e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2078e-112">Parent elements</span></span>

|<span data-ttu-id="2078e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2078e-113">**Element**</span></span>|<span data-ttu-id="2078e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2078e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2078e-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="2078e-116">自動検出サービスによって返されるすべての応答の基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="2078e-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="2078e-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="2078e-118">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2078e-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="2078e-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="2078e-120">個々 のドメインの[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2078e-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="2078e-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="2078e-122">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2078e-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="2078e-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="2078e-124">[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2078e-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="2078e-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="2078e-126">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="2078e-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="2078e-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="2078e-128">個々 のユーザーに対して[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="2078e-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2078e-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2078e-129">Text value</span></span>

<span data-ttu-id="2078e-130">テキスト値は、自動検出エラー応答のエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="2078e-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="2078e-131">可能なテキスト要素の値、**エラー コード**を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="2078e-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="2078e-132">**エラー コードのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="2078e-132">**Error code text value**</span></span>|<span data-ttu-id="2078e-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="2078e-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2078e-134">NoError</span><span class="sxs-lookup"><span data-stu-id="2078e-134">NoError</span></span>  <br/> |<span data-ttu-id="2078e-135">エラーはありませんでした。</span><span class="sxs-lookup"><span data-stu-id="2078e-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="2078e-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="2078e-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="2078e-137">呼び出し元は、自動検出によって返された電子メール アドレスのリダイレクトに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="2078e-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="2078e-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="2078e-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="2078e-139">呼び出し元は、自動検出によって返された URL のリダイレクトに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="2078e-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="2078e-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="2078e-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="2078e-141">要求で渡されたユーザーが正しくありません。</span><span class="sxs-lookup"><span data-stu-id="2078e-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="2078e-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="2078e-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="2078e-143">要求が有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="2078e-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="2078e-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="2078e-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="2078e-145">指定した設定が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="2078e-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="2078e-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="2078e-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="2078e-147">指定した設定が使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="2078e-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="2078e-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="2078e-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="2078e-149">サーバは、要求を処理するがビジー状態です。</span><span class="sxs-lookup"><span data-stu-id="2078e-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="2078e-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="2078e-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="2078e-151">要求されたドメインが正しくありません。</span><span class="sxs-lookup"><span data-stu-id="2078e-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="2078e-152">NotFederated</span><span class="sxs-lookup"><span data-stu-id="2078e-152">NotFederated</span></span>  <br/> |<span data-ttu-id="2078e-153">組織は連合がないです。</span><span class="sxs-lookup"><span data-stu-id="2078e-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="2078e-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="2078e-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="2078e-155">内部サーバー エラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2078e-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2078e-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="2078e-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2078e-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="2078e-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2078e-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2078e-158">Schema Name</span></span>  <br/> |<span data-ttu-id="2078e-159">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="2078e-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2078e-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2078e-160">Validation File</span></span>  <br/> |<span data-ttu-id="2078e-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2078e-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2078e-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2078e-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="2078e-163">True</span><span class="sxs-lookup"><span data-stu-id="2078e-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2078e-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="2078e-164">See also</span></span>



[<span data-ttu-id="2078e-165">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="2078e-166">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="2078e-167">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2078e-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

