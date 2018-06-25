---
title: WithinDateRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinDateRange
api_type:
- schema
ms.assetid: 226aeb15-016f-45ca-992a-c137ba09ca08
description: WithinDateRange 要素は、受信メッセージが適用の条件または例外のために到着したが、日付の範囲を指定します。
ms.openlocfilehash: d85ef91c581008c2aafb06b1900c4514aebacd65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840025"
---
# <a name="withindaterange"></a><span data-ttu-id="9e7e9-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="9e7e9-103">WithinDateRange</span></span>

<span data-ttu-id="9e7e9-104">**WithinDateRange**要素は、受信メッセージが適用の条件または例外のために到着したが、日付の範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="9e7e9-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="9e7e9-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e7e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9e7e9-106">Attributes and elements</span></span>

<span data-ttu-id="9e7e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e7e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e7e9-108">Attributes</span></span>

<span data-ttu-id="9e7e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e7e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e7e9-110">Child elements</span></span>

|<span data-ttu-id="9e7e9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e7e9-111">**Element**</span></span>|<span data-ttu-id="9e7e9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e7e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e7e9-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7e9-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="9e7e9-114">ルールの時間帯を指定し、この値の後にルールの条件が満たされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="9e7e9-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7e9-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="9e7e9-116">ルールの時間帯を指定し、この値の前にルールの条件が満たされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e7e9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="9e7e9-117">Parent elements</span></span>

|<span data-ttu-id="9e7e9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e7e9-118">**Element**</span></span>|<span data-ttu-id="9e7e9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e7e9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e7e9-120">条件</span><span class="sxs-lookup"><span data-stu-id="9e7e9-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="9e7e9-121">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="9e7e9-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="9e7e9-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="9e7e9-123">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e7e9-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e7e9-124">Text value</span></span>

<span data-ttu-id="9e7e9-125">なし。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e7e9-126">備考</span><span class="sxs-lookup"><span data-stu-id="9e7e9-126">Remarks</span></span>

<span data-ttu-id="9e7e9-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e7e9-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e7e9-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="9e7e9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e7e9-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="9e7e9-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e7e9-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e7e9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9e7e9-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9e7e9-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e7e9-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e7e9-132">Validation File</span></span>  <br/> |<span data-ttu-id="9e7e9-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e7e9-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e7e9-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9e7e9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e7e9-135">True</span><span class="sxs-lookup"><span data-stu-id="9e7e9-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e7e9-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e7e9-136">See also</span></span>



- [<span data-ttu-id="9e7e9-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e7e9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

