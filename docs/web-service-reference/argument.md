---
title: 主張
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Argument
api_type:
- schema
ms.assetid: 15b0bfb8-2448-4ceb-aeac-965115e0fb72
description: 引数要素は、アクションへの引数を指定します。
ms.openlocfilehash: 41e3b1d891610669b0cc93f3daf6e8ee98c48396
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464757"
---
# <a name="argument"></a><span data-ttu-id="e65b1-103">主張</span><span class="sxs-lookup"><span data-stu-id="e65b1-103">Argument</span></span>

<span data-ttu-id="e65b1-104">**引数**要素は、アクションへの引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e65b1-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="e65b1-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="e65b1-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e65b1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e65b1-106">Attributes and elements</span></span>

<span data-ttu-id="e65b1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e65b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e65b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="e65b1-108">Attributes</span></span>

|<span data-ttu-id="e65b1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e65b1-109">**Attribute**</span></span>|<span data-ttu-id="e65b1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e65b1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e65b1-111">**値**</span><span class="sxs-lookup"><span data-stu-id="e65b1-111">**Value**</span></span> <br/> |<span data-ttu-id="e65b1-112">保護ルールのアクション部分の引数の値を表す、空ではない文字列値。</span><span class="sxs-lookup"><span data-stu-id="e65b1-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="e65b1-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="e65b1-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e65b1-114">子要素</span><span class="sxs-lookup"><span data-stu-id="e65b1-114">Child elements</span></span>

<span data-ttu-id="e65b1-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e65b1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e65b1-116">親要素</span><span class="sxs-lookup"><span data-stu-id="e65b1-116">Parent elements</span></span>

|<span data-ttu-id="e65b1-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e65b1-117">**Element**</span></span>|<span data-ttu-id="e65b1-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e65b1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e65b1-119">アクション (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="e65b1-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="e65b1-120">ルールの条件部分が一致する場合に実行する必要のあるアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="e65b1-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e65b1-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e65b1-121">Text value</span></span>

<span data-ttu-id="e65b1-122">なし。</span><span class="sxs-lookup"><span data-stu-id="e65b1-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e65b1-123">注釈</span><span class="sxs-lookup"><span data-stu-id="e65b1-123">Remarks</span></span>

<span data-ttu-id="e65b1-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e65b1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e65b1-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e65b1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e65b1-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e65b1-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e65b1-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e65b1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e65b1-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e65b1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e65b1-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e65b1-129">Validation File</span></span>  <br/> |<span data-ttu-id="e65b1-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e65b1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e65b1-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e65b1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e65b1-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="e65b1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e65b1-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="e65b1-133">See also</span></span>

- [<span data-ttu-id="e65b1-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e65b1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

