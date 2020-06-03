---
title: Error
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Error 要素は、特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460681"
---
# <a name="error"></a><span data-ttu-id="a1d8b-103">Error</span><span class="sxs-lookup"><span data-stu-id="a1d8b-103">Error</span></span>

<span data-ttu-id="a1d8b-104">**Error**要素は、特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="a1d8b-105">**RuleValidationErrorType**</span><span class="sxs-lookup"><span data-stu-id="a1d8b-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1d8b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a1d8b-106">Attributes and elements</span></span>

<span data-ttu-id="a1d8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1d8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1d8b-108">Attributes</span></span>

<span data-ttu-id="a1d8b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1d8b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a1d8b-110">Child elements</span></span>

|<span data-ttu-id="a1d8b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a1d8b-111">**Element**</span></span>|<span data-ttu-id="a1d8b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1d8b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d8b-113">FieldUri (ルール)</span><span class="sxs-lookup"><span data-stu-id="a1d8b-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="a1d8b-114">検証エラーの原因となったルールフィールドへの URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="a1d8b-115">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="a1d8b-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="a1d8b-116">ルールの述語またはアクションごとに、検証に失敗したことを示すルールの検証エラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="a1d8b-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="a1d8b-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="a1d8b-118">検証エラーの理由を表します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="a1d8b-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="a1d8b-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="a1d8b-120">検証エラーの原因となったフィールドの値を表します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1d8b-121">親要素</span><span class="sxs-lookup"><span data-stu-id="a1d8b-121">Parent elements</span></span>

|<span data-ttu-id="a1d8b-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="a1d8b-122">**Element**</span></span>|<span data-ttu-id="a1d8b-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1d8b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d8b-124">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="a1d8b-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="a1d8b-125">エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1d8b-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a1d8b-126">Text value</span></span>

<span data-ttu-id="a1d8b-127">なし。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1d8b-128">注釈</span><span class="sxs-lookup"><span data-stu-id="a1d8b-128">Remarks</span></span>

<span data-ttu-id="a1d8b-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a1d8b-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1d8b-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a1d8b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1d8b-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1d8b-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1d8b-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a1d8b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a1d8b-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a1d8b-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1d8b-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a1d8b-134">Validation File</span></span>  <br/> |<span data-ttu-id="a1d8b-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a1d8b-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1d8b-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a1d8b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1d8b-137">正しい</span><span class="sxs-lookup"><span data-stu-id="a1d8b-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1d8b-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1d8b-138">See also</span></span>



- [<span data-ttu-id="a1d8b-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a1d8b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

