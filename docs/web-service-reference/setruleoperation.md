---
title: SetRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetRuleOperation
api_type:
- schema
ms.assetid: 2106a85b-58fe-49be-b71d-4ca6aa66e060
description: SetRuleOperation 要素は、既存のルールを更新する操作を表します。
ms.openlocfilehash: 96fba2f229003b8c729c36614e69655852a3aa8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526334"
---
# <a name="setruleoperation"></a><span data-ttu-id="814e4-103">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="814e4-103">SetRuleOperation</span></span>

<span data-ttu-id="814e4-104">**SetRuleOperation**要素は、既存のルールを更新する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="814e4-104">The **SetRuleOperation** element represents an operation to update an existing rule.</span></span> 
  
[<span data-ttu-id="814e4-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="814e4-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="814e4-106">Operations</span><span class="sxs-lookup"><span data-stu-id="814e4-106">Operations</span></span>](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 <span data-ttu-id="814e4-107">**SetRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="814e4-107">**SetRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="814e4-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="814e4-108">Attributes and elements</span></span>

<span data-ttu-id="814e4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="814e4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="814e4-110">属性</span><span class="sxs-lookup"><span data-stu-id="814e4-110">Attributes</span></span>

<span data-ttu-id="814e4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="814e4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="814e4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="814e4-112">Child elements</span></span>

|<span data-ttu-id="814e4-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="814e4-113">**Element**</span></span>|<span data-ttu-id="814e4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="814e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="814e4-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="814e4-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="814e4-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="814e4-116">Represents a rule in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="814e4-117">親要素</span><span class="sxs-lookup"><span data-stu-id="814e4-117">Parent elements</span></span>

|<span data-ttu-id="814e4-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="814e4-118">**Element**</span></span>|<span data-ttu-id="814e4-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="814e4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="814e4-120">Operations</span><span class="sxs-lookup"><span data-stu-id="814e4-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="814e4-121">受信トレイに対して実行できるルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="814e4-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="814e4-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="814e4-122">Text value</span></span>

<span data-ttu-id="814e4-123">なし。</span><span class="sxs-lookup"><span data-stu-id="814e4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="814e4-124">注釈</span><span class="sxs-lookup"><span data-stu-id="814e4-124">Remarks</span></span>

<span data-ttu-id="814e4-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="814e4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="814e4-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="814e4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="814e4-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="814e4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="814e4-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="814e4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="814e4-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="814e4-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="814e4-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="814e4-130">Validation File</span></span>  <br/> |<span data-ttu-id="814e4-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="814e4-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="814e4-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="814e4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="814e4-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="814e4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="814e4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="814e4-134">See also</span></span>



[<span data-ttu-id="814e4-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="814e4-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="814e4-136">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="814e4-136">DeleteRuleOperation</span></span>](deleteruleoperation.md)
  
[<span data-ttu-id="814e4-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="814e4-137">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="814e4-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="814e4-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

