---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: RuleOperationErrors 要素は、エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。
ms.openlocfilehash: 7dc85b5cd84af5ad00511a3df2b31ee3541e12b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833261"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="b0a60-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="b0a60-103">RuleOperationErrors</span></span>

<span data-ttu-id="b0a60-104">**RuleOperationErrors**要素は、エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="b0a60-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="b0a60-105">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="b0a60-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="b0a60-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="b0a60-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="b0a60-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="b0a60-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0a60-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b0a60-108">Attributes and elements</span></span>

<span data-ttu-id="b0a60-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0a60-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0a60-110">属性</span><span class="sxs-lookup"><span data-stu-id="b0a60-110">Attributes</span></span>

<span data-ttu-id="b0a60-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b0a60-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0a60-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b0a60-112">Child elements</span></span>

|<span data-ttu-id="b0a60-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0a60-113">**Element**</span></span>|<span data-ttu-id="b0a60-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0a60-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a60-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="b0a60-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="b0a60-116">ルール操作のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="b0a60-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0a60-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b0a60-117">Parent elements</span></span>

|<span data-ttu-id="b0a60-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0a60-118">**Element**</span></span>|<span data-ttu-id="b0a60-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0a60-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a60-120">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="b0a60-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="b0a60-121">[UpdateInboxRules](updateinboxrules.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b0a60-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0a60-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b0a60-122">Text value</span></span>

<span data-ttu-id="b0a60-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b0a60-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0a60-124">備考</span><span class="sxs-lookup"><span data-stu-id="b0a60-124">Remarks</span></span>

<span data-ttu-id="b0a60-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b0a60-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0a60-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b0a60-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0a60-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b0a60-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0a60-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0a60-128">Schema name</span></span>  <br/> |<span data-ttu-id="b0a60-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b0a60-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0a60-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0a60-130">Validation file</span></span>  <br/> |<span data-ttu-id="b0a60-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b0a60-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0a60-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b0a60-132">Can be empty</span></span>  <br/> |<span data-ttu-id="b0a60-133">True</span><span class="sxs-lookup"><span data-stu-id="b0a60-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0a60-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0a60-134">See also</span></span>



[<span data-ttu-id="b0a60-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="b0a60-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="b0a60-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0a60-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

