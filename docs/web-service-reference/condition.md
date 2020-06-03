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
description: Condition 要素は、実行するルールのアクション部分に対して満たす必要がある条件を指定します。
ms.openlocfilehash: 2aea11197f072a4dbe21292bb47075d6f273d31b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463224"
---
# <a name="condition"></a><span data-ttu-id="a8f7f-103">条件</span><span class="sxs-lookup"><span data-stu-id="a8f7f-103">Condition</span></span>

<span data-ttu-id="a8f7f-104">**Condition**要素は、実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

<span data-ttu-id="a8f7f-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="a8f7f-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8f7f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8f7f-106">Attributes and elements</span></span>

<span data-ttu-id="a8f7f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8f7f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8f7f-108">Attributes</span></span>

<span data-ttu-id="a8f7f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8f7f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a8f7f-110">Child elements</span></span>

|<span data-ttu-id="a8f7f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a8f7f-111">**Element**</span></span>|<span data-ttu-id="a8f7f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8f7f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8f7f-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="a8f7f-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="a8f7f-114">電子メールメッセージのすべての受信者が送信者の組織の内部にある場合は、 **true**に評価されます。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="a8f7f-115">および (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="a8f7f-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="a8f7f-116">**True**に評価するためにすべての子要素を一致させる必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="a8f7f-117">保護ルールの子条件が複数存在する必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="a8f7f-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="a8f7f-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="a8f7f-119">電子メールメッセージのすべての受信者が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された受信者のいずれかと一致するように指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a8f7f-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="a8f7f-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="a8f7f-121">送信者の部署が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された部署のいずれかと一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a8f7f-122">True</span><span class="sxs-lookup"><span data-stu-id="a8f7f-122">True</span></span>](true.md) <br/> |<span data-ttu-id="a8f7f-123">常に一致する条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8f7f-124">親要素</span><span class="sxs-lookup"><span data-stu-id="a8f7f-124">Parent elements</span></span>

|<span data-ttu-id="a8f7f-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8f7f-125">**Element**</span></span>|<span data-ttu-id="a8f7f-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8f7f-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8f7f-127">Rule</span><span class="sxs-lookup"><span data-stu-id="a8f7f-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="a8f7f-128">1つの保護ルールを含みます。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8f7f-129">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8f7f-129">Text value</span></span>

<span data-ttu-id="a8f7f-130">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8f7f-131">注釈</span><span class="sxs-lookup"><span data-stu-id="a8f7f-131">Remarks</span></span>

<span data-ttu-id="a8f7f-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a8f7f-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8f7f-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8f7f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8f7f-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8f7f-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8f7f-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8f7f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a8f7f-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8f7f-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8f7f-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8f7f-137">Validation File</span></span>  <br/> |<span data-ttu-id="a8f7f-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8f7f-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8f7f-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8f7f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8f7f-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8f7f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8f7f-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8f7f-141">See also</span></span>

- [<span data-ttu-id="a8f7f-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8f7f-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

