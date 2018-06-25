---
title: アクション (ProtectionRuleActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: Action 要素では、ルールの条件部分と一致する場合、どのようなアクションを実行する必要がありますを識別します。
ms.openlocfilehash: 8f699e698d3159c5ff2636da506542da3b218251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760446"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="b2f8f-103">アクション (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="b2f8f-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="b2f8f-104">**Action**要素では、ルールの条件部分と一致する場合、どのようなアクションを実行する必要がありますを識別します。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="b2f8f-105">**ProtectionRuleActionType**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2f8f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b2f8f-106">Attributes and elements</span></span>

<span data-ttu-id="b2f8f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2f8f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2f8f-108">Attributes</span></span>

|<span data-ttu-id="b2f8f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-109">**Attribute**</span></span>|<span data-ttu-id="b2f8f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b2f8f-111">**名前**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-111">**Name**</span></span> <br/> |<span data-ttu-id="b2f8f-112">アクションの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b2f8f-113">子要素</span><span class="sxs-lookup"><span data-stu-id="b2f8f-113">Child elements</span></span>

|<span data-ttu-id="b2f8f-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-114">**Element**</span></span>|<span data-ttu-id="b2f8f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2f8f-116">引数</span><span class="sxs-lookup"><span data-stu-id="b2f8f-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="b2f8f-117">アクションに引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-117">Specifies arguments to the action.</span></span> <span data-ttu-id="b2f8f-118">指定されたアクションが引数を指定する必要がない場合は、この要素は表示されません。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="b2f8f-119">アクションが 1 つまたは複数の引数を必要とする場合、この要素は 1 つまたは複数回を発生します。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="b2f8f-120">**RightsProtectMessage**アクションは、1 つの引数に含まれます。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b2f8f-121">親要素</span><span class="sxs-lookup"><span data-stu-id="b2f8f-121">Parent elements</span></span>

|<span data-ttu-id="b2f8f-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-122">**Element**</span></span>|<span data-ttu-id="b2f8f-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2f8f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2f8f-124">Rule</span><span class="sxs-lookup"><span data-stu-id="b2f8f-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="b2f8f-125">1 つの保護ルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b2f8f-126">備考</span><span class="sxs-lookup"><span data-stu-id="b2f8f-126">Remarks</span></span>

<span data-ttu-id="b2f8f-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2f8f-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2f8f-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="b2f8f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2f8f-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="b2f8f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2f8f-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2f8f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b2f8f-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b2f8f-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2f8f-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2f8f-132">Validation File</span></span>  <br/> |<span data-ttu-id="b2f8f-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b2f8f-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2f8f-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b2f8f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2f8f-135">False</span><span class="sxs-lookup"><span data-stu-id="b2f8f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2f8f-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2f8f-136">See also</span></span>

- [<span data-ttu-id="b2f8f-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b2f8f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

