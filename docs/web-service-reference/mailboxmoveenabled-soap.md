---
title: MailboxMoveEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73d09137-d3bd-46b3-954a-a358ead07c91
description: MailBoxMoveEnabled 要素は、MailboxMoveEnabled() フラグを表します。 MailBoxMoveEnabled 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 9ba4f49cbd43ab8ca24d9597f69b55c448fd9263
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832292"
---
# <a name="mailboxmoveenabled-soap"></a><span data-ttu-id="c0294-105">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0294-105">MailboxMoveEnabled (SOAP)</span></span>

<span data-ttu-id="c0294-106">**MailBoxMoveEnabled**要素は、 **MailboxMoveEnabled()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="c0294-106">The **MailBoxMoveEnabled** element represents the **MailboxMoveEnabled()** flag.</span></span> <span data-ttu-id="c0294-107">**MailBoxMoveEnabled**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="c0294-107">The **MailBoxMoveEnabled** element is for internal use only.</span></span> <span data-ttu-id="c0294-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="c0294-108">This element is not used by clients.</span></span> 
  
```XML
<MailBoxMoveEnabled>true | false</MailBoxMoveEnabled>
```

<span data-ttu-id="c0294-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c0294-109">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c0294-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c0294-110">Attributes and elements</span></span>

<span data-ttu-id="c0294-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0294-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0294-112">属性</span><span class="sxs-lookup"><span data-stu-id="c0294-112">Attributes</span></span>

<span data-ttu-id="c0294-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c0294-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0294-114">子要素</span><span class="sxs-lookup"><span data-stu-id="c0294-114">Child elements</span></span>

<span data-ttu-id="c0294-115">なし。</span><span class="sxs-lookup"><span data-stu-id="c0294-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0294-116">親要素</span><span class="sxs-lookup"><span data-stu-id="c0294-116">Parent elements</span></span>

|<span data-ttu-id="c0294-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0294-117">**Element**</span></span>|<span data-ttu-id="c0294-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0294-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0294-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0294-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="c0294-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="c0294-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c0294-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="c0294-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0294-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="c0294-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c0294-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0294-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c0294-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="c0294-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c0294-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0294-125">Validation File</span></span>  <br/> |<span data-ttu-id="c0294-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0294-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0294-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c0294-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0294-128">True</span><span class="sxs-lookup"><span data-stu-id="c0294-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0294-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0294-129">See also</span></span>

- [<span data-ttu-id="c0294-130">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0294-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

