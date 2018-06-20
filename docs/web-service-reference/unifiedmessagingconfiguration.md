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
description: UnifiedMessagingConfiguration 要素には、ユニファイド メッセージング サービスのサービスの構成情報が含まれています。
ms.openlocfilehash: 3ad8f66ecdf21062c00c2a6ac6f65fac875da38c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839781"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="e396e-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="e396e-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="e396e-104">**UnifiedMessagingConfiguration**要素には、ユニファイド メッセージング サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e396e-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="e396e-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="e396e-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e396e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e396e-106">Attributes and elements</span></span>

<span data-ttu-id="e396e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e396e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e396e-108">属性</span><span class="sxs-lookup"><span data-stu-id="e396e-108">Attributes</span></span>

<span data-ttu-id="e396e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e396e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e396e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e396e-110">Child elements</span></span>

|<span data-ttu-id="e396e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e396e-111">**Element**</span></span>|<span data-ttu-id="e396e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e396e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e396e-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="e396e-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="e396e-114">アカウントのユニファイド メッセージングが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e396e-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="e396e-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="e396e-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="e396e-116">PlayOnPhoneDialString (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="e396e-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="e396e-117">電話での再生の電話番号を識別します。</span><span class="sxs-lookup"><span data-stu-id="e396e-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="e396e-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="e396e-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="e396e-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="e396e-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="e396e-120">電話での再生機能が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e396e-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="e396e-121">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="e396e-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e396e-122">親要素</span><span class="sxs-lookup"><span data-stu-id="e396e-122">Parent elements</span></span>

|<span data-ttu-id="e396e-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="e396e-123">**Element**</span></span>|<span data-ttu-id="e396e-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e396e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e396e-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="e396e-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="e396e-126">サービス構成の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e396e-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e396e-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e396e-127">Text value</span></span>

<span data-ttu-id="e396e-128">なし。</span><span class="sxs-lookup"><span data-stu-id="e396e-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e396e-129">備考</span><span class="sxs-lookup"><span data-stu-id="e396e-129">Remarks</span></span>

<span data-ttu-id="e396e-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e396e-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e396e-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="e396e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e396e-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="e396e-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e396e-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e396e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e396e-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e396e-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e396e-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e396e-135">Validation File</span></span>  <br/> |<span data-ttu-id="e396e-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e396e-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e396e-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e396e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e396e-138">False</span><span class="sxs-lookup"><span data-stu-id="e396e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e396e-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="e396e-139">See also</span></span>



- [<span data-ttu-id="e396e-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e396e-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

