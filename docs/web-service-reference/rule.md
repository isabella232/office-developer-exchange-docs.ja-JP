---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: ルール要素には、1 つの保護ルールが含まれています。
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833263"
---
# <a name="rule"></a><span data-ttu-id="d762c-103">Rule</span><span class="sxs-lookup"><span data-stu-id="d762c-103">Rule</span></span>

<span data-ttu-id="d762c-104">**ルール**要素には、1 つの保護ルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d762c-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="d762c-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="d762c-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d762c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d762c-106">Attributes and elements</span></span>

<span data-ttu-id="d762c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d762c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d762c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d762c-108">Attributes</span></span>

|<span data-ttu-id="d762c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d762c-109">**Attribute**</span></span>|<span data-ttu-id="d762c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d762c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d762c-111">**名前**</span><span class="sxs-lookup"><span data-stu-id="d762c-111">**Name**</span></span> <br/> |<span data-ttu-id="d762c-112">ルールの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="d762c-112">Identifies the name of the rule.</span></span> <span data-ttu-id="d762c-113">1 の最小の長さと文字列型の必須の属性です。</span><span class="sxs-lookup"><span data-stu-id="d762c-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="d762c-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="d762c-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="d762c-115">ルールが必須かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d762c-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="d762c-116">ルールが必須の場合は、この属性値は**false を指定**する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d762c-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="d762c-117">ブール型の必須の属性です。</span><span class="sxs-lookup"><span data-stu-id="d762c-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="d762c-118">**Priority**</span><span class="sxs-lookup"><span data-stu-id="d762c-118">**Priority**</span></span> <br/> |<span data-ttu-id="d762c-119">ルールの優先度を指定します。</span><span class="sxs-lookup"><span data-stu-id="d762c-119">Specifies the rule priority.</span></span> <span data-ttu-id="d762c-120">1 の最小値を int 型の必須の属性です。</span><span class="sxs-lookup"><span data-stu-id="d762c-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d762c-121">子要素</span><span class="sxs-lookup"><span data-stu-id="d762c-121">Child elements</span></span>

|<span data-ttu-id="d762c-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="d762c-122">**Element**</span></span>|<span data-ttu-id="d762c-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="d762c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d762c-124">条件</span><span class="sxs-lookup"><span data-stu-id="d762c-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="d762c-125">実行するルールのアクション部の満たされている必要がある条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="d762c-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="d762c-126">アクション (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="d762c-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="d762c-127">ルールの条件部分と一致する場合、どのようなアクションを実行する必要がありますを識別します。</span><span class="sxs-lookup"><span data-stu-id="d762c-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d762c-128">親要素</span><span class="sxs-lookup"><span data-stu-id="d762c-128">Parent elements</span></span>

|<span data-ttu-id="d762c-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="d762c-129">**Element**</span></span>|<span data-ttu-id="d762c-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="d762c-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d762c-131">ルール</span><span class="sxs-lookup"><span data-stu-id="d762c-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d762c-132">保護規則の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d762c-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d762c-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d762c-133">Text value</span></span>

<span data-ttu-id="d762c-134">なし。</span><span class="sxs-lookup"><span data-stu-id="d762c-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d762c-135">備考</span><span class="sxs-lookup"><span data-stu-id="d762c-135">Remarks</span></span>

<span data-ttu-id="d762c-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d762c-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d762c-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="d762c-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d762c-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="d762c-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d762c-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d762c-139">Schema Name</span></span>  <br/> |<span data-ttu-id="d762c-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d762c-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="d762c-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d762c-141">Validation File</span></span>  <br/> |<span data-ttu-id="d762c-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d762c-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d762c-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d762c-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="d762c-144">False</span><span class="sxs-lookup"><span data-stu-id="d762c-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d762c-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d762c-145">See also</span></span>



- [<span data-ttu-id="d762c-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d762c-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

