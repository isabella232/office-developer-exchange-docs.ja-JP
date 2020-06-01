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
description: ConfigurationName 要素は、要求されたサービス構成を名前で指定します。
ms.openlocfilehash: 5e1216253a633af643dbd276827842dbe2db5d5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463924"
---
# <a name="configurationname"></a><span data-ttu-id="64b9c-103">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="64b9c-103">ConfigurationName</span></span>

<span data-ttu-id="64b9c-104">**ConfigurationName**要素は、要求されたサービス構成を名前で指定します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="64b9c-105">**ServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="64b9c-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64b9c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64b9c-106">Attributes and elements</span></span>

<span data-ttu-id="64b9c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64b9c-108">属性</span><span class="sxs-lookup"><span data-stu-id="64b9c-108">Attributes</span></span>

<span data-ttu-id="64b9c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="64b9c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64b9c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="64b9c-110">Child elements</span></span>

<span data-ttu-id="64b9c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="64b9c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64b9c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="64b9c-112">Parent elements</span></span>

|<span data-ttu-id="64b9c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="64b9c-113">**Element**</span></span>|<span data-ttu-id="64b9c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="64b9c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64b9c-115">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="64b9c-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="64b9c-116">要求されたサービス構成を含みます。</span><span class="sxs-lookup"><span data-stu-id="64b9c-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64b9c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="64b9c-117">Text value</span></span>

<span data-ttu-id="64b9c-118">次の表に、 **ConfigurationName**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="64b9c-119">**ConfigurationName 要素の値**</span><span class="sxs-lookup"><span data-stu-id="64b9c-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="64b9c-120">**値**</span><span class="sxs-lookup"><span data-stu-id="64b9c-120">**Value**</span></span>|<span data-ttu-id="64b9c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="64b9c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64b9c-122">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="64b9c-122">MailTips</span></span>  <br/> |<span data-ttu-id="64b9c-123">メールヒントサービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="64b9c-124">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="64b9c-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="64b9c-125">ユニファイドメッセージングサービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="64b9c-126">ProtectionRules</span><span class="sxs-lookup"><span data-stu-id="64b9c-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="64b9c-127">保護ルールサービスの構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="64b9c-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64b9c-128">注釈</span><span class="sxs-lookup"><span data-stu-id="64b9c-128">Remarks</span></span>

<span data-ttu-id="64b9c-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="64b9c-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64b9c-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="64b9c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64b9c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="64b9c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="64b9c-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64b9c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="64b9c-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="64b9c-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="64b9c-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64b9c-134">Validation File</span></span>  <br/> |<span data-ttu-id="64b9c-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="64b9c-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="64b9c-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="64b9c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="64b9c-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="64b9c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64b9c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="64b9c-138">See also</span></span>



- [<span data-ttu-id="64b9c-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="64b9c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

