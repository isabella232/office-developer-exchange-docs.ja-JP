---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: ErrorCode 要素は、各ルール述語またはアクションの検証に失敗したことを示すルールの検証エラーコードを表します。
ms.openlocfilehash: 6432aeee786d74a9afcb346cb66765f9001257de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460079"
---
# <a name="errorcode"></a><span data-ttu-id="1ddca-103">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="1ddca-103">ErrorCode</span></span>

<span data-ttu-id="1ddca-104">**ErrorCode**要素は、各ルール述語またはアクションの検証に失敗したことを示すルールの検証エラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddca-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="1ddca-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="1ddca-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ddca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1ddca-106">Attributes and elements</span></span>

<span data-ttu-id="1ddca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ddca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ddca-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ddca-108">Attributes</span></span>

<span data-ttu-id="1ddca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1ddca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ddca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1ddca-110">Child elements</span></span>

<span data-ttu-id="1ddca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1ddca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ddca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1ddca-112">Parent elements</span></span>

|<span data-ttu-id="1ddca-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ddca-113">**Element**</span></span>|<span data-ttu-id="1ddca-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ddca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ddca-115">Error</span><span class="sxs-lookup"><span data-stu-id="1ddca-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="1ddca-116">特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddca-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ddca-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1ddca-117">Text value</span></span>

<span data-ttu-id="1ddca-118">この要素のテキスト値は、次の文字列のいずれかに制限されています。</span><span class="sxs-lookup"><span data-stu-id="1ddca-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="1ddca-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="1ddca-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="1ddca-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="1ddca-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="1ddca-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="1ddca-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="1ddca-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="1ddca-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="1ddca-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="1ddca-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="1ddca-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="1ddca-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="1ddca-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="1ddca-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="1ddca-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="1ddca-126">InvalidAddress</span></span>
    
- <span data-ttu-id="1ddca-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="1ddca-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="1ddca-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="1ddca-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="1ddca-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="1ddca-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="1ddca-130">InvalidValue</span><span class="sxs-lookup"><span data-stu-id="1ddca-130">InvalidValue</span></span>
    
- <span data-ttu-id="1ddca-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="1ddca-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="1ddca-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="1ddca-132">MissingAction</span></span>
    
- <span data-ttu-id="1ddca-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="1ddca-133">MissingParameter</span></span>
    
- <span data-ttu-id="1ddca-134">誤 Singrangevalue</span><span class="sxs-lookup"><span data-stu-id="1ddca-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="1ddca-135">NotSettable 可能</span><span class="sxs-lookup"><span data-stu-id="1ddca-135">NotSettable</span></span>
    
- <span data-ttu-id="1ddca-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="1ddca-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="1ddca-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="1ddca-137">RuleNotFound</span></span>
    
- <span data-ttu-id="1ddca-138">Sizeless0</span><span class="sxs-lookup"><span data-stu-id="1ddca-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="1ddca-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="1ddca-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="1ddca-140">アン Supportedaddress</span><span class="sxs-lookup"><span data-stu-id="1ddca-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="1ddca-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="1ddca-141">UnexpectedError</span></span>
    
- <span data-ttu-id="1ddca-142">アン Supportedrule</span><span class="sxs-lookup"><span data-stu-id="1ddca-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1ddca-143">注釈</span><span class="sxs-lookup"><span data-stu-id="1ddca-143">Remarks</span></span>

<span data-ttu-id="1ddca-144">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ddca-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ddca-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1ddca-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ddca-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ddca-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ddca-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ddca-147">Schema Name</span></span>  <br/> |<span data-ttu-id="1ddca-148">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ddca-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ddca-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ddca-149">Validation File</span></span>  <br/> |<span data-ttu-id="1ddca-150">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1ddca-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ddca-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ddca-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ddca-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="1ddca-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ddca-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ddca-153">See also</span></span>



- [<span data-ttu-id="1ddca-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ddca-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

