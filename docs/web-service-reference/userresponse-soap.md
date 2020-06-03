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
description: UserResponse 要素は、個々のユーザーに対する GetUserSettings 要求への応答を表します。
ms.openlocfilehash: 73848cb19d9c859e07216f354965ac4051d0d20c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468902"
---
# <a name="userresponse-soap"></a><span data-ttu-id="a0837-103">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="a0837-104">**Userresponse**要素は、個々のユーザーに対する getusersettings 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="a0837-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="a0837-105">**UserResponse**</span><span class="sxs-lookup"><span data-stu-id="a0837-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0837-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a0837-106">Attributes and elements</span></span>

<span data-ttu-id="a0837-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0837-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0837-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0837-108">Attributes</span></span>

<span data-ttu-id="a0837-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a0837-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0837-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a0837-110">Child elements</span></span>

|<span data-ttu-id="a0837-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a0837-111">**Element**</span></span>|<span data-ttu-id="a0837-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0837-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0837-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="a0837-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="a0837-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a0837-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="a0837-116">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="a0837-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a0837-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="a0837-118">リダイレクト URL またはメールアドレスのターゲットを含みます。</span><span class="sxs-lookup"><span data-stu-id="a0837-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="a0837-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="a0837-120">返すことができなかった設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a0837-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="a0837-121">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="a0837-122">ユーザーに対して要求された設定。</span><span class="sxs-lookup"><span data-stu-id="a0837-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0837-123">親要素</span><span class="sxs-lookup"><span data-stu-id="a0837-123">Parent elements</span></span>

|<span data-ttu-id="a0837-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="a0837-124">**Element**</span></span>|<span data-ttu-id="a0837-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0837-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0837-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="a0837-127">ユーザー応答の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="a0837-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="a0837-128">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a0837-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="a0837-129">要求された各ユーザーの構成設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a0837-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="a0837-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a0837-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0837-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0837-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a0837-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a0837-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a0837-133">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="a0837-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a0837-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a0837-134">Validation File</span></span>  <br/> |<span data-ttu-id="a0837-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a0837-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0837-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a0837-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0837-137">正しい</span><span class="sxs-lookup"><span data-stu-id="a0837-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0837-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0837-138">See also</span></span>



[<span data-ttu-id="a0837-139">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="a0837-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

