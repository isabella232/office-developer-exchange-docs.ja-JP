---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: AlternateMailbox 要素は、代替メールボックスを表します。
ms.openlocfilehash: 9019f85a373cc186cc9dadddceee3dc9d11b3854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466158"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="9a459-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="9a459-104">**AlternateMailbox**要素は、代替メールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="9a459-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="9a459-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a459-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9a459-106">Attributes and elements</span></span>

<span data-ttu-id="9a459-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a459-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a459-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a459-108">Attributes</span></span>

<span data-ttu-id="9a459-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9a459-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a459-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9a459-110">Child elements</span></span>

|<span data-ttu-id="9a459-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9a459-111">**Element**</span></span>|<span data-ttu-id="9a459-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a459-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a459-113">Type (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="9a459-114">代替メールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="9a459-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="9a459-116">代替メールボックスの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="9a459-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="9a459-118">代替メールボックスの従来の識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="9a459-119">サーバー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="9a459-120">代替メールボックスサーバーを表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="9a459-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="9a459-122">代替メールボックス SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a459-123">親要素</span><span class="sxs-lookup"><span data-stu-id="9a459-123">Parent elements</span></span>

|<span data-ttu-id="9a459-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a459-124">**Element**</span></span>|<span data-ttu-id="9a459-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a459-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a459-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="9a459-127">代替メールボックスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="9a459-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a459-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9a459-128">Text value</span></span>

<span data-ttu-id="9a459-129">なし。</span><span class="sxs-lookup"><span data-stu-id="9a459-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a459-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9a459-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a459-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a459-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9a459-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a459-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9a459-133">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="9a459-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9a459-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a459-134">Validation File</span></span>  <br/> |<span data-ttu-id="9a459-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9a459-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a459-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9a459-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a459-137">正しい</span><span class="sxs-lookup"><span data-stu-id="9a459-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a459-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a459-138">See also</span></span>

- [<span data-ttu-id="9a459-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a459-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

