---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: SenderDepartments 要素は、送信者の部署が、子の値 (ProtectionRuleValueType) 要素で指定された部署のいずれかと一致することを指定します。
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530346"
---
# <a name="senderdepartments"></a><span data-ttu-id="10df7-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="10df7-103">SenderDepartments</span></span>

<span data-ttu-id="10df7-104">**SenderDepartments**要素は、送信者の部署が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された部署のいずれかと一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="10df7-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="10df7-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="10df7-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10df7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="10df7-106">Attributes and elements</span></span>

<span data-ttu-id="10df7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="10df7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10df7-108">属性</span><span class="sxs-lookup"><span data-stu-id="10df7-108">Attributes</span></span>

<span data-ttu-id="10df7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="10df7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10df7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="10df7-110">Child elements</span></span>

|<span data-ttu-id="10df7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="10df7-111">**Element**</span></span>|<span data-ttu-id="10df7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="10df7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10df7-113">Value (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="10df7-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="10df7-114">単一の送信者部署を識別します。</span><span class="sxs-lookup"><span data-stu-id="10df7-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10df7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="10df7-115">Parent elements</span></span>

|<span data-ttu-id="10df7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="10df7-116">**Element**</span></span>|<span data-ttu-id="10df7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="10df7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10df7-118">条件</span><span class="sxs-lookup"><span data-stu-id="10df7-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="10df7-119">実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="10df7-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="10df7-120">および (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="10df7-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="10df7-121">**True**に評価するためにすべての子要素を一致させる必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="10df7-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="10df7-122">保護ルールの子条件が複数存在する必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="10df7-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="10df7-123">注釈</span><span class="sxs-lookup"><span data-stu-id="10df7-123">Remarks</span></span>

<span data-ttu-id="10df7-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="10df7-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10df7-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="10df7-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10df7-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="10df7-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10df7-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="10df7-127">Schema Name</span></span>  <br/> |<span data-ttu-id="10df7-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="10df7-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="10df7-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="10df7-129">Validation File</span></span>  <br/> |<span data-ttu-id="10df7-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="10df7-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10df7-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="10df7-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="10df7-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="10df7-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10df7-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="10df7-133">See also</span></span>



- [<span data-ttu-id="10df7-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="10df7-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

