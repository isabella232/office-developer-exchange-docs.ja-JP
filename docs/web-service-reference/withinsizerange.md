---
title: WithinSizeRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: WithinSizeRange 要素は、条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。
ms.openlocfilehash: 31da5815b70e20c47594da89b0b7ccab87eaf8f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459743"
---
# <a name="withinsizerange"></a><span data-ttu-id="4584b-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="4584b-103">WithinSizeRange</span></span>

<span data-ttu-id="4584b-104">**WithinSizeRange**要素は、条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="4584b-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="4584b-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="4584b-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4584b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4584b-106">Attributes and elements</span></span>

<span data-ttu-id="4584b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4584b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4584b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4584b-108">Attributes</span></span>

<span data-ttu-id="4584b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4584b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4584b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4584b-110">Child elements</span></span>

|<span data-ttu-id="4584b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4584b-111">**Element**</span></span>|<span data-ttu-id="4584b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4584b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4584b-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="4584b-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="4584b-114">条件または例外を適用するために、メッセージが必要な最小サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="4584b-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="4584b-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="4584b-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="4584b-116">条件または例外を適用するためにメッセージが必要とされる最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="4584b-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4584b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4584b-117">Parent elements</span></span>

|<span data-ttu-id="4584b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="4584b-118">**Element**</span></span>|<span data-ttu-id="4584b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4584b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4584b-120">条件</span><span class="sxs-lookup"><span data-stu-id="4584b-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="4584b-121">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="4584b-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="4584b-122">例外</span><span class="sxs-lookup"><span data-stu-id="4584b-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="4584b-123">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="4584b-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4584b-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4584b-124">Text value</span></span>

<span data-ttu-id="4584b-125">なし。</span><span class="sxs-lookup"><span data-stu-id="4584b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4584b-126">注釈</span><span class="sxs-lookup"><span data-stu-id="4584b-126">Remarks</span></span>

<span data-ttu-id="4584b-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4584b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4584b-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4584b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4584b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="4584b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4584b-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4584b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4584b-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4584b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4584b-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4584b-132">Validation File</span></span>  <br/> |<span data-ttu-id="4584b-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4584b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4584b-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4584b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4584b-135">正しい</span><span class="sxs-lookup"><span data-stu-id="4584b-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4584b-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="4584b-136">See also</span></span>



- [<span data-ttu-id="4584b-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4584b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

