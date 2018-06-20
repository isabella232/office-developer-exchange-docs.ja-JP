---
title: (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: 要素は、すべての子要素と一致するが true に評価するを指定します。
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759321"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="a9d1e-103">(ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="a9d1e-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="a9d1e-104">**および**要素は、すべての子要素と一致するが**true**と評価されるを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="a9d1e-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9d1e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a9d1e-106">Attributes and elements</span></span>

<span data-ttu-id="a9d1e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9d1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9d1e-108">Attributes</span></span>

<span data-ttu-id="a9d1e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9d1e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a9d1e-110">Child elements</span></span>

|<span data-ttu-id="a9d1e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-111">**Element**</span></span>|<span data-ttu-id="a9d1e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9d1e-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="a9d1e-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="a9d1e-114">電子メール メッセージのすべての受信者が送信者の組織の内部場合は、 **true**に評価されます。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="a9d1e-115">**And**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-115">**And**</span></span> <br/> |<span data-ttu-id="a9d1e-116">すべての子要素と一致するが**true**と評価されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="a9d1e-117">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="a9d1e-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="a9d1e-118">電子メール メッセージの受信者と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定した受信者のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a9d1e-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="a9d1e-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="a9d1e-120">送信者の部署と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定された部門のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a9d1e-121">True</span><span class="sxs-lookup"><span data-stu-id="a9d1e-121">True</span></span>](true.md) <br/> |<span data-ttu-id="a9d1e-122">常に一致する条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9d1e-123">親要素</span><span class="sxs-lookup"><span data-stu-id="a9d1e-123">Parent elements</span></span>

|<span data-ttu-id="a9d1e-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-124">**Element**</span></span>|<span data-ttu-id="a9d1e-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9d1e-126">条件</span><span class="sxs-lookup"><span data-stu-id="a9d1e-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="a9d1e-127">実行するルールのアクション部の満たされている必要がある条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="a9d1e-128">**And**</span><span class="sxs-lookup"><span data-stu-id="a9d1e-128">**And**</span></span> <br/> |<span data-ttu-id="a9d1e-129">すべての子要素と一致するが**true**と評価されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9d1e-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a9d1e-130">Text value</span></span>

<span data-ttu-id="a9d1e-131">なし。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a9d1e-132">備考</span><span class="sxs-lookup"><span data-stu-id="a9d1e-132">Remarks</span></span>

<span data-ttu-id="a9d1e-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a9d1e-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9d1e-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="a9d1e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9d1e-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="a9d1e-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9d1e-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a9d1e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="a9d1e-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a9d1e-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9d1e-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a9d1e-138">Validation File</span></span>  <br/> |<span data-ttu-id="a9d1e-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a9d1e-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9d1e-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a9d1e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9d1e-141">False</span><span class="sxs-lookup"><span data-stu-id="a9d1e-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9d1e-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9d1e-142">See also</span></span>

- [<span data-ttu-id="a9d1e-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a9d1e-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

