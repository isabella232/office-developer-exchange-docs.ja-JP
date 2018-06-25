---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: AutodiscoverResponse (SOAP) の要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759476"
---
# <a name="autodiscoverresponse-soap"></a><span data-ttu-id="f3dba-103">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-103">AutodiscoverResponse (SOAP)</span></span>

<span data-ttu-id="f3dba-104">**AutodiscoverResponse (SOAP)** の要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。</span><span class="sxs-lookup"><span data-stu-id="f3dba-104">The **AutodiscoverResponse (SOAP)** element represents the base element for all responses that are returned by the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="f3dba-105">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-105">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 <span data-ttu-id="f3dba-106">**AutodiscoverResponse**</span><span class="sxs-lookup"><span data-stu-id="f3dba-106">**AutodiscoverResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3dba-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f3dba-107">Attributes and elements</span></span>

<span data-ttu-id="f3dba-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3dba-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3dba-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3dba-109">Attributes</span></span>

<span data-ttu-id="f3dba-110">なし。</span><span class="sxs-lookup"><span data-stu-id="f3dba-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3dba-111">子要素</span><span class="sxs-lookup"><span data-stu-id="f3dba-111">Child elements</span></span>

|<span data-ttu-id="f3dba-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3dba-112">**Element**</span></span>|<span data-ttu-id="f3dba-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3dba-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3dba-114">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-114">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="f3dba-115">[UserResponse (SOAP)](userresponse-soap.md)要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f3dba-115">Represents a collection of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="f3dba-116">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-116">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="f3dba-117">[UserSettingError (SOAP)](usersettingerror-soap.md)要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f3dba-117">Represents a collection of [UserSettingError (SOAP)](usersettingerror-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="f3dba-118">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-118">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="f3dba-119">[UserSetting (SOAP)](usersetting-soap.md)要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f3dba-119">Represents a collection of [UserSetting (SOAP)](usersetting-soap.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3dba-120">親要素</span><span class="sxs-lookup"><span data-stu-id="f3dba-120">Parent elements</span></span>

<span data-ttu-id="f3dba-121">なし。</span><span class="sxs-lookup"><span data-stu-id="f3dba-121">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f3dba-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f3dba-122">Text value</span></span>

<span data-ttu-id="f3dba-123">なし。</span><span class="sxs-lookup"><span data-stu-id="f3dba-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3dba-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="f3dba-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3dba-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="f3dba-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f3dba-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f3dba-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f3dba-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="f3dba-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f3dba-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f3dba-128">Validation File</span></span>  <br/> |<span data-ttu-id="f3dba-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3dba-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3dba-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f3dba-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3dba-131">True</span><span class="sxs-lookup"><span data-stu-id="f3dba-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3dba-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3dba-132">See also</span></span>

- [<span data-ttu-id="f3dba-133">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="f3dba-134">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
- [<span data-ttu-id="f3dba-135">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3dba-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

