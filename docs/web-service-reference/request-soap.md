---
title: 要求 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: 要求要素には、要求された構成設定とターゲットのユーザーが含まれています。
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833125"
---
# <a name="request-soap"></a><span data-ttu-id="ee9e1-103">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-103">Request (SOAP)</span></span>

<span data-ttu-id="ee9e1-104">**要求**の要素には、要求された構成設定とターゲットのユーザーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="ee9e1-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="ee9e1-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee9e1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ee9e1-106">Attributes and elements</span></span>

<span data-ttu-id="ee9e1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee9e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee9e1-108">Attributes</span></span>

<span data-ttu-id="ee9e1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee9e1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ee9e1-110">Child elements</span></span>

|<span data-ttu-id="ee9e1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ee9e1-111">**Element**</span></span>|<span data-ttu-id="ee9e1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee9e1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee9e1-113">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="ee9e1-114">設定を取得する対象となるユーザーの電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="ee9e1-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="ee9e1-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="ee9e1-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="ee9e1-118">プロバイダーの利用を希望する特定のサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee9e1-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ee9e1-119">Parent elements</span></span>

|<span data-ttu-id="ee9e1-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="ee9e1-120">**Element**</span></span>|<span data-ttu-id="ee9e1-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee9e1-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee9e1-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="ee9e1-123">[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee9e1-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ee9e1-124">Text value</span></span>

<span data-ttu-id="ee9e1-125">なし。</span><span class="sxs-lookup"><span data-stu-id="ee9e1-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee9e1-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="ee9e1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee9e1-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="ee9e1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ee9e1-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ee9e1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ee9e1-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="ee9e1-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ee9e1-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ee9e1-130">Validation File</span></span>  <br/> |<span data-ttu-id="ee9e1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee9e1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee9e1-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ee9e1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee9e1-133">True</span><span class="sxs-lookup"><span data-stu-id="ee9e1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee9e1-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="ee9e1-134">See also</span></span>



[<span data-ttu-id="ee9e1-135">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ee9e1-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

