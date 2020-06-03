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
description: Rule 要素には、1つのルールが含まれており、ユーザーのメールボックス内のルールを表します。
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465080"
---
# <a name="rule-ruletype"></a><span data-ttu-id="55361-103">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="55361-103">Rule (RuleType)</span></span>

<span data-ttu-id="55361-104">**Rule**要素には、1つのルールが含まれており、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="55361-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
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

 <span data-ttu-id="55361-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="55361-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55361-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="55361-106">Attributes and elements</span></span>

<span data-ttu-id="55361-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55361-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55361-108">属性</span><span class="sxs-lookup"><span data-stu-id="55361-108">Attributes</span></span>

<span data-ttu-id="55361-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55361-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55361-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55361-110">Child elements</span></span>

|<span data-ttu-id="55361-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="55361-111">**Element**</span></span>|<span data-ttu-id="55361-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="55361-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55361-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="55361-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="55361-114">ルール識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="55361-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="55361-115">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="55361-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="55361-116">ルールの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="55361-116">Contains the display name of a rule.</span></span>  <br/> |
|<span data-ttu-id="55361-117">[[優先度]](priority.md)</span><span class="sxs-lookup"><span data-stu-id="55361-117">[Priority](priority.md)</span></span> <br/> |<span data-ttu-id="55361-118">ルールを実行する順序を示します。</span><span class="sxs-lookup"><span data-stu-id="55361-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="55361-119">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="55361-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="55361-120">ルールが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="55361-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="55361-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="55361-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="55361-122">マネージコード Api でルールを変更できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="55361-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="55361-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="55361-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="55361-124">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="55361-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="55361-125">条件</span><span class="sxs-lookup"><span data-stu-id="55361-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="55361-126">[処理時] がルールのルールの処理をトリガーする条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="55361-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="55361-127">例外</span><span class="sxs-lookup"><span data-stu-id="55361-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="55361-128">受信トレイルールの使用可能なルールの例外条件をすべて表す例外を識別します。</span><span class="sxs-lookup"><span data-stu-id="55361-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="55361-129">Actions</span><span class="sxs-lookup"><span data-stu-id="55361-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="55361-130">条件が満たされたときにメッセージに対して実行されるアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="55361-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55361-131">親要素</span><span class="sxs-lookup"><span data-stu-id="55361-131">Parent elements</span></span>

|<span data-ttu-id="55361-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="55361-132">**Element**</span></span>|<span data-ttu-id="55361-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="55361-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55361-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="55361-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="55361-135">新しいルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="55361-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="55361-136">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="55361-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="55361-137">ユーザーのメールボックス内のルールの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="55361-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="55361-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="55361-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="55361-139">既存のルールを更新する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="55361-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55361-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55361-140">Text value</span></span>

<span data-ttu-id="55361-141">なし。</span><span class="sxs-lookup"><span data-stu-id="55361-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55361-142">注釈</span><span class="sxs-lookup"><span data-stu-id="55361-142">Remarks</span></span>

<span data-ttu-id="55361-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="55361-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55361-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="55361-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55361-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="55361-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55361-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55361-146">Schema Name</span></span>  <br/> |<span data-ttu-id="55361-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="55361-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="55361-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55361-148">Validation File</span></span>  <br/> |<span data-ttu-id="55361-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="55361-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55361-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="55361-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="55361-151">正しい</span><span class="sxs-lookup"><span data-stu-id="55361-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55361-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="55361-152">See also</span></span>



[<span data-ttu-id="55361-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="55361-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="55361-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="55361-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="55361-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="55361-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="55361-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="55361-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

