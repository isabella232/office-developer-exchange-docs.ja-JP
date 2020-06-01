---
title: Mailヒント Accesslevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 730e349e-8250-4236-af53-cd9039c74d8f
description: Mailヒント Accesslevel 要素は、Mailヒント Accesslevel プロパティを表します。 Mailヒント Accesslevel 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 8e3a467f7aa8484fc8a4bfb23f8b4ac4c138ccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458069"
---
# <a name="mailtipsaccesslevel-soap"></a><span data-ttu-id="b8a5a-105">Mailヒント Accesslevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b8a5a-105">MailTipsAccessLevel (SOAP)</span></span>

<span data-ttu-id="b8a5a-106">**Mailヒント accesslevel**要素は、 **mailヒント accesslevel**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-106">The **MailTipsAccessLevel** element represents the **MailTipsAccessLevel** property.</span></span> <span data-ttu-id="b8a5a-107">**Mailヒント Accesslevel**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-107">The **MailTipsAccessLevel** element is for internal use only.</span></span> <span data-ttu-id="b8a5a-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-108">This element is not used by clients.</span></span> 
  
```XML
<MailTipsAccessLevel/>
```

 <span data-ttu-id="b8a5a-109">**string**</span><span class="sxs-lookup"><span data-stu-id="b8a5a-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8a5a-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8a5a-110">Attributes and elements</span></span>

<span data-ttu-id="b8a5a-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8a5a-112">属性</span><span class="sxs-lookup"><span data-stu-id="b8a5a-112">Attributes</span></span>

<span data-ttu-id="b8a5a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8a5a-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b8a5a-114">Child elements</span></span>

<span data-ttu-id="b8a5a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8a5a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b8a5a-116">Parent elements</span></span>

|<span data-ttu-id="b8a5a-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8a5a-117">**Element**</span></span>|<span data-ttu-id="b8a5a-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8a5a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a5a-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b8a5a-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="b8a5a-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8a5a-121">注釈</span><span class="sxs-lookup"><span data-stu-id="b8a5a-121">Remarks</span></span>

<span data-ttu-id="b8a5a-122">この要素は、応答で返されるメールヒントの詳細の最大量を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8a5a-122">This element specifies the maximum amount of mail tips detail that will be returned in the response.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8a5a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8a5a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8a5a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8a5a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b8a5a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8a5a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b8a5a-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="b8a5a-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b8a5a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8a5a-127">Validation File</span></span>  <br/> |<span data-ttu-id="b8a5a-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b8a5a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8a5a-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b8a5a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8a5a-130">正しい</span><span class="sxs-lookup"><span data-stu-id="b8a5a-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8a5a-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8a5a-131">See also</span></span>



[<span data-ttu-id="b8a5a-132">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b8a5a-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

