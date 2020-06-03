---
title: および (ProtectionRuleAndType)
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
description: And 要素は、すべての子要素が true に評価されるように一致する必要があることを指定します。
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464736"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="ed9be-103">および (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="ed9be-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="ed9be-104">**And**要素は、すべての子要素が**true**に評価されるように一致する必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="ed9be-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="ed9be-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed9be-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ed9be-106">Attributes and elements</span></span>

<span data-ttu-id="ed9be-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed9be-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed9be-108">Attributes</span></span>

<span data-ttu-id="ed9be-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed9be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed9be-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed9be-110">Child elements</span></span>

|<span data-ttu-id="ed9be-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ed9be-111">**Element**</span></span>|<span data-ttu-id="ed9be-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed9be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed9be-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="ed9be-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="ed9be-114">電子メールメッセージのすべての受信者が送信者の組織の内部にある場合は、 **true**に評価されます。</span><span class="sxs-lookup"><span data-stu-id="ed9be-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="ed9be-115">**And**</span><span class="sxs-lookup"><span data-stu-id="ed9be-115">**And**</span></span> <br/> |<span data-ttu-id="ed9be-116">**True**に評価するためにすべての子要素を一致させる必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="ed9be-117">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="ed9be-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="ed9be-118">電子メールメッセージのすべての受信者が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された受信者のいずれかと一致するように指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="ed9be-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="ed9be-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="ed9be-120">送信者の部署が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された部署のいずれかと一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="ed9be-121">True</span><span class="sxs-lookup"><span data-stu-id="ed9be-121">True</span></span>](true.md) <br/> |<span data-ttu-id="ed9be-122">常に一致する条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed9be-123">親要素</span><span class="sxs-lookup"><span data-stu-id="ed9be-123">Parent elements</span></span>

|<span data-ttu-id="ed9be-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed9be-124">**Element**</span></span>|<span data-ttu-id="ed9be-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed9be-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed9be-126">条件</span><span class="sxs-lookup"><span data-stu-id="ed9be-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="ed9be-127">実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="ed9be-128">**And**</span><span class="sxs-lookup"><span data-stu-id="ed9be-128">**And**</span></span> <br/> |<span data-ttu-id="ed9be-129">**True**に評価するためにすべての子要素を一致させる必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9be-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed9be-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed9be-130">Text value</span></span>

<span data-ttu-id="ed9be-131">なし。</span><span class="sxs-lookup"><span data-stu-id="ed9be-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed9be-132">注釈</span><span class="sxs-lookup"><span data-stu-id="ed9be-132">Remarks</span></span>

<span data-ttu-id="ed9be-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ed9be-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed9be-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ed9be-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed9be-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed9be-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed9be-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed9be-136">Schema Name</span></span>  <br/> |<span data-ttu-id="ed9be-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ed9be-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed9be-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed9be-138">Validation File</span></span>  <br/> |<span data-ttu-id="ed9be-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ed9be-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed9be-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed9be-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed9be-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="ed9be-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed9be-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed9be-142">See also</span></span>

- [<span data-ttu-id="ed9be-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ed9be-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

