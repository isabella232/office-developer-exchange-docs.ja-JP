---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: RecipientIs 要素は、電子メールメッセージのすべての受信者が、子の値 (ProtectionRuleValueType) 要素内の指定された受信者のいずれかと一致することを指定します。
ms.openlocfilehash: 8f27c4484ce310c62f9bab0e6ffeea2bfac1d3ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463882"
---
# <a name="recipientis"></a><span data-ttu-id="9bac5-103">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="9bac5-103">RecipientIs</span></span>

<span data-ttu-id="9bac5-104">**RecipientIs**要素は、電子メールメッセージのすべての受信者が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素内の指定された受信者のいずれかと一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="9bac5-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="9bac5-105">**Protection/の Pientistype**</span><span class="sxs-lookup"><span data-stu-id="9bac5-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9bac5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9bac5-106">Attributes and elements</span></span>

<span data-ttu-id="9bac5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9bac5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9bac5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9bac5-108">Attributes</span></span>

<span data-ttu-id="9bac5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9bac5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9bac5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9bac5-110">Child elements</span></span>

|<span data-ttu-id="9bac5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9bac5-111">**Element**</span></span>|<span data-ttu-id="9bac5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bac5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bac5-113">Value (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="9bac5-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="9bac5-114">受信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="9bac5-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9bac5-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9bac5-115">Parent elements</span></span>

|<span data-ttu-id="9bac5-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9bac5-116">**Element**</span></span>|<span data-ttu-id="9bac5-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bac5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bac5-118">条件</span><span class="sxs-lookup"><span data-stu-id="9bac5-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="9bac5-119">実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="9bac5-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="9bac5-120">および (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="9bac5-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="9bac5-121">**True**に評価するためにすべての子要素を一致させる必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9bac5-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9bac5-122">注釈</span><span class="sxs-lookup"><span data-stu-id="9bac5-122">Remarks</span></span>

<span data-ttu-id="9bac5-123">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="9bac5-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9bac5-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9bac5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9bac5-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9bac5-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9bac5-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9bac5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9bac5-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9bac5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9bac5-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9bac5-128">Validation File</span></span>  <br/> |<span data-ttu-id="9bac5-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9bac5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9bac5-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9bac5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9bac5-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="9bac5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9bac5-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9bac5-132">See also</span></span>



- [<span data-ttu-id="9bac5-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9bac5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

