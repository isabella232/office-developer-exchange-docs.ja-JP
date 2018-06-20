---
title: エラー コード
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: エラー コード要素は、失敗した内容を説明するルールの検証のエラー コードを表すルール述語またはアクションごとに検証します。
ms.openlocfilehash: ed8e2fa72b0eb007925742e6d194f3a391b3f3cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760326"
---
# <a name="errorcode"></a><span data-ttu-id="390ee-103">エラー コード</span><span class="sxs-lookup"><span data-stu-id="390ee-103">ErrorCode</span></span>

<span data-ttu-id="390ee-104">**エラー コード**要素は、失敗した内容を説明するルールの検証のエラー コードを表すルール述語またはアクションごとに検証します。</span><span class="sxs-lookup"><span data-stu-id="390ee-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="390ee-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="390ee-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="390ee-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="390ee-106">Attributes and elements</span></span>

<span data-ttu-id="390ee-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="390ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="390ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="390ee-108">Attributes</span></span>

<span data-ttu-id="390ee-109">なし。</span><span class="sxs-lookup"><span data-stu-id="390ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="390ee-110">子要素</span><span class="sxs-lookup"><span data-stu-id="390ee-110">Child elements</span></span>

<span data-ttu-id="390ee-111">なし。</span><span class="sxs-lookup"><span data-stu-id="390ee-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="390ee-112">親要素</span><span class="sxs-lookup"><span data-stu-id="390ee-112">Parent elements</span></span>

|<span data-ttu-id="390ee-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="390ee-113">**Element**</span></span>|<span data-ttu-id="390ee-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="390ee-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="390ee-115">Error</span><span class="sxs-lookup"><span data-stu-id="390ee-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="390ee-116">特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="390ee-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="390ee-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="390ee-117">Text value</span></span>

<span data-ttu-id="390ee-118">この要素のテキスト値は、次の文字列のいずれかに制限されています。</span><span class="sxs-lookup"><span data-stu-id="390ee-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="390ee-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="390ee-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="390ee-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="390ee-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="390ee-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="390ee-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="390ee-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="390ee-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="390ee-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="390ee-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="390ee-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="390ee-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="390ee-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="390ee-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="390ee-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="390ee-126">InvalidAddress</span></span>
    
- <span data-ttu-id="390ee-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="390ee-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="390ee-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="390ee-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="390ee-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="390ee-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="390ee-130">数量</span><span class="sxs-lookup"><span data-stu-id="390ee-130">InvalidValue</span></span>
    
- <span data-ttu-id="390ee-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="390ee-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="390ee-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="390ee-132">MissingAction</span></span>
    
- <span data-ttu-id="390ee-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="390ee-133">MissingParameter</span></span>
    
- <span data-ttu-id="390ee-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="390ee-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="390ee-135">NotSettable</span><span class="sxs-lookup"><span data-stu-id="390ee-135">NotSettable</span></span>
    
- <span data-ttu-id="390ee-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="390ee-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="390ee-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="390ee-137">RuleNotFound</span></span>
    
- <span data-ttu-id="390ee-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="390ee-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="390ee-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="390ee-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="390ee-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="390ee-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="390ee-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="390ee-141">UnexpectedError</span></span>
    
- <span data-ttu-id="390ee-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="390ee-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="390ee-143">備考</span><span class="sxs-lookup"><span data-stu-id="390ee-143">Remarks</span></span>

<span data-ttu-id="390ee-144">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="390ee-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="390ee-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="390ee-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="390ee-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="390ee-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="390ee-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="390ee-147">Schema Name</span></span>  <br/> |<span data-ttu-id="390ee-148">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="390ee-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="390ee-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="390ee-149">Validation File</span></span>  <br/> |<span data-ttu-id="390ee-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="390ee-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="390ee-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="390ee-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="390ee-152">False</span><span class="sxs-lookup"><span data-stu-id="390ee-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="390ee-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="390ee-153">See also</span></span>



- [<span data-ttu-id="390ee-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="390ee-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

