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
description: WithinSizeRange 要素は、受信メッセージは、適用の条件または例外のためにする必要がある最小値と最大サイズを指定します。
ms.openlocfilehash: 7711db9ca68f972f080c98197e30c7710620119a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840033"
---
# <a name="withinsizerange"></a><span data-ttu-id="ff773-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="ff773-103">WithinSizeRange</span></span>

<span data-ttu-id="ff773-104">**WithinSizeRange**要素は、受信メッセージは、適用の条件または例外のためにする必要がある最小値と最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="ff773-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="ff773-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="ff773-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff773-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ff773-106">Attributes and elements</span></span>

<span data-ttu-id="ff773-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff773-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff773-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff773-108">Attributes</span></span>

<span data-ttu-id="ff773-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff773-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff773-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff773-110">Child elements</span></span>

|<span data-ttu-id="ff773-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff773-111">**Element**</span></span>|<span data-ttu-id="ff773-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff773-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff773-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="ff773-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="ff773-114">適用する場合の条件または例外の順序でメッセージをする必要がある最小サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="ff773-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="ff773-115">作成</span><span class="sxs-lookup"><span data-stu-id="ff773-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="ff773-116">メッセージ内に含まれる条件や例外条件を適用する順序の最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="ff773-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff773-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ff773-117">Parent elements</span></span>

|<span data-ttu-id="ff773-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff773-118">**Element**</span></span>|<span data-ttu-id="ff773-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff773-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff773-120">条件</span><span class="sxs-lookup"><span data-stu-id="ff773-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="ff773-121">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="ff773-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="ff773-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ff773-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="ff773-123">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="ff773-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff773-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ff773-124">Text value</span></span>

<span data-ttu-id="ff773-125">なし。</span><span class="sxs-lookup"><span data-stu-id="ff773-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff773-126">備考</span><span class="sxs-lookup"><span data-stu-id="ff773-126">Remarks</span></span>

<span data-ttu-id="ff773-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff773-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff773-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="ff773-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff773-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="ff773-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff773-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff773-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ff773-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff773-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff773-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff773-132">Validation File</span></span>  <br/> |<span data-ttu-id="ff773-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff773-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff773-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff773-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff773-135">True</span><span class="sxs-lookup"><span data-stu-id="ff773-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff773-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff773-136">See also</span></span>



- [<span data-ttu-id="ff773-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff773-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

