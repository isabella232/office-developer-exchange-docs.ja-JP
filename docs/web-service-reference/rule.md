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
description: Rule 要素には、1つの保護ルールが含まれています。
ms.openlocfilehash: 6c18a2bd026893cd333bc7007203abf04a6f0be7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465002"
---
# <a name="rule"></a><span data-ttu-id="db2af-103">Rule</span><span class="sxs-lookup"><span data-stu-id="db2af-103">Rule</span></span>

<span data-ttu-id="db2af-104">**Rule**要素には、1つの保護ルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="db2af-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="db2af-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="db2af-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db2af-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="db2af-106">Attributes and elements</span></span>

<span data-ttu-id="db2af-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db2af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db2af-108">属性</span><span class="sxs-lookup"><span data-stu-id="db2af-108">Attributes</span></span>

|<span data-ttu-id="db2af-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="db2af-109">**Attribute**</span></span>|<span data-ttu-id="db2af-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="db2af-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db2af-111">**名前**</span><span class="sxs-lookup"><span data-stu-id="db2af-111">**Name**</span></span> <br/> |<span data-ttu-id="db2af-112">ルールの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="db2af-112">Identifies the name of the rule.</span></span> <span data-ttu-id="db2af-113">最小の長さが1の文字列型の必須属性。</span><span class="sxs-lookup"><span data-stu-id="db2af-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="db2af-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="db2af-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="db2af-115">ルールが必須であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="db2af-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="db2af-116">ルールが必須の場合、この属性値は**false**にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="db2af-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="db2af-117">Boolean 型の必須の属性。</span><span class="sxs-lookup"><span data-stu-id="db2af-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="db2af-118">**[優先度]**</span><span class="sxs-lookup"><span data-stu-id="db2af-118">**Priority**</span></span> <br/> |<span data-ttu-id="db2af-119">ルールの優先度を指定します。</span><span class="sxs-lookup"><span data-stu-id="db2af-119">Specifies the rule priority.</span></span> <span data-ttu-id="db2af-120">最小値が1の int 型の必須属性。</span><span class="sxs-lookup"><span data-stu-id="db2af-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="db2af-121">子要素</span><span class="sxs-lookup"><span data-stu-id="db2af-121">Child elements</span></span>

|<span data-ttu-id="db2af-122">**Element**</span><span class="sxs-lookup"><span data-stu-id="db2af-122">**Element**</span></span>|<span data-ttu-id="db2af-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="db2af-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db2af-124">条件</span><span class="sxs-lookup"><span data-stu-id="db2af-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="db2af-125">実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="db2af-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="db2af-126">アクション (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="db2af-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="db2af-127">ルールの条件部分が一致する場合に実行する必要のあるアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="db2af-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db2af-128">親要素</span><span class="sxs-lookup"><span data-stu-id="db2af-128">Parent elements</span></span>

|<span data-ttu-id="db2af-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="db2af-129">**Element**</span></span>|<span data-ttu-id="db2af-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="db2af-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db2af-131">ルール</span><span class="sxs-lookup"><span data-stu-id="db2af-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="db2af-132">保護ルールの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="db2af-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db2af-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="db2af-133">Text value</span></span>

<span data-ttu-id="db2af-134">なし。</span><span class="sxs-lookup"><span data-stu-id="db2af-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db2af-135">注釈</span><span class="sxs-lookup"><span data-stu-id="db2af-135">Remarks</span></span>

<span data-ttu-id="db2af-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="db2af-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db2af-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="db2af-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db2af-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="db2af-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db2af-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db2af-139">Schema Name</span></span>  <br/> |<span data-ttu-id="db2af-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="db2af-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="db2af-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db2af-141">Validation File</span></span>  <br/> |<span data-ttu-id="db2af-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="db2af-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db2af-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db2af-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="db2af-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="db2af-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db2af-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="db2af-145">See also</span></span>



- [<span data-ttu-id="db2af-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="db2af-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

