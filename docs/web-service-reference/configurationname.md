---
title: ConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: ConfigurationName 要素は、名前によって要求されたサービスの構成を指定します。
ms.openlocfilehash: a03a0bc0ab7ecbc1c2aec31f864503ee0f560908
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759651"
---
# <a name="configurationname"></a><span data-ttu-id="a4c55-103">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="a4c55-103">ConfigurationName</span></span>

<span data-ttu-id="a4c55-104">**ConfigurationName**要素は、名前によって要求されたサービスの構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="a4c55-105">**ServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="a4c55-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4c55-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4c55-106">Attributes and elements</span></span>

<span data-ttu-id="a4c55-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4c55-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4c55-108">Attributes</span></span>

<span data-ttu-id="a4c55-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4c55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4c55-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4c55-110">Child elements</span></span>

<span data-ttu-id="a4c55-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a4c55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4c55-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a4c55-112">Parent elements</span></span>

|<span data-ttu-id="a4c55-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4c55-113">**Element**</span></span>|<span data-ttu-id="a4c55-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4c55-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4c55-115">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4c55-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="a4c55-116">要求されたサービスの構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4c55-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4c55-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4c55-117">Text value</span></span>

<span data-ttu-id="a4c55-118">**ConfigurationName**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="a4c55-119">**ConfigurationName 要素の値**</span><span class="sxs-lookup"><span data-stu-id="a4c55-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="a4c55-120">**値**</span><span class="sxs-lookup"><span data-stu-id="a4c55-120">**Value**</span></span>|<span data-ttu-id="a4c55-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4c55-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a4c55-122">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="a4c55-122">MailTips</span></span>  <br/> |<span data-ttu-id="a4c55-123">メール ヒント サービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="a4c55-124">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4c55-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="a4c55-125">ユニファイド メッセージング サービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="a4c55-126">ProtectionRules</span><span class="sxs-lookup"><span data-stu-id="a4c55-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="a4c55-127">保護ルールのサービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="a4c55-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a4c55-128">備考</span><span class="sxs-lookup"><span data-stu-id="a4c55-128">Remarks</span></span>

<span data-ttu-id="a4c55-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4c55-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4c55-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4c55-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4c55-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4c55-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4c55-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4c55-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a4c55-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a4c55-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4c55-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4c55-134">Validation File</span></span>  <br/> |<span data-ttu-id="a4c55-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4c55-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4c55-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4c55-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4c55-137">False</span><span class="sxs-lookup"><span data-stu-id="a4c55-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4c55-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4c55-138">See also</span></span>



- [<span data-ttu-id="a4c55-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4c55-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

