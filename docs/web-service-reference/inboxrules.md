---
title: 受信トレイのルール
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
description: 受信トレイルール要素は、ユーザーのメールボックス内のルールの配列を表します。
ms.openlocfilehash: a3107c3c317a912d0bd3e60d03da4168f2f3a0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458272"
---
# <a name="inboxrules"></a><span data-ttu-id="cdfd8-103">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="cdfd8-103">InboxRules</span></span>

<span data-ttu-id="cdfd8-104">受信**トレイルール**要素は、ユーザーのメールボックス内のルールの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-104">The **InboxRules** element represents an array of rules in the user's mailbox.</span></span> 
  
[<span data-ttu-id="cdfd8-105">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="cdfd8-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="cdfd8-106">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="cdfd8-106">InboxRules</span></span>](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 <span data-ttu-id="cdfd8-107">**ArrayOfRulesType y**</span><span class="sxs-lookup"><span data-stu-id="cdfd8-107">**ArrayOfRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cdfd8-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cdfd8-108">Attributes and elements</span></span>

<span data-ttu-id="cdfd8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdfd8-110">属性</span><span class="sxs-lookup"><span data-stu-id="cdfd8-110">Attributes</span></span>

<span data-ttu-id="cdfd8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdfd8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="cdfd8-112">Child elements</span></span>

|<span data-ttu-id="cdfd8-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="cdfd8-113">**Element**</span></span>|<span data-ttu-id="cdfd8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cdfd8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdfd8-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="cdfd8-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="cdfd8-116">1つのルールを含み、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-116">Contains a single rule and represents a rule in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cdfd8-117">親要素</span><span class="sxs-lookup"><span data-stu-id="cdfd8-117">Parent elements</span></span>

|<span data-ttu-id="cdfd8-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="cdfd8-118">**Element**</span></span>|<span data-ttu-id="cdfd8-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="cdfd8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdfd8-120">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="cdfd8-120">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="cdfd8-121">[Get受信トレイルール操作](getinboxrules-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-121">Defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cdfd8-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cdfd8-122">Text value</span></span>

<span data-ttu-id="cdfd8-123">なし。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cdfd8-124">注釈</span><span class="sxs-lookup"><span data-stu-id="cdfd8-124">Remarks</span></span>

<span data-ttu-id="cdfd8-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cdfd8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdfd8-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cdfd8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdfd8-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cdfd8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cdfd8-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cdfd8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cdfd8-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cdfd8-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cdfd8-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cdfd8-130">Validation File</span></span>  <br/> |<span data-ttu-id="cdfd8-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cdfd8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cdfd8-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cdfd8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cdfd8-133">正しい</span><span class="sxs-lookup"><span data-stu-id="cdfd8-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cdfd8-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="cdfd8-134">See also</span></span>



[<span data-ttu-id="cdfd8-135">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="cdfd8-135">GetInboxRules</span></span>](getinboxrules.md)
  
[<span data-ttu-id="cdfd8-136">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="cdfd8-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)


- [<span data-ttu-id="cdfd8-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cdfd8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

