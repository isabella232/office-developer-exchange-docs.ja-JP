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
description: AlternateMailbox 要素は、別のメールボックスを表します。
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19759367"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="6e14b-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="6e14b-104">**AlternateMailbox**要素は、別のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="6e14b-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="6e14b-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e14b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6e14b-106">Attributes and elements</span></span>

<span data-ttu-id="6e14b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e14b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e14b-108">Attributes</span></span>

<span data-ttu-id="6e14b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6e14b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e14b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6e14b-110">Child elements</span></span>

|<span data-ttu-id="6e14b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e14b-111">**Element**</span></span>|<span data-ttu-id="6e14b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e14b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e14b-113">(SOAP) の種類</span><span class="sxs-lookup"><span data-stu-id="6e14b-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="6e14b-114">代替メールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="6e14b-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="6e14b-116">代替メールボックスの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="6e14b-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="6e14b-118">代替メールボックスの従来の識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="6e14b-119">サーバー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="6e14b-120">代替メールボックス サーバーを表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="6e14b-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="6e14b-122">代替メールボックスの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e14b-123">親要素</span><span class="sxs-lookup"><span data-stu-id="6e14b-123">Parent elements</span></span>

|<span data-ttu-id="6e14b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e14b-124">**Element**</span></span>|<span data-ttu-id="6e14b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e14b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e14b-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="6e14b-127">メールボックスを別のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6e14b-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e14b-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6e14b-128">Text value</span></span>

<span data-ttu-id="6e14b-129">なし。</span><span class="sxs-lookup"><span data-stu-id="6e14b-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e14b-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="6e14b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e14b-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="6e14b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6e14b-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e14b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6e14b-133">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="6e14b-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6e14b-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e14b-134">Validation File</span></span>  <br/> |<span data-ttu-id="6e14b-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e14b-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e14b-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6e14b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e14b-137">True</span><span class="sxs-lookup"><span data-stu-id="6e14b-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e14b-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e14b-138">See also</span></span>

- [<span data-ttu-id="6e14b-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e14b-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

