---
title: Protectionルールの構成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: Protectionrules 構成要素には、保護ルールサービスのサービス構成情報が含まれています。
ms.openlocfilehash: e664fba78f170c9f4c59b49b3a08c0dd2e4ed4cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456770"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="d81dc-103">Protectionルールの構成</span><span class="sxs-lookup"><span data-stu-id="d81dc-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="d81dc-104">**Protectionrules 構成**要素には、保護ルールサービスのサービス構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d81dc-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="d81dc-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="d81dc-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d81dc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d81dc-106">Attributes and elements</span></span>

<span data-ttu-id="d81dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d81dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d81dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d81dc-108">Attributes</span></span>

|<span data-ttu-id="d81dc-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d81dc-109">**Attribute**</span></span>|<span data-ttu-id="d81dc-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d81dc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d81dc-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="d81dc-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="d81dc-112">クライアントがサーバーに保護ルールを要求する頻度 (時間単位) を指定します。</span><span class="sxs-lookup"><span data-stu-id="d81dc-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="d81dc-113">この属性は必須であり、その値は1以上の整数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d81dc-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d81dc-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d81dc-114">Child elements</span></span>

|<span data-ttu-id="d81dc-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="d81dc-115">**Element**</span></span>|<span data-ttu-id="d81dc-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d81dc-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d81dc-117">ルール</span><span class="sxs-lookup"><span data-stu-id="d81dc-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d81dc-118">保護ルールの配列。</span><span class="sxs-lookup"><span data-stu-id="d81dc-118">An array of protection rules.</span></span> <span data-ttu-id="d81dc-119">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="d81dc-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d81dc-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="d81dc-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="d81dc-121">組織の内部 SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="d81dc-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="d81dc-122">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="d81dc-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d81dc-123">親要素</span><span class="sxs-lookup"><span data-stu-id="d81dc-123">Parent elements</span></span>

|<span data-ttu-id="d81dc-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="d81dc-124">**Element**</span></span>|<span data-ttu-id="d81dc-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="d81dc-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d81dc-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="d81dc-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="d81dc-127">サービス構成の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d81dc-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d81dc-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d81dc-128">Text value</span></span>

<span data-ttu-id="d81dc-129">なし。</span><span class="sxs-lookup"><span data-stu-id="d81dc-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d81dc-130">注釈</span><span class="sxs-lookup"><span data-stu-id="d81dc-130">Remarks</span></span>

<span data-ttu-id="d81dc-131">保護ルールサービスの構成は、ルール、内部ドメイン、および更新間隔のリストで構成されます。</span><span class="sxs-lookup"><span data-stu-id="d81dc-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="d81dc-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d81dc-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d81dc-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d81dc-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d81dc-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="d81dc-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d81dc-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d81dc-135">Schema Name</span></span>  <br/> |<span data-ttu-id="d81dc-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d81dc-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d81dc-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d81dc-137">Validation File</span></span>  <br/> |<span data-ttu-id="d81dc-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d81dc-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d81dc-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d81dc-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="d81dc-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="d81dc-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d81dc-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="d81dc-141">See also</span></span>



- [<span data-ttu-id="d81dc-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d81dc-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

