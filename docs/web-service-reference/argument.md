---
title: 引数
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
description: 引数の要素は、アクションの引数を指定します。
ms.openlocfilehash: ed4e46a8d9897516e9c96bf3930f7d488bc06714
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759438"
---
# <a name="argument"></a><span data-ttu-id="7cf0b-103">引数</span><span class="sxs-lookup"><span data-stu-id="7cf0b-103">Argument</span></span>

<span data-ttu-id="7cf0b-104">**引数**の要素は、アクションの引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="7cf0b-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cf0b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7cf0b-106">Attributes and elements</span></span>

<span data-ttu-id="7cf0b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cf0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7cf0b-108">Attributes</span></span>

|<span data-ttu-id="7cf0b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-109">**Attribute**</span></span>|<span data-ttu-id="7cf0b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cf0b-111">**Value**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-111">**Value**</span></span> <br/> |<span data-ttu-id="7cf0b-112">保護ルールのアクションに引数の値を表す空白以外の文字列値。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="7cf0b-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7cf0b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7cf0b-114">Child elements</span></span>

<span data-ttu-id="7cf0b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7cf0b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7cf0b-116">Parent elements</span></span>

|<span data-ttu-id="7cf0b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-117">**Element**</span></span>|<span data-ttu-id="7cf0b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cf0b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cf0b-119">アクション (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="7cf0b-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="7cf0b-120">ルールの条件部分と一致する場合、どのようなアクションを実行する必要がありますを識別します。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cf0b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7cf0b-121">Text value</span></span>

<span data-ttu-id="7cf0b-122">なし。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cf0b-123">備考</span><span class="sxs-lookup"><span data-stu-id="7cf0b-123">Remarks</span></span>

<span data-ttu-id="7cf0b-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7cf0b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cf0b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="7cf0b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cf0b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="7cf0b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cf0b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7cf0b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7cf0b-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7cf0b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cf0b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7cf0b-129">Validation File</span></span>  <br/> |<span data-ttu-id="7cf0b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cf0b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cf0b-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7cf0b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cf0b-132">False</span><span class="sxs-lookup"><span data-stu-id="7cf0b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cf0b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7cf0b-133">See also</span></span>

- [<span data-ttu-id="7cf0b-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7cf0b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

