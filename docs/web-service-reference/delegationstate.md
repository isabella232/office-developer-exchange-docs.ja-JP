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
description: Taskitem.delegationstate 要素は、委任されたタスクの状態を表します。
ms.openlocfilehash: b938b5a2240283c265006dd47cd6ff475ad80978
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457369"
---
# <a name="delegationstate"></a><span data-ttu-id="6781d-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="6781d-103">DelegationState</span></span>

<span data-ttu-id="6781d-104">**Taskitem.delegationstate**要素は、委任されたタスクの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="6781d-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="6781d-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="6781d-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6781d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6781d-106">Attributes and elements</span></span>

<span data-ttu-id="6781d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6781d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6781d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6781d-108">Attributes</span></span>

<span data-ttu-id="6781d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6781d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6781d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6781d-110">Child elements</span></span>

<span data-ttu-id="6781d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6781d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6781d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6781d-112">Parent elements</span></span>

|<span data-ttu-id="6781d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6781d-113">**Element**</span></span>|<span data-ttu-id="6781d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6781d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6781d-115">Task</span><span class="sxs-lookup"><span data-stu-id="6781d-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="6781d-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="6781d-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6781d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6781d-117">Text value</span></span>

<span data-ttu-id="6781d-118">これは読み取り専用のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="6781d-118">This is a read-only property.</span></span> <span data-ttu-id="6781d-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6781d-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="6781d-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="6781d-120">NoMatch</span></span>
    
- <span data-ttu-id="6781d-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="6781d-121">OwnNew</span></span>
    
- <span data-ttu-id="6781d-122">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="6781d-122">Owned</span></span>
    
- <span data-ttu-id="6781d-123">Accepted</span><span class="sxs-lookup"><span data-stu-id="6781d-123">Accepted</span></span>
    
- <span data-ttu-id="6781d-124">同意</span><span class="sxs-lookup"><span data-stu-id="6781d-124">Declined</span></span>
    
- <span data-ttu-id="6781d-125">Max</span><span class="sxs-lookup"><span data-stu-id="6781d-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6781d-126">注釈</span><span class="sxs-lookup"><span data-stu-id="6781d-126">Remarks</span></span>

<span data-ttu-id="6781d-127">Microsoft Exchange Server 2007 の exchange Web サービスは、タスク割り当てをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="6781d-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="6781d-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6781d-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6781d-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6781d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6781d-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6781d-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6781d-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6781d-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6781d-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6781d-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6781d-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6781d-133">Validation File</span></span>  <br/> |<span data-ttu-id="6781d-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6781d-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6781d-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6781d-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6781d-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6781d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6781d-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6781d-137">See also</span></span>

- [<span data-ttu-id="6781d-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6781d-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

