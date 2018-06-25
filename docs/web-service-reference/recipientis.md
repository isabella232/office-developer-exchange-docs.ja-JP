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
description: RecipientIs 要素は、電子メール メッセージの受信者と一致している値 (ProtectionRuleValueType) の子要素で指定した受信者のいずれかを指定します。
ms.openlocfilehash: b6d5c150cd874d1aced7f2d83ff36409e0738728
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832975"
---
# <a name="recipientis"></a><span data-ttu-id="4b7f4-103">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="4b7f4-103">RecipientIs</span></span>

<span data-ttu-id="4b7f4-104">**RecipientIs**要素は、電子メール メッセージの受信者と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定した受信者のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="4b7f4-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="4b7f4-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b7f4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4b7f4-106">Attributes and elements</span></span>

<span data-ttu-id="4b7f4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b7f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b7f4-108">Attributes</span></span>

<span data-ttu-id="4b7f4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b7f4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4b7f4-110">Child elements</span></span>

|<span data-ttu-id="4b7f4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4b7f4-111">**Element**</span></span>|<span data-ttu-id="4b7f4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4b7f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b7f4-113">値 (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="4b7f4-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="4b7f4-114">受信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b7f4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4b7f4-115">Parent elements</span></span>

|<span data-ttu-id="4b7f4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4b7f4-116">**Element**</span></span>|<span data-ttu-id="4b7f4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4b7f4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b7f4-118">条件</span><span class="sxs-lookup"><span data-stu-id="4b7f4-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="4b7f4-119">実行するルールのアクション部の満たされている必要がある条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="4b7f4-120">(ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="4b7f4-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="4b7f4-121">すべての子要素と一致するが**true**と評価されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b7f4-122">備考</span><span class="sxs-lookup"><span data-stu-id="4b7f4-122">Remarks</span></span>

<span data-ttu-id="4b7f4-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4b7f4-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b7f4-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="4b7f4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b7f4-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="4b7f4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b7f4-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4b7f4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4b7f4-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4b7f4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b7f4-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4b7f4-128">Validation File</span></span>  <br/> |<span data-ttu-id="4b7f4-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b7f4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b7f4-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4b7f4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b7f4-131">False</span><span class="sxs-lookup"><span data-stu-id="4b7f4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b7f4-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4b7f4-132">See also</span></span>



- [<span data-ttu-id="4b7f4-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4b7f4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

