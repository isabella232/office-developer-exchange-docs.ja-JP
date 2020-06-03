---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: LegacyDN 要素は、ユーザーのメールボックスを従来の識別名で識別します。
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526383"
---
# <a name="legacydn-pox"></a><span data-ttu-id="8b0d8-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="8b0d8-103">LegacyDN (POX)</span></span>

<span data-ttu-id="8b0d8-104">**LegacyDN**要素は、ユーザーのメールボックスを従来の識別名で識別します。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8b0d8-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8b0d8-105">Attributes and elements</span></span>

<span data-ttu-id="8b0d8-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b0d8-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b0d8-107">Attributes</span></span>

<span data-ttu-id="8b0d8-108">なし。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b0d8-109">子要素</span><span class="sxs-lookup"><span data-stu-id="8b0d8-109">Child elements</span></span>

<span data-ttu-id="8b0d8-110">なし。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b0d8-111">親要素</span><span class="sxs-lookup"><span data-stu-id="8b0d8-111">Parent elements</span></span>

|<span data-ttu-id="8b0d8-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="8b0d8-112">**Element**</span></span>|<span data-ttu-id="8b0d8-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="8b0d8-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b0d8-114">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="8b0d8-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="8b0d8-115">自動検出サービスへの要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="8b0d8-116">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="8b0d8-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="8b0d8-117">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b0d8-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8b0d8-118">Text value</span></span>

<span data-ttu-id="8b0d8-119">テキスト値は、ユーザーの従来の電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b0d8-120">注釈</span><span class="sxs-lookup"><span data-stu-id="8b0d8-120">Remarks</span></span>

<span data-ttu-id="8b0d8-121">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素は、自動検出要求の代替要素です。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="8b0d8-122">これは、Microsoft Exchange Server 2007 を実行しているコンピューター上にメールボックスが存在する場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="8b0d8-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8b0d8-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="8b0d8-123">See also</span></span>

- [<span data-ttu-id="8b0d8-124">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="8b0d8-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

