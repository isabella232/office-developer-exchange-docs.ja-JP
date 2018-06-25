---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: InboxRules 要素は、ユーザーのメールボックスのルールの配列を表します。
ms.openlocfilehash: 47fcad5dde06f3af9fbae7e70adbfd8b225081c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831899"
---
# <a name="inboxrules"></a><span data-ttu-id="d71a2-103">InboxRules</span><span class="sxs-lookup"><span data-stu-id="d71a2-103">InboxRules</span></span>

<span data-ttu-id="d71a2-104">**InboxRules**要素は、ユーザーのメールボックスのルールの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="d71a2-104">The **InboxRules** element represents an array of rules in the user's mailbox.</span></span> 
  
[<span data-ttu-id="d71a2-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="d71a2-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="d71a2-106">InboxRules</span><span class="sxs-lookup"><span data-stu-id="d71a2-106">InboxRules</span></span>](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 <span data-ttu-id="d71a2-107">**ArrayOfRulesType**</span><span class="sxs-lookup"><span data-stu-id="d71a2-107">**ArrayOfRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d71a2-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d71a2-108">Attributes and elements</span></span>

<span data-ttu-id="d71a2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d71a2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d71a2-110">属性</span><span class="sxs-lookup"><span data-stu-id="d71a2-110">Attributes</span></span>

<span data-ttu-id="d71a2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d71a2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d71a2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d71a2-112">Child elements</span></span>

|<span data-ttu-id="d71a2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d71a2-113">**Element**</span></span>|<span data-ttu-id="d71a2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d71a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d71a2-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="d71a2-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="d71a2-116">1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="d71a2-116">Contains a single rule and represents a rule in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d71a2-117">親要素</span><span class="sxs-lookup"><span data-stu-id="d71a2-117">Parent elements</span></span>

|<span data-ttu-id="d71a2-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="d71a2-118">**Element**</span></span>|<span data-ttu-id="d71a2-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d71a2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d71a2-120">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="d71a2-120">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="d71a2-121">[GetInboxRules 操作](getinboxrules-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d71a2-121">Defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d71a2-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d71a2-122">Text value</span></span>

<span data-ttu-id="d71a2-123">なし。</span><span class="sxs-lookup"><span data-stu-id="d71a2-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d71a2-124">備考</span><span class="sxs-lookup"><span data-stu-id="d71a2-124">Remarks</span></span>

<span data-ttu-id="d71a2-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d71a2-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d71a2-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="d71a2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d71a2-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="d71a2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d71a2-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d71a2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d71a2-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d71a2-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d71a2-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d71a2-130">Validation File</span></span>  <br/> |<span data-ttu-id="d71a2-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d71a2-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d71a2-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d71a2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d71a2-133">True</span><span class="sxs-lookup"><span data-stu-id="d71a2-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d71a2-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="d71a2-134">See also</span></span>



[<span data-ttu-id="d71a2-135">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="d71a2-135">GetInboxRules</span></span>](getinboxrules.md)
  
[<span data-ttu-id="d71a2-136">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="d71a2-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)


- [<span data-ttu-id="d71a2-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d71a2-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

