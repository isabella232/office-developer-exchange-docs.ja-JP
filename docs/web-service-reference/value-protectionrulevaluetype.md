---
title: Value (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Value 要素は、1人の受信者または送信者の部署を識別します。
ms.openlocfilehash: 908ea451800abc343fb6e4d4a4ed98d57223bd23
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465241"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="39e2d-103">Value (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="39e2d-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="39e2d-104">**Value**要素は、1人の受信者または送信者の部署を識別します。</span><span class="sxs-lookup"><span data-stu-id="39e2d-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="39e2d-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="39e2d-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="39e2d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="39e2d-106">Attributes and elements</span></span>

<span data-ttu-id="39e2d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="39e2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39e2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="39e2d-108">Attributes</span></span>

<span data-ttu-id="39e2d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="39e2d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39e2d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="39e2d-110">Child elements</span></span>

<span data-ttu-id="39e2d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="39e2d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="39e2d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="39e2d-112">Parent elements</span></span>

|<span data-ttu-id="39e2d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="39e2d-113">**Element**</span></span>|<span data-ttu-id="39e2d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="39e2d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39e2d-115">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="39e2d-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="39e2d-116">電子メールメッセージのすべての受信者が、子の**値**要素内の指定された受信者のいずれかと一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="39e2d-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="39e2d-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="39e2d-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="39e2d-118">送信者の部署が、子の**値**要素で指定された各部に一致することを指定します。</span><span class="sxs-lookup"><span data-stu-id="39e2d-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="39e2d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="39e2d-119">Text value</span></span>

<span data-ttu-id="39e2d-120">この要素には、空でない文字列値を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="39e2d-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39e2d-121">注釈</span><span class="sxs-lookup"><span data-stu-id="39e2d-121">Remarks</span></span>

<span data-ttu-id="39e2d-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="39e2d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39e2d-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="39e2d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39e2d-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="39e2d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="39e2d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="39e2d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="39e2d-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="39e2d-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="39e2d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="39e2d-127">Validation File</span></span>  <br/> |<span data-ttu-id="39e2d-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="39e2d-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="39e2d-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="39e2d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="39e2d-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="39e2d-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39e2d-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="39e2d-131">See also</span></span>

- [<span data-ttu-id="39e2d-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="39e2d-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

