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
description: WithinDateRange 要素は、条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。
ms.openlocfilehash: ef5fb15b64ee4f7060f907818c4ebd4367ced5e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461850"
---
# <a name="withindaterange"></a><span data-ttu-id="753de-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="753de-103">WithinDateRange</span></span>

<span data-ttu-id="753de-104">**WithinDateRange**要素は、条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="753de-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="753de-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="753de-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="753de-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="753de-106">Attributes and elements</span></span>

<span data-ttu-id="753de-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="753de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="753de-108">属性</span><span class="sxs-lookup"><span data-stu-id="753de-108">Attributes</span></span>

<span data-ttu-id="753de-109">なし。</span><span class="sxs-lookup"><span data-stu-id="753de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="753de-110">子要素</span><span class="sxs-lookup"><span data-stu-id="753de-110">Child elements</span></span>

|<span data-ttu-id="753de-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="753de-111">**Element**</span></span>|<span data-ttu-id="753de-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="753de-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="753de-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="753de-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="753de-114">ルールの期間を指定します。この値の後にルールの条件が満たされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="753de-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="753de-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="753de-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="753de-116">ルールの期間を指定します。この値より前にルールの条件が満たされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="753de-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="753de-117">親要素</span><span class="sxs-lookup"><span data-stu-id="753de-117">Parent elements</span></span>

|<span data-ttu-id="753de-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="753de-118">**Element**</span></span>|<span data-ttu-id="753de-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="753de-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="753de-120">条件</span><span class="sxs-lookup"><span data-stu-id="753de-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="753de-121">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="753de-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="753de-122">例外</span><span class="sxs-lookup"><span data-stu-id="753de-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="753de-123">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="753de-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="753de-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="753de-124">Text value</span></span>

<span data-ttu-id="753de-125">なし。</span><span class="sxs-lookup"><span data-stu-id="753de-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="753de-126">注釈</span><span class="sxs-lookup"><span data-stu-id="753de-126">Remarks</span></span>

<span data-ttu-id="753de-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="753de-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="753de-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="753de-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="753de-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="753de-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="753de-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="753de-130">Schema Name</span></span>  <br/> |<span data-ttu-id="753de-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="753de-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="753de-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="753de-132">Validation File</span></span>  <br/> |<span data-ttu-id="753de-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="753de-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="753de-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="753de-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="753de-135">正しい</span><span class="sxs-lookup"><span data-stu-id="753de-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="753de-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="753de-136">See also</span></span>



- [<span data-ttu-id="753de-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="753de-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

