---
title: ルール (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: ルール要素は、1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833259"
---
# <a name="rule-ruletype"></a><span data-ttu-id="3fd10-103">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="3fd10-103">Rule (RuleType)</span></span>

<span data-ttu-id="3fd10-104">**ルール**要素は、1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 <span data-ttu-id="3fd10-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="3fd10-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fd10-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3fd10-106">Attributes and elements</span></span>

<span data-ttu-id="3fd10-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fd10-108">属性</span><span class="sxs-lookup"><span data-stu-id="3fd10-108">Attributes</span></span>

<span data-ttu-id="3fd10-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3fd10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fd10-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3fd10-110">Child elements</span></span>

|<span data-ttu-id="3fd10-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fd10-111">**Element**</span></span>|<span data-ttu-id="3fd10-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fd10-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fd10-113">規則 Id</span><span class="sxs-lookup"><span data-stu-id="3fd10-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="3fd10-114">ルールの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-115">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="3fd10-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="3fd10-116">ルールの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fd10-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-117">Priority</span><span class="sxs-lookup"><span data-stu-id="3fd10-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="3fd10-118">ルールの実行順序を示します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-119">有効</span><span class="sxs-lookup"><span data-stu-id="3fd10-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="3fd10-120">ルールが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="3fd10-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="3fd10-122">Api のマネージ コードでルールを変更できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="3fd10-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="3fd10-124">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-125">条件</span><span class="sxs-lookup"><span data-stu-id="3fd10-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3fd10-126">条件を識別するには、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="3fd10-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="3fd10-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3fd10-128">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を識別します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-129">アクション</span><span class="sxs-lookup"><span data-stu-id="3fd10-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="3fd10-130">条件が満たされるときに、メッセージに対して実行されるアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fd10-131">親要素</span><span class="sxs-lookup"><span data-stu-id="3fd10-131">Parent elements</span></span>

|<span data-ttu-id="3fd10-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fd10-132">**Element**</span></span>|<span data-ttu-id="3fd10-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fd10-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fd10-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3fd10-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="3fd10-135">新しいルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-136">InboxRules</span><span class="sxs-lookup"><span data-stu-id="3fd10-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="3fd10-137">ユーザーのメールボックスのルールの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3fd10-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3fd10-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="3fd10-139">既存のルールを更新する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="3fd10-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3fd10-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3fd10-140">Text value</span></span>

<span data-ttu-id="3fd10-141">なし。</span><span class="sxs-lookup"><span data-stu-id="3fd10-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3fd10-142">備考</span><span class="sxs-lookup"><span data-stu-id="3fd10-142">Remarks</span></span>

<span data-ttu-id="3fd10-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3fd10-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fd10-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="3fd10-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fd10-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="3fd10-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fd10-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3fd10-146">Schema Name</span></span>  <br/> |<span data-ttu-id="3fd10-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3fd10-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fd10-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3fd10-148">Validation File</span></span>  <br/> |<span data-ttu-id="3fd10-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3fd10-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fd10-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3fd10-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fd10-151">True</span><span class="sxs-lookup"><span data-stu-id="3fd10-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fd10-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fd10-152">See also</span></span>



[<span data-ttu-id="3fd10-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3fd10-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="3fd10-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3fd10-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="3fd10-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="3fd10-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="3fd10-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3fd10-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

