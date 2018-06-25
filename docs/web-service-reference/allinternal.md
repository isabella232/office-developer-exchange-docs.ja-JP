---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: AllInternal 要素は、電子メール メッセージのすべての受信者が送信者の組織に内部にある場合に、true に評価します。
ms.openlocfilehash: 0ffd4178e711e3117497eed682e3fd3e0594989b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759310"
---
# <a name="allinternal"></a><span data-ttu-id="406aa-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="406aa-103">AllInternal</span></span>

<span data-ttu-id="406aa-104">**AllInternal**要素は、電子メール メッセージのすべての受信者が送信者の組織に内部にある場合に**true**に評価されました。</span><span class="sxs-lookup"><span data-stu-id="406aa-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="406aa-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="406aa-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="406aa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="406aa-106">Attributes and elements</span></span>

<span data-ttu-id="406aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="406aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="406aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="406aa-108">Attributes</span></span>

<span data-ttu-id="406aa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="406aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="406aa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="406aa-110">Child elements</span></span>

<span data-ttu-id="406aa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="406aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="406aa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="406aa-112">Parent elements</span></span>

|<span data-ttu-id="406aa-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="406aa-113">**Element**</span></span>|<span data-ttu-id="406aa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="406aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="406aa-115">条件</span><span class="sxs-lookup"><span data-stu-id="406aa-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="406aa-116">実行するルールのアクション部の満たされている必要がある条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="406aa-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="406aa-117">(ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="406aa-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="406aa-118">すべての子要素と一致するが**true**と評価されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="406aa-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="406aa-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="406aa-119">Text value</span></span>

<span data-ttu-id="406aa-120">**AllInternal**要素を空にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="406aa-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="406aa-121">備考</span><span class="sxs-lookup"><span data-stu-id="406aa-121">Remarks</span></span>

<span data-ttu-id="406aa-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="406aa-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="406aa-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="406aa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="406aa-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="406aa-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="406aa-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="406aa-125">Schema Name</span></span>  <br/> |<span data-ttu-id="406aa-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="406aa-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="406aa-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="406aa-127">Validation File</span></span>  <br/> |<span data-ttu-id="406aa-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="406aa-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="406aa-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="406aa-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="406aa-130">False</span><span class="sxs-lookup"><span data-stu-id="406aa-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="406aa-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="406aa-131">See also</span></span>

- [<span data-ttu-id="406aa-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="406aa-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

