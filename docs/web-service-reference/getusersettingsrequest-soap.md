---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: GetUserSettingsRequest 要素は、1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。
ms.openlocfilehash: dc22570144a6947dc6e7042326c7416422680cc1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831702"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="ce22f-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce22f-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="ce22f-104">**GetUserSettingsRequest**要素は、1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="ce22f-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="ce22f-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="ce22f-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce22f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ce22f-106">Attributes and elements</span></span>

<span data-ttu-id="ce22f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce22f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce22f-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce22f-108">Attributes</span></span>

<span data-ttu-id="ce22f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ce22f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce22f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ce22f-110">Child elements</span></span>

|<span data-ttu-id="ce22f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ce22f-111">**Element**</span></span>|<span data-ttu-id="ce22f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce22f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce22f-113">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce22f-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="ce22f-114">設定を取得する対象となるユーザーの電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ce22f-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="ce22f-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce22f-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="ce22f-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce22f-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="ce22f-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce22f-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="ce22f-118">プロバイダーの利用を希望する特定のサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="ce22f-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce22f-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ce22f-119">Parent elements</span></span>

<span data-ttu-id="ce22f-120">なし。</span><span class="sxs-lookup"><span data-stu-id="ce22f-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ce22f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ce22f-121">Text value</span></span>

<span data-ttu-id="ce22f-122">なし。</span><span class="sxs-lookup"><span data-stu-id="ce22f-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce22f-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="ce22f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce22f-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="ce22f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ce22f-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce22f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ce22f-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="ce22f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ce22f-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce22f-127">Validation File</span></span>  <br/> |<span data-ttu-id="ce22f-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce22f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce22f-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ce22f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce22f-130">True</span><span class="sxs-lookup"><span data-stu-id="ce22f-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce22f-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce22f-131">See also</span></span>



[<span data-ttu-id="ce22f-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce22f-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

