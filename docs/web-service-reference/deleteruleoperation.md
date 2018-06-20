---
title: DeleteRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: DeleteRuleOperation 要素には、既存の受信トレイ ルールを削除する操作が含まれています。
ms.openlocfilehash: 3410361e0b896fb0ef01c1873c9f8b0ac99afe58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759993"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="18086-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="18086-103">DeleteRuleOperation</span></span>

<span data-ttu-id="18086-104">**DeleteRuleOperation**要素には、既存の受信トレイ ルールを削除する操作が含まれています。</span><span class="sxs-lookup"><span data-stu-id="18086-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="18086-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="18086-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="18086-106">Operations</span><span class="sxs-lookup"><span data-stu-id="18086-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="18086-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="18086-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18086-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18086-108">Attributes and elements</span></span>

<span data-ttu-id="18086-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18086-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18086-110">属性</span><span class="sxs-lookup"><span data-stu-id="18086-110">Attributes</span></span>

<span data-ttu-id="18086-111">なし。</span><span class="sxs-lookup"><span data-stu-id="18086-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18086-112">子要素</span><span class="sxs-lookup"><span data-stu-id="18086-112">Child elements</span></span>

|<span data-ttu-id="18086-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="18086-113">**Element**</span></span>|<span data-ttu-id="18086-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="18086-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18086-115">規則 Id</span><span class="sxs-lookup"><span data-stu-id="18086-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="18086-116">削除する規則の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="18086-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18086-117">親要素</span><span class="sxs-lookup"><span data-stu-id="18086-117">Parent elements</span></span>

|<span data-ttu-id="18086-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="18086-118">**Element**</span></span>|<span data-ttu-id="18086-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="18086-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18086-120">Operations</span><span class="sxs-lookup"><span data-stu-id="18086-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="18086-121">受信トレイ ルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="18086-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18086-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18086-122">Text value</span></span>

<span data-ttu-id="18086-123">なし。</span><span class="sxs-lookup"><span data-stu-id="18086-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18086-124">備考</span><span class="sxs-lookup"><span data-stu-id="18086-124">Remarks</span></span>

<span data-ttu-id="18086-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18086-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18086-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="18086-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18086-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="18086-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18086-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18086-128">Schema Name</span></span>  <br/> |<span data-ttu-id="18086-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="18086-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="18086-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18086-130">Validation File</span></span>  <br/> |<span data-ttu-id="18086-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18086-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18086-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18086-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="18086-133">False</span><span class="sxs-lookup"><span data-stu-id="18086-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18086-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="18086-134">See also</span></span>

- [<span data-ttu-id="18086-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="18086-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="18086-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="18086-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="18086-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="18086-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="18086-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18086-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

