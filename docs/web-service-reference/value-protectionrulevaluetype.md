---
title: 値 (ProtectionRuleValueType)
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
description: 値要素は、1 つの受信者または送信者の部署を識別します。
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839975"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="0bcc4-103">値 (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="0bcc4-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="0bcc4-104">**値**要素は、1 つの受信者または送信者の部署を識別します。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="0bcc4-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="0bcc4-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0bcc4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0bcc4-106">Attributes and elements</span></span>

<span data-ttu-id="0bcc4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bcc4-108">属性</span><span class="sxs-lookup"><span data-stu-id="0bcc4-108">Attributes</span></span>

<span data-ttu-id="0bcc4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bcc4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0bcc4-110">Child elements</span></span>

<span data-ttu-id="0bcc4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bcc4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0bcc4-112">Parent elements</span></span>

|<span data-ttu-id="0bcc4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bcc4-113">**Element**</span></span>|<span data-ttu-id="0bcc4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bcc4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bcc4-115">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="0bcc4-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="0bcc4-116">電子メール メッセージの受信者と一致している**値**の子要素で指定した受信者のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="0bcc4-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="0bcc4-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="0bcc4-118">送信者の部署と一致している**値**の子要素で指定された部門のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bcc4-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0bcc4-119">Text value</span></span>

<span data-ttu-id="0bcc4-120">この要素は空でない文字列の値を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bcc4-121">備考</span><span class="sxs-lookup"><span data-stu-id="0bcc4-121">Remarks</span></span>

<span data-ttu-id="0bcc4-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0bcc4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bcc4-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="0bcc4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bcc4-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="0bcc4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bcc4-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bcc4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0bcc4-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0bcc4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bcc4-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bcc4-127">Validation File</span></span>  <br/> |<span data-ttu-id="0bcc4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bcc4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bcc4-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0bcc4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bcc4-130">False</span><span class="sxs-lookup"><span data-stu-id="0bcc4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bcc4-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bcc4-131">See also</span></span>

- [<span data-ttu-id="0bcc4-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0bcc4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

