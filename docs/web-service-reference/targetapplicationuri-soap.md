---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: TargetApplicationUri 要素は、ターゲットアプリケーション URI を定義します。 TargetApplicationUri 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 88968aac604b77cd057dbc69c396227a489ac9a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457089"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="d2e12-105">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e12-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="d2e12-106">**Targetapplicationuri**要素は、ターゲットアプリケーション uri を定義します。</span><span class="sxs-lookup"><span data-stu-id="d2e12-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="d2e12-107">**Targetapplicationuri**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="d2e12-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="d2e12-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="d2e12-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="d2e12-109">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="d2e12-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2e12-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2e12-110">Attributes and elements</span></span>

<span data-ttu-id="d2e12-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2e12-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2e12-112">属性</span><span class="sxs-lookup"><span data-stu-id="d2e12-112">Attributes</span></span>

<span data-ttu-id="d2e12-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d2e12-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2e12-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d2e12-114">Child elements</span></span>

<span data-ttu-id="d2e12-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d2e12-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2e12-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d2e12-116">Parent elements</span></span>

|<span data-ttu-id="d2e12-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2e12-117">**Element**</span></span>|<span data-ttu-id="d2e12-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2e12-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2e12-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e12-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="d2e12-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="d2e12-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2e12-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d2e12-121">Remarks</span></span>

<span data-ttu-id="d2e12-122">この要素は、外部組織のターゲット URI を定義します。</span><span class="sxs-lookup"><span data-stu-id="d2e12-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2e12-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2e12-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2e12-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2e12-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d2e12-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2e12-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d2e12-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d2e12-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d2e12-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2e12-127">Validation File</span></span>  <br/> |<span data-ttu-id="d2e12-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d2e12-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2e12-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d2e12-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2e12-130">正しい</span><span class="sxs-lookup"><span data-stu-id="d2e12-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2e12-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2e12-131">See also</span></span>



[<span data-ttu-id="d2e12-132">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2e12-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

