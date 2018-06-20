---
title: ValidationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: ValidationErrors 要素は、エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。
ms.openlocfilehash: c95c8057ad2d16a314d33e3738553b495355fd76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839961"
---
# <a name="validationerrors"></a><span data-ttu-id="fc2ce-103">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="fc2ce-103">ValidationErrors</span></span>

<span data-ttu-id="fc2ce-104">**ValidationErrors**要素は、エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-104">The **ValidationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 <span data-ttu-id="fc2ce-105">**ArrayOfRuleValidationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="fc2ce-105">**ArrayOfRuleValidationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc2ce-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fc2ce-106">Attributes and elements</span></span>

<span data-ttu-id="fc2ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc2ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc2ce-108">Attributes</span></span>

<span data-ttu-id="fc2ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc2ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fc2ce-110">Child elements</span></span>

|<span data-ttu-id="fc2ce-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fc2ce-111">**Element**</span></span>|<span data-ttu-id="fc2ce-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fc2ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc2ce-113">Error</span><span class="sxs-lookup"><span data-stu-id="fc2ce-113">Error</span></span>](error.md) <br/> |<span data-ttu-id="fc2ce-114">特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します</span><span class="sxs-lookup"><span data-stu-id="fc2ce-114">Represents a single validation error on a particular rule property value, predicate property value, or action property value</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc2ce-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fc2ce-115">Parent elements</span></span>

|<span data-ttu-id="fc2ce-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="fc2ce-116">**Element**</span></span>|<span data-ttu-id="fc2ce-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="fc2ce-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc2ce-118">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="fc2ce-118">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="fc2ce-119">ルール操作のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-119">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc2ce-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fc2ce-120">Text value</span></span>

<span data-ttu-id="fc2ce-121">なし。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc2ce-122">備考</span><span class="sxs-lookup"><span data-stu-id="fc2ce-122">Remarks</span></span>

<span data-ttu-id="fc2ce-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fc2ce-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc2ce-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="fc2ce-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc2ce-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="fc2ce-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc2ce-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fc2ce-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fc2ce-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fc2ce-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc2ce-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fc2ce-128">Validation File</span></span>  <br/> |<span data-ttu-id="fc2ce-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc2ce-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc2ce-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fc2ce-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc2ce-131">True</span><span class="sxs-lookup"><span data-stu-id="fc2ce-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc2ce-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc2ce-132">See also</span></span>



- [<span data-ttu-id="fc2ce-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fc2ce-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

