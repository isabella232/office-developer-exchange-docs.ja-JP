---
title: ProtectionRulesConfiguration
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
description: ProtectionRulesConfiguration 要素には、保護ルールのサービスのサービスの構成情報が含まれています。
ms.openlocfilehash: 9c286fcf9752d591d53323f45a264f4bdd078c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832912"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="bda2b-103">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="bda2b-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="bda2b-104">**ProtectionRulesConfiguration**要素には、保護ルールのサービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bda2b-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="bda2b-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="bda2b-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bda2b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bda2b-106">Attributes and elements</span></span>

<span data-ttu-id="bda2b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bda2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bda2b-108">属性</span><span class="sxs-lookup"><span data-stu-id="bda2b-108">Attributes</span></span>

|<span data-ttu-id="bda2b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="bda2b-109">**Attribute**</span></span>|<span data-ttu-id="bda2b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="bda2b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bda2b-111">**間隔**</span><span class="sxs-lookup"><span data-stu-id="bda2b-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="bda2b-112">どのくらいの頻度、時間の単位でクライアントする必要があります保護規則サーバーからの要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="bda2b-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="bda2b-113">この属性は必須であり、その値は 1 以上の整数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="bda2b-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bda2b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="bda2b-114">Child elements</span></span>

|<span data-ttu-id="bda2b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="bda2b-115">**Element**</span></span>|<span data-ttu-id="bda2b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="bda2b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bda2b-117">ルール</span><span class="sxs-lookup"><span data-stu-id="bda2b-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bda2b-118">保護規則の配列。</span><span class="sxs-lookup"><span data-stu-id="bda2b-118">An array of protection rules.</span></span> <span data-ttu-id="bda2b-119">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="bda2b-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="bda2b-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="bda2b-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="bda2b-121">組織の内部の SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="bda2b-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="bda2b-122">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="bda2b-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bda2b-123">親要素</span><span class="sxs-lookup"><span data-stu-id="bda2b-123">Parent elements</span></span>

|<span data-ttu-id="bda2b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="bda2b-124">**Element**</span></span>|<span data-ttu-id="bda2b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="bda2b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bda2b-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="bda2b-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="bda2b-127">サービス構成の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bda2b-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bda2b-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bda2b-128">Text value</span></span>

<span data-ttu-id="bda2b-129">なし。</span><span class="sxs-lookup"><span data-stu-id="bda2b-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bda2b-130">備考</span><span class="sxs-lookup"><span data-stu-id="bda2b-130">Remarks</span></span>

<span data-ttu-id="bda2b-131">保護ルールのサービスの構成は、ルール、内部ドメイン、および更新間隔の一覧で構成されます。</span><span class="sxs-lookup"><span data-stu-id="bda2b-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="bda2b-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bda2b-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bda2b-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="bda2b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bda2b-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="bda2b-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bda2b-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bda2b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bda2b-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bda2b-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bda2b-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bda2b-137">Validation File</span></span>  <br/> |<span data-ttu-id="bda2b-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bda2b-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bda2b-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bda2b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="bda2b-140">False</span><span class="sxs-lookup"><span data-stu-id="bda2b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bda2b-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="bda2b-141">See also</span></span>



- [<span data-ttu-id="bda2b-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bda2b-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

