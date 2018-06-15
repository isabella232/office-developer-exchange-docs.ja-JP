---
title: UserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: UserResponse 要素は、個々 のユーザーの GetUserSettings の要求に対する応答を表します。
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19839948"
---
# <a name="userresponse-soap"></a><span data-ttu-id="e8138-103">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="e8138-104">**UserResponse**要素は、個々 のユーザーの GetUserSettings の要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="e8138-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="e8138-105">**UserResponse**</span><span class="sxs-lookup"><span data-stu-id="e8138-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8138-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e8138-106">Attributes and elements</span></span>

<span data-ttu-id="e8138-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8138-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8138-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8138-108">Attributes</span></span>

<span data-ttu-id="e8138-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8138-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8138-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8138-110">Child elements</span></span>

|<span data-ttu-id="e8138-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8138-111">**Element**</span></span>|<span data-ttu-id="e8138-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8138-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8138-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="e8138-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="e8138-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="e8138-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="e8138-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e8138-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="e8138-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="e8138-118">リダイレクト URL または電子メール アドレスのターゲットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8138-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="e8138-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="e8138-120">返されませんでしたの設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e8138-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="e8138-121">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="e8138-122">ユーザーの要求された設定です。</span><span class="sxs-lookup"><span data-stu-id="e8138-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8138-123">親要素</span><span class="sxs-lookup"><span data-stu-id="e8138-123">Parent elements</span></span>

|<span data-ttu-id="e8138-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8138-124">**Element**</span></span>|<span data-ttu-id="e8138-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8138-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8138-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="e8138-127">ユーザー応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8138-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="e8138-128">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8138-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="e8138-129">要求された各ユーザーの構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8138-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="e8138-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="e8138-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8138-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="e8138-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e8138-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8138-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e8138-133">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e8138-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e8138-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8138-134">Validation File</span></span>  <br/> |<span data-ttu-id="e8138-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8138-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8138-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e8138-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8138-137">True</span><span class="sxs-lookup"><span data-stu-id="e8138-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8138-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8138-138">See also</span></span>



[<span data-ttu-id="e8138-139">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="e8138-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

