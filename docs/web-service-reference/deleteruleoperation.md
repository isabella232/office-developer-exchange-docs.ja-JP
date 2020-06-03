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
description: DeleteRuleOperation 要素には、既存の受信トレイルールを削除する操作が含まれています。
ms.openlocfilehash: 6b17f7f99f1fd9b9889db00fdf55fba5eef5aba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526922"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="7012e-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7012e-103">DeleteRuleOperation</span></span>

<span data-ttu-id="7012e-104">**DeleteRuleOperation**要素には、既存の受信トレイルールを削除する操作が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7012e-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="7012e-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7012e-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="7012e-106">Operations</span><span class="sxs-lookup"><span data-stu-id="7012e-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="7012e-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="7012e-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7012e-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7012e-108">Attributes and elements</span></span>

<span data-ttu-id="7012e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7012e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7012e-110">属性</span><span class="sxs-lookup"><span data-stu-id="7012e-110">Attributes</span></span>

<span data-ttu-id="7012e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7012e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7012e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7012e-112">Child elements</span></span>

|<span data-ttu-id="7012e-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="7012e-113">**Element**</span></span>|<span data-ttu-id="7012e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7012e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7012e-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="7012e-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="7012e-116">削除するルールの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="7012e-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7012e-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7012e-117">Parent elements</span></span>

|<span data-ttu-id="7012e-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7012e-118">**Element**</span></span>|<span data-ttu-id="7012e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7012e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7012e-120">Operations</span><span class="sxs-lookup"><span data-stu-id="7012e-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="7012e-121">受信トレイに対して実行できるルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7012e-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7012e-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7012e-122">Text value</span></span>

<span data-ttu-id="7012e-123">なし。</span><span class="sxs-lookup"><span data-stu-id="7012e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7012e-124">注釈</span><span class="sxs-lookup"><span data-stu-id="7012e-124">Remarks</span></span>

<span data-ttu-id="7012e-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7012e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7012e-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7012e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7012e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7012e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7012e-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7012e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7012e-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7012e-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7012e-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7012e-130">Validation File</span></span>  <br/> |<span data-ttu-id="7012e-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7012e-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7012e-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7012e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7012e-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="7012e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7012e-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7012e-134">See also</span></span>

- [<span data-ttu-id="7012e-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7012e-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="7012e-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7012e-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="7012e-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7012e-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="7012e-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7012e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

