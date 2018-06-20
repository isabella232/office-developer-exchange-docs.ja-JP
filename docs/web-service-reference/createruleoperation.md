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
description: CreateRuleOperation 要素は、新しい受信トレイ ルールを作成する操作を表します。
ms.openlocfilehash: c531f222ffe886e6ef53a99609cfa27e84fd6107
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759854"
---
# <a name="createruleoperation"></a><span data-ttu-id="ae4d1-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ae4d1-103">CreateRuleOperation</span></span>

<span data-ttu-id="ae4d1-104">**CreateRuleOperation**要素は、新しい受信トレイ ルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="ae4d1-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="ae4d1-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="ae4d1-106">Operations</span><span class="sxs-lookup"><span data-stu-id="ae4d1-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="ae4d1-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="ae4d1-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae4d1-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ae4d1-108">Attributes and elements</span></span>

<span data-ttu-id="ae4d1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae4d1-110">属性</span><span class="sxs-lookup"><span data-stu-id="ae4d1-110">Attributes</span></span>

<span data-ttu-id="ae4d1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae4d1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ae4d1-112">Child elements</span></span>

|<span data-ttu-id="ae4d1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae4d1-113">**Element**</span></span>|<span data-ttu-id="ae4d1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae4d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4d1-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="ae4d1-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="ae4d1-116">ユーザーのメールボックス内に作成する規則を表します。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae4d1-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ae4d1-117">Parent elements</span></span>

|<span data-ttu-id="ae4d1-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae4d1-118">**Element**</span></span>|<span data-ttu-id="ae4d1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae4d1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4d1-120">Operations</span><span class="sxs-lookup"><span data-stu-id="ae4d1-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="ae4d1-121">受信トレイで実行できる操作が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae4d1-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ae4d1-122">Text value</span></span>

<span data-ttu-id="ae4d1-123">なし。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae4d1-124">備考</span><span class="sxs-lookup"><span data-stu-id="ae4d1-124">Remarks</span></span>

<span data-ttu-id="ae4d1-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ae4d1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae4d1-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="ae4d1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae4d1-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="ae4d1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae4d1-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae4d1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ae4d1-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ae4d1-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae4d1-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae4d1-130">Validation File</span></span>  <br/> |<span data-ttu-id="ae4d1-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae4d1-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae4d1-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ae4d1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae4d1-133">False</span><span class="sxs-lookup"><span data-stu-id="ae4d1-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae4d1-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae4d1-134">See also</span></span>



[<span data-ttu-id="ae4d1-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="ae4d1-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="ae4d1-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ae4d1-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="ae4d1-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ae4d1-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="ae4d1-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae4d1-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

