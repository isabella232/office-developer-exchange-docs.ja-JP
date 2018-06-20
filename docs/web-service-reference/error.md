---
title: エラー
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
description: エラー要素は、特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760321"
---
# <a name="error"></a><span data-ttu-id="281fb-103">エラー</span><span class="sxs-lookup"><span data-stu-id="281fb-103">Error</span></span>

<span data-ttu-id="281fb-104">**エラー**要素は、特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="281fb-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="281fb-105">**RuleValidationErrorType**</span><span class="sxs-lookup"><span data-stu-id="281fb-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="281fb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="281fb-106">Attributes and elements</span></span>

<span data-ttu-id="281fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="281fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="281fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="281fb-108">Attributes</span></span>

<span data-ttu-id="281fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="281fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="281fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="281fb-110">Child elements</span></span>

|<span data-ttu-id="281fb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="281fb-111">**Element**</span></span>|<span data-ttu-id="281fb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="281fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="281fb-113">FieldUri (ルール)</span><span class="sxs-lookup"><span data-stu-id="281fb-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="281fb-114">検証エラーの原因となったルール] フィールドに URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="281fb-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="281fb-115">エラー コード</span><span class="sxs-lookup"><span data-stu-id="281fb-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="281fb-116">失敗した内容を説明するルールの検証のエラー コードを表すルール述語またはアクションごとに検証します。</span><span class="sxs-lookup"><span data-stu-id="281fb-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="281fb-117">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="281fb-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="281fb-118">検証エラーの原因を表します。</span><span class="sxs-lookup"><span data-stu-id="281fb-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="281fb-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="281fb-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="281fb-120">検証エラーが発生したフィールドの値を表します。</span><span class="sxs-lookup"><span data-stu-id="281fb-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="281fb-121">親要素</span><span class="sxs-lookup"><span data-stu-id="281fb-121">Parent elements</span></span>

|<span data-ttu-id="281fb-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="281fb-122">**Element**</span></span>|<span data-ttu-id="281fb-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="281fb-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="281fb-124">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="281fb-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="281fb-125">エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="281fb-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="281fb-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="281fb-126">Text value</span></span>

<span data-ttu-id="281fb-127">なし。</span><span class="sxs-lookup"><span data-stu-id="281fb-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="281fb-128">備考</span><span class="sxs-lookup"><span data-stu-id="281fb-128">Remarks</span></span>

<span data-ttu-id="281fb-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="281fb-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="281fb-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="281fb-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="281fb-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="281fb-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="281fb-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="281fb-132">Schema Name</span></span>  <br/> |<span data-ttu-id="281fb-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="281fb-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="281fb-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="281fb-134">Validation File</span></span>  <br/> |<span data-ttu-id="281fb-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="281fb-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="281fb-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="281fb-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="281fb-137">True</span><span class="sxs-lookup"><span data-stu-id="281fb-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="281fb-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="281fb-138">See also</span></span>



- [<span data-ttu-id="281fb-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="281fb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

