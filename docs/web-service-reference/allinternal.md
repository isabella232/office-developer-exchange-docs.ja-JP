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
description: 電子メールメッセージのすべての受信者が送信者の組織の内部にある場合、AllInternal 要素は true に評価されます。
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464834"
---
# <a name="allinternal"></a><span data-ttu-id="f33f0-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="f33f0-103">AllInternal</span></span>

<span data-ttu-id="f33f0-104">電子メールメッセージのすべての受信者が送信者の組織の内部にある場合、 **AllInternal**要素は**true**に評価されます。</span><span class="sxs-lookup"><span data-stu-id="f33f0-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="f33f0-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="f33f0-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f33f0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f33f0-106">Attributes and elements</span></span>

<span data-ttu-id="f33f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f33f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f33f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="f33f0-108">Attributes</span></span>

<span data-ttu-id="f33f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f33f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f33f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f33f0-110">Child elements</span></span>

<span data-ttu-id="f33f0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f33f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f33f0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f33f0-112">Parent elements</span></span>

|<span data-ttu-id="f33f0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f33f0-113">**Element**</span></span>|<span data-ttu-id="f33f0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f33f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f33f0-115">条件</span><span class="sxs-lookup"><span data-stu-id="f33f0-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="f33f0-116">実行するルールのアクション部分に対して満たす必要がある条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="f33f0-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="f33f0-117">および (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="f33f0-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="f33f0-118">**True**に評価するためにすべての子要素を一致させる必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="f33f0-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f33f0-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f33f0-119">Text value</span></span>

<span data-ttu-id="f33f0-120">**AllInternal**要素は空である必要があります。</span><span class="sxs-lookup"><span data-stu-id="f33f0-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f33f0-121">注釈</span><span class="sxs-lookup"><span data-stu-id="f33f0-121">Remarks</span></span>

<span data-ttu-id="f33f0-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f33f0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f33f0-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f33f0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f33f0-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f33f0-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f33f0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f33f0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f33f0-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f33f0-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f33f0-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f33f0-127">Validation File</span></span>  <br/> |<span data-ttu-id="f33f0-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f33f0-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f33f0-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f33f0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f33f0-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="f33f0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f33f0-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f33f0-131">See also</span></span>

- [<span data-ttu-id="f33f0-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f33f0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

