---
title: MailTipsAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 730e349e-8250-4236-af53-cd9039c74d8f
description: MailTipsAccessLevel 要素は、MailTipsAccessLevel プロパティを表します。 MailTipsAccessLevel 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 35fb4aa56bbfa42ac4be196a379dc48aff5ec101
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832313"
---
# <a name="mailtipsaccesslevel-soap"></a><span data-ttu-id="33858-105">MailTipsAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33858-105">MailTipsAccessLevel (SOAP)</span></span>

<span data-ttu-id="33858-106">**MailTipsAccessLevel**要素は、 **MailTipsAccessLevel**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="33858-106">The **MailTipsAccessLevel** element represents the **MailTipsAccessLevel** property.</span></span> <span data-ttu-id="33858-107">**MailTipsAccessLevel**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="33858-107">The **MailTipsAccessLevel** element is for internal use only.</span></span> <span data-ttu-id="33858-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="33858-108">This element is not used by clients.</span></span> 
  
```XML
<MailTipsAccessLevel/>
```

 <span data-ttu-id="33858-109">**string**</span><span class="sxs-lookup"><span data-stu-id="33858-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33858-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="33858-110">Attributes and elements</span></span>

<span data-ttu-id="33858-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33858-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33858-112">属性</span><span class="sxs-lookup"><span data-stu-id="33858-112">Attributes</span></span>

<span data-ttu-id="33858-113">なし。</span><span class="sxs-lookup"><span data-stu-id="33858-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33858-114">子要素</span><span class="sxs-lookup"><span data-stu-id="33858-114">Child elements</span></span>

<span data-ttu-id="33858-115">なし。</span><span class="sxs-lookup"><span data-stu-id="33858-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33858-116">親要素</span><span class="sxs-lookup"><span data-stu-id="33858-116">Parent elements</span></span>

|<span data-ttu-id="33858-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="33858-117">**Element**</span></span>|<span data-ttu-id="33858-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="33858-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33858-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33858-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="33858-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="33858-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33858-121">備考</span><span class="sxs-lookup"><span data-stu-id="33858-121">Remarks</span></span>

<span data-ttu-id="33858-122">この要素は、応答で返されるメール ヒントの詳細情報の最大量を指定します。</span><span class="sxs-lookup"><span data-stu-id="33858-122">This element specifies the maximum amount of mail tips detail that will be returned in the response.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33858-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="33858-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33858-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="33858-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="33858-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33858-125">Schema Name</span></span>  <br/> |<span data-ttu-id="33858-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="33858-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="33858-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33858-127">Validation File</span></span>  <br/> |<span data-ttu-id="33858-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33858-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33858-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="33858-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="33858-130">True</span><span class="sxs-lookup"><span data-stu-id="33858-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33858-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="33858-131">See also</span></span>



[<span data-ttu-id="33858-132">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33858-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

