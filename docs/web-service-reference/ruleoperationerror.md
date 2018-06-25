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
description: RuleOperationError 要素は、ルール処理のエラーを表します。
ms.openlocfilehash: ff42addea0f55b13794e2c910d4d865ad0b17bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833265"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="7f492-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="7f492-103">RuleOperationError</span></span>

<span data-ttu-id="7f492-104">**RuleOperationError**要素は、ルール処理のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="7f492-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="7f492-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="7f492-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f492-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f492-106">Attributes and elements</span></span>

<span data-ttu-id="7f492-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f492-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f492-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f492-108">Attributes</span></span>

<span data-ttu-id="7f492-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f492-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f492-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f492-110">Child elements</span></span>

|<span data-ttu-id="7f492-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f492-111">**Element**</span></span>|<span data-ttu-id="7f492-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f492-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f492-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="7f492-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="7f492-114">ルール操作エラーが発生した要求の処理のインデックスを示します。</span><span class="sxs-lookup"><span data-stu-id="7f492-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="7f492-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="7f492-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="7f492-116">エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="7f492-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f492-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7f492-117">Parent elements</span></span>

|<span data-ttu-id="7f492-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f492-118">**Element**</span></span>|<span data-ttu-id="7f492-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f492-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f492-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="7f492-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="7f492-121">エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="7f492-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f492-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f492-122">Text value</span></span>

<span data-ttu-id="7f492-123">なし。</span><span class="sxs-lookup"><span data-stu-id="7f492-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7f492-124">備考</span><span class="sxs-lookup"><span data-stu-id="7f492-124">Remarks</span></span>

<span data-ttu-id="7f492-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f492-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f492-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f492-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f492-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f492-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f492-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f492-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7f492-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f492-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f492-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f492-130">Validation File</span></span>  <br/> |<span data-ttu-id="7f492-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f492-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f492-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7f492-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f492-133">True</span><span class="sxs-lookup"><span data-stu-id="7f492-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f492-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f492-134">See also</span></span>



- [<span data-ttu-id="7f492-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7f492-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

