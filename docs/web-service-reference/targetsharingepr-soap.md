---
title: TargetSharingEpr (SOAP)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0115a740-9264-4e57-a410-197bb39e6c81
description: TargetSharingEpr 要素は、TargetSharingEpr プロパティを表します。 TargetSharingEpr 要素は、内部使用のみを対象としています。
ms.openlocfilehash: 8cb8d114ae43dfc8ad76aebe87e0e920c16477f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457082"
---
# <a name="targetsharingepr-soap"></a><span data-ttu-id="785e7-104">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="785e7-104">TargetSharingEpr (SOAP)</span></span>
 
<span data-ttu-id="785e7-105">**Targetsharingepr**要素は、 **targetsharingepr**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="785e7-105">The **TargetSharingEpr** element represents the **TargetSharingEpr** property.</span></span> <span data-ttu-id="785e7-106">**Targetsharingepr**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="785e7-106">The **TargetSharingEpr** element is for internal use only.</span></span> <span data-ttu-id="785e7-107">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="785e7-107">This element is not used by clients.</span></span> 
  
```XML
<TargetSharingEpr/>
```

<span data-ttu-id="785e7-108">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="785e7-108">**anyURI**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="785e7-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="785e7-109">Attributes and elements</span></span>

<span data-ttu-id="785e7-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="785e7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="785e7-111">属性</span><span class="sxs-lookup"><span data-stu-id="785e7-111">Attributes</span></span>

<span data-ttu-id="785e7-112">なし。</span><span class="sxs-lookup"><span data-stu-id="785e7-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="785e7-113">子要素</span><span class="sxs-lookup"><span data-stu-id="785e7-113">Child elements</span></span>

<span data-ttu-id="785e7-114">なし。</span><span class="sxs-lookup"><span data-stu-id="785e7-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="785e7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="785e7-115">Parent elements</span></span>

|<span data-ttu-id="785e7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="785e7-116">**Element**</span></span>|<span data-ttu-id="785e7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="785e7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="785e7-118">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="785e7-118">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="785e7-119">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="785e7-119">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="785e7-120">注釈</span><span class="sxs-lookup"><span data-stu-id="785e7-120">Remarks</span></span>

<span data-ttu-id="785e7-121">この要素は、外部組織のターゲットサーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="785e7-121">This element specifies the URL of the target server for the external organization.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="785e7-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="785e7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="785e7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="785e7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="785e7-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="785e7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="785e7-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="785e7-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="785e7-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="785e7-126">Validation File</span></span>  <br/> |<span data-ttu-id="785e7-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="785e7-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="785e7-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="785e7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="785e7-129">正しい</span><span class="sxs-lookup"><span data-stu-id="785e7-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="785e7-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="785e7-130">See also</span></span>

- [<span data-ttu-id="785e7-131">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="785e7-131">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

