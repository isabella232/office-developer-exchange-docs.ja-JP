---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: RuleOperationErrors 要素は、エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。
ms.openlocfilehash: d547155f3cbf9eedd0f9bfac7bf3768b3630b50e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464953"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="6af2f-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="6af2f-103">RuleOperationErrors</span></span>

<span data-ttu-id="6af2f-104">**Ruleoperationerrors**要素は、エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="6af2f-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="6af2f-105">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="6af2f-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="6af2f-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="6af2f-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="6af2f-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="6af2f-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6af2f-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6af2f-108">Attributes and elements</span></span>

<span data-ttu-id="6af2f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6af2f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6af2f-110">属性</span><span class="sxs-lookup"><span data-stu-id="6af2f-110">Attributes</span></span>

<span data-ttu-id="6af2f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6af2f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6af2f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6af2f-112">Child elements</span></span>

|<span data-ttu-id="6af2f-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="6af2f-113">**Element**</span></span>|<span data-ttu-id="6af2f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6af2f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6af2f-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="6af2f-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="6af2f-116">ルール操作エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="6af2f-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6af2f-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6af2f-117">Parent elements</span></span>

|<span data-ttu-id="6af2f-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="6af2f-118">**Element**</span></span>|<span data-ttu-id="6af2f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6af2f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6af2f-120">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="6af2f-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="6af2f-121">[Update受信トレイルール](updateinboxrules.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="6af2f-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6af2f-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6af2f-122">Text value</span></span>

<span data-ttu-id="6af2f-123">なし。</span><span class="sxs-lookup"><span data-stu-id="6af2f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6af2f-124">注釈</span><span class="sxs-lookup"><span data-stu-id="6af2f-124">Remarks</span></span>

<span data-ttu-id="6af2f-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6af2f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6af2f-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6af2f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6af2f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="6af2f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6af2f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6af2f-128">Schema name</span></span>  <br/> |<span data-ttu-id="6af2f-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6af2f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6af2f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6af2f-130">Validation file</span></span>  <br/> |<span data-ttu-id="6af2f-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6af2f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6af2f-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6af2f-132">Can be empty</span></span>  <br/> |<span data-ttu-id="6af2f-133">正しい</span><span class="sxs-lookup"><span data-stu-id="6af2f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6af2f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="6af2f-134">See also</span></span>



[<span data-ttu-id="6af2f-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6af2f-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="6af2f-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6af2f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

