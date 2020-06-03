---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: InternalDomains 要素は、組織の内部 SMTP ドメインのリストを識別します。
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459967"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="3bc43-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="3bc43-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="3bc43-104">**Internaldomains**要素は、組織の内部 SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="3bc43-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="3bc43-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="3bc43-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bc43-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3bc43-106">Attributes and elements</span></span>

<span data-ttu-id="3bc43-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3bc43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bc43-108">属性</span><span class="sxs-lookup"><span data-stu-id="3bc43-108">Attributes</span></span>

<span data-ttu-id="3bc43-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3bc43-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bc43-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3bc43-110">Child elements</span></span>

|<span data-ttu-id="3bc43-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3bc43-111">**Element**</span></span>|<span data-ttu-id="3bc43-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3bc43-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bc43-113">ドメイン</span><span class="sxs-lookup"><span data-stu-id="3bc43-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="3bc43-114">単一の SMTP ドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="3bc43-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bc43-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3bc43-115">Parent elements</span></span>

|<span data-ttu-id="3bc43-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3bc43-116">**Element**</span></span>|<span data-ttu-id="3bc43-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3bc43-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bc43-118">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="3bc43-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="3bc43-119">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="3bc43-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="3bc43-120">Protectionルールの構成</span><span class="sxs-lookup"><span data-stu-id="3bc43-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="3bc43-121">保護ルールサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="3bc43-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3bc43-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3bc43-122">Text value</span></span>

<span data-ttu-id="3bc43-123">なし。</span><span class="sxs-lookup"><span data-stu-id="3bc43-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3bc43-124">注釈</span><span class="sxs-lookup"><span data-stu-id="3bc43-124">Remarks</span></span>

<span data-ttu-id="3bc43-125">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="3bc43-125">This element is required.</span></span> 
  
<span data-ttu-id="3bc43-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3bc43-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bc43-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3bc43-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bc43-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3bc43-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3bc43-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3bc43-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3bc43-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3bc43-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3bc43-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3bc43-131">Validation File</span></span>  <br/> |<span data-ttu-id="3bc43-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3bc43-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3bc43-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3bc43-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3bc43-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="3bc43-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bc43-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="3bc43-135">See also</span></span>



- [<span data-ttu-id="3bc43-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3bc43-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

