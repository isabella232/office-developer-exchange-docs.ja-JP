---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: UnifiedMessagingConfiguration 要素には、ユニファイドメッセージングサービスのサービス構成情報が含まれています。
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528693"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="6cb0d-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cb0d-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="6cb0d-104">**UnifiedMessagingConfiguration**要素には、ユニファイドメッセージングサービスのサービス構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="6cb0d-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="6cb0d-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cb0d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6cb0d-106">Attributes and elements</span></span>

<span data-ttu-id="6cb0d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cb0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cb0d-108">Attributes</span></span>

<span data-ttu-id="6cb0d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cb0d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6cb0d-110">Child elements</span></span>

|<span data-ttu-id="6cb0d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6cb0d-111">**Element**</span></span>|<span data-ttu-id="6cb0d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cb0d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cb0d-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="6cb0d-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="6cb0d-114">アカウントに対してユニファイドメッセージングが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="6cb0d-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6cb0d-116">PlayOnPhoneDialString (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="6cb0d-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="6cb0d-117">電話での通話のダイヤル文字列を識別します。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="6cb0d-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6cb0d-119">Playon電話有効</span><span class="sxs-lookup"><span data-stu-id="6cb0d-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="6cb0d-120">電話での再生機能が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="6cb0d-121">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cb0d-122">親要素</span><span class="sxs-lookup"><span data-stu-id="6cb0d-122">Parent elements</span></span>

|<span data-ttu-id="6cb0d-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cb0d-123">**Element**</span></span>|<span data-ttu-id="6cb0d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cb0d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cb0d-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="6cb0d-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="6cb0d-126">サービス構成の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6cb0d-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6cb0d-127">Text value</span></span>

<span data-ttu-id="6cb0d-128">なし。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6cb0d-129">注釈</span><span class="sxs-lookup"><span data-stu-id="6cb0d-129">Remarks</span></span>

<span data-ttu-id="6cb0d-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6cb0d-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cb0d-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6cb0d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cb0d-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="6cb0d-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cb0d-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cb0d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="6cb0d-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6cb0d-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cb0d-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cb0d-135">Validation File</span></span>  <br/> |<span data-ttu-id="6cb0d-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6cb0d-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cb0d-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6cb0d-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cb0d-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="6cb0d-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cb0d-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cb0d-139">See also</span></span>



- [<span data-ttu-id="6cb0d-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cb0d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

