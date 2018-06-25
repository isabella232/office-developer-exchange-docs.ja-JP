---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: DelegationState 要素では、委任されたタスクのステータスを表します。
ms.openlocfilehash: 00b0e41ae223f1c70f9a3a21662e8858f8690a86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759956"
---
# <a name="delegationstate"></a><span data-ttu-id="05a2e-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="05a2e-103">DelegationState</span></span>

<span data-ttu-id="05a2e-104">**DelegationState**要素では、委任されたタスクのステータスを表します。</span><span class="sxs-lookup"><span data-stu-id="05a2e-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="05a2e-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="05a2e-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="05a2e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="05a2e-106">Attributes and elements</span></span>

<span data-ttu-id="05a2e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05a2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05a2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="05a2e-108">Attributes</span></span>

<span data-ttu-id="05a2e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05a2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05a2e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05a2e-110">Child elements</span></span>

<span data-ttu-id="05a2e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="05a2e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05a2e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="05a2e-112">Parent elements</span></span>

|<span data-ttu-id="05a2e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="05a2e-113">**Element**</span></span>|<span data-ttu-id="05a2e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="05a2e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05a2e-115">タスク</span><span class="sxs-lookup"><span data-stu-id="05a2e-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="05a2e-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="05a2e-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05a2e-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05a2e-117">Text value</span></span>

<span data-ttu-id="05a2e-118">これは、プロパティは読み取り専用プロパティです。</span><span class="sxs-lookup"><span data-stu-id="05a2e-118">This is a read-only property.</span></span> <span data-ttu-id="05a2e-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="05a2e-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="05a2e-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="05a2e-120">NoMatch</span></span>
    
- <span data-ttu-id="05a2e-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="05a2e-121">OwnNew</span></span>
    
- <span data-ttu-id="05a2e-122">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="05a2e-122">Owned</span></span>
    
- <span data-ttu-id="05a2e-123">了承済み</span><span class="sxs-lookup"><span data-stu-id="05a2e-123">Accepted</span></span>
    
- <span data-ttu-id="05a2e-124">辞退</span><span class="sxs-lookup"><span data-stu-id="05a2e-124">Declined</span></span>
    
- <span data-ttu-id="05a2e-125">Max</span><span class="sxs-lookup"><span data-stu-id="05a2e-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="05a2e-126">備考</span><span class="sxs-lookup"><span data-stu-id="05a2e-126">Remarks</span></span>

<span data-ttu-id="05a2e-127">Microsoft Exchange Server 2007 で Exchange Web サービスでは、タスクの割り当てをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="05a2e-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="05a2e-128">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="05a2e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05a2e-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="05a2e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05a2e-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="05a2e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05a2e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05a2e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="05a2e-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="05a2e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="05a2e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05a2e-133">Validation File</span></span>  <br/> |<span data-ttu-id="05a2e-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05a2e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05a2e-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="05a2e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="05a2e-136">False</span><span class="sxs-lookup"><span data-stu-id="05a2e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05a2e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="05a2e-137">See also</span></span>

- [<span data-ttu-id="05a2e-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="05a2e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

