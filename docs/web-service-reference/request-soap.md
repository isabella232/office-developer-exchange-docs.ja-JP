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
description: 要求要素には、要求された構成設定と対象ユーザーが含まれています。
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448990"
---
# <a name="request-soap"></a><span data-ttu-id="09af4-103">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-103">Request (SOAP)</span></span>

<span data-ttu-id="09af4-104">**要求**要素には、要求された構成設定と対象ユーザーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09af4-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="09af4-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="09af4-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09af4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="09af4-106">Attributes and elements</span></span>

<span data-ttu-id="09af4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09af4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09af4-108">属性</span><span class="sxs-lookup"><span data-stu-id="09af4-108">Attributes</span></span>

<span data-ttu-id="09af4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="09af4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09af4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="09af4-110">Child elements</span></span>

|<span data-ttu-id="09af4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="09af4-111">**Element**</span></span>|<span data-ttu-id="09af4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="09af4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09af4-113">Users (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="09af4-114">設定を取得するユーザーの電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="09af4-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="09af4-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="09af4-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09af4-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="09af4-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="09af4-118">プロバイダーが使用する特定のサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="09af4-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09af4-119">親要素</span><span class="sxs-lookup"><span data-stu-id="09af4-119">Parent elements</span></span>

|<span data-ttu-id="09af4-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="09af4-120">**Element**</span></span>|<span data-ttu-id="09af4-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="09af4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09af4-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="09af4-123">[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="09af4-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09af4-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09af4-124">Text value</span></span>

<span data-ttu-id="09af4-125">なし。</span><span class="sxs-lookup"><span data-stu-id="09af4-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09af4-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="09af4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09af4-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="09af4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="09af4-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09af4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="09af4-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="09af4-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="09af4-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09af4-130">Validation File</span></span>  <br/> |<span data-ttu-id="09af4-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="09af4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09af4-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="09af4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="09af4-133">正しい</span><span class="sxs-lookup"><span data-stu-id="09af4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09af4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="09af4-134">See also</span></span>



[<span data-ttu-id="09af4-135">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="09af4-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

