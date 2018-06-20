---
title: 条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: 条件要素では、実行されるルールのアクション部の満たされている必要がある条件を識別します。
ms.openlocfilehash: ed605946f99aa63416337cd0e731c931176a8ed4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759647"
---
# <a name="condition"></a><span data-ttu-id="7b788-103">条件</span><span class="sxs-lookup"><span data-stu-id="7b788-103">Condition</span></span>

<span data-ttu-id="7b788-104">**条件**要素では、実行されるルールのアクション部の満たされている必要がある条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="7b788-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

 <span data-ttu-id="7b788-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="7b788-105">**ProtectionRuleConditionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b788-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7b788-106">Attributes and elements</span></span>

<span data-ttu-id="7b788-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b788-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b788-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b788-108">Attributes</span></span>

<span data-ttu-id="7b788-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7b788-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b788-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7b788-110">Child elements</span></span>

|<span data-ttu-id="7b788-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b788-111">**Element**</span></span>|<span data-ttu-id="7b788-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b788-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b788-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="7b788-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="7b788-114">電子メール メッセージのすべての受信者が送信者の組織の内部場合は、 **true**に評価されます。</span><span class="sxs-lookup"><span data-stu-id="7b788-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="7b788-115">(ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="7b788-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="7b788-116">すべての子要素と一致するが**true**と評価されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b788-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="7b788-117">保護ルール子の 1 つ以上の条件が存在する必要がありますを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b788-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="7b788-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="7b788-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="7b788-119">電子メール メッセージの受信者と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定した受信者のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b788-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="7b788-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="7b788-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="7b788-121">送信者の部署と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定された部門のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b788-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="7b788-122">True</span><span class="sxs-lookup"><span data-stu-id="7b788-122">True</span></span>](true.md) <br/> |<span data-ttu-id="7b788-123">常に一致する条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b788-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b788-124">親要素</span><span class="sxs-lookup"><span data-stu-id="7b788-124">Parent elements</span></span>

|<span data-ttu-id="7b788-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b788-125">**Element**</span></span>|<span data-ttu-id="7b788-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b788-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b788-127">Rule</span><span class="sxs-lookup"><span data-stu-id="7b788-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="7b788-128">1 つの保護ルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b788-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b788-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7b788-129">Text value</span></span>

<span data-ttu-id="7b788-130">なし。</span><span class="sxs-lookup"><span data-stu-id="7b788-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7b788-131">備考</span><span class="sxs-lookup"><span data-stu-id="7b788-131">Remarks</span></span>

<span data-ttu-id="7b788-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7b788-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b788-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="7b788-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b788-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="7b788-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b788-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b788-135">Schema Name</span></span>  <br/> |<span data-ttu-id="7b788-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7b788-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b788-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b788-137">Validation File</span></span>  <br/> |<span data-ttu-id="7b788-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b788-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b788-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7b788-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b788-140">False</span><span class="sxs-lookup"><span data-stu-id="7b788-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b788-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b788-141">See also</span></span>



- [<span data-ttu-id="7b788-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7b788-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

