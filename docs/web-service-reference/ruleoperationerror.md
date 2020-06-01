---
title: RuleOperationError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleOperationError
api_type:
- schema
ms.assetid: b447e610-d37c-40d3-9158-aa108a9f248e
description: RuleOperationError 要素は、ルール操作エラーを表します。
ms.openlocfilehash: b5e0105a1fdb1564b3115a4c3a8411019f725483
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464960"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="83520-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="83520-103">RuleOperationError</span></span>

<span data-ttu-id="83520-104">**Ruleoperationerror**要素は、ルール操作エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="83520-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="83520-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="83520-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83520-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="83520-106">Attributes and elements</span></span>

<span data-ttu-id="83520-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83520-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83520-108">属性</span><span class="sxs-lookup"><span data-stu-id="83520-108">Attributes</span></span>

<span data-ttu-id="83520-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83520-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83520-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83520-110">Child elements</span></span>

|<span data-ttu-id="83520-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="83520-111">**Element**</span></span>|<span data-ttu-id="83520-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="83520-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83520-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="83520-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="83520-114">ルールの操作エラーの原因となった、要求内の操作のインデックスを示します。</span><span class="sxs-lookup"><span data-stu-id="83520-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="83520-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="83520-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="83520-116">エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="83520-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83520-117">親要素</span><span class="sxs-lookup"><span data-stu-id="83520-117">Parent elements</span></span>

|<span data-ttu-id="83520-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="83520-118">**Element**</span></span>|<span data-ttu-id="83520-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="83520-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83520-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="83520-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="83520-121">エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="83520-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83520-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="83520-122">Text value</span></span>

<span data-ttu-id="83520-123">なし。</span><span class="sxs-lookup"><span data-stu-id="83520-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83520-124">注釈</span><span class="sxs-lookup"><span data-stu-id="83520-124">Remarks</span></span>

<span data-ttu-id="83520-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="83520-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83520-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="83520-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83520-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="83520-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83520-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83520-128">Schema Name</span></span>  <br/> |<span data-ttu-id="83520-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="83520-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83520-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83520-130">Validation File</span></span>  <br/> |<span data-ttu-id="83520-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="83520-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83520-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="83520-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="83520-133">正しい</span><span class="sxs-lookup"><span data-stu-id="83520-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83520-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="83520-134">See also</span></span>



- [<span data-ttu-id="83520-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="83520-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

