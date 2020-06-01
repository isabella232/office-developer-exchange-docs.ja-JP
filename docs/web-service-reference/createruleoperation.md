---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: CreateRuleOperation 要素は、新しい受信トレイルールを作成する操作を表します。
ms.openlocfilehash: df857544e6d5840a3f738740114195e4c4bb5798
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460772"
---
# <a name="createruleoperation"></a><span data-ttu-id="3a521-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3a521-103">CreateRuleOperation</span></span>

<span data-ttu-id="3a521-104">**CreateRuleOperation**要素は、新しい受信トレイルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="3a521-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="3a521-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3a521-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="3a521-106">Operations</span><span class="sxs-lookup"><span data-stu-id="3a521-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="3a521-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="3a521-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a521-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3a521-108">Attributes and elements</span></span>

<span data-ttu-id="3a521-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a521-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a521-110">属性</span><span class="sxs-lookup"><span data-stu-id="3a521-110">Attributes</span></span>

<span data-ttu-id="3a521-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3a521-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a521-112">子要素</span><span class="sxs-lookup"><span data-stu-id="3a521-112">Child elements</span></span>

|<span data-ttu-id="3a521-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="3a521-113">**Element**</span></span>|<span data-ttu-id="3a521-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a521-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a521-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="3a521-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="3a521-116">ユーザーのメールボックスに作成されるルールを表します。</span><span class="sxs-lookup"><span data-stu-id="3a521-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a521-117">親要素</span><span class="sxs-lookup"><span data-stu-id="3a521-117">Parent elements</span></span>

|<span data-ttu-id="3a521-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a521-118">**Element**</span></span>|<span data-ttu-id="3a521-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a521-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a521-120">Operations</span><span class="sxs-lookup"><span data-stu-id="3a521-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="3a521-121">受信トレイに対して実行できる操作が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3a521-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a521-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3a521-122">Text value</span></span>

<span data-ttu-id="3a521-123">なし。</span><span class="sxs-lookup"><span data-stu-id="3a521-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a521-124">注釈</span><span class="sxs-lookup"><span data-stu-id="3a521-124">Remarks</span></span>

<span data-ttu-id="3a521-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a521-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a521-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3a521-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a521-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a521-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a521-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a521-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3a521-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3a521-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="3a521-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a521-130">Validation File</span></span>  <br/> |<span data-ttu-id="3a521-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3a521-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a521-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3a521-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a521-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="3a521-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a521-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a521-134">See also</span></span>



[<span data-ttu-id="3a521-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3a521-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="3a521-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3a521-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="3a521-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3a521-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="3a521-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3a521-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

