---
title: FlaggedForAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: FlaggedForAction 要素を適用する場合の条件または例外の順序で受信したメッセージに表示する必要がありますアクションの値のフラグを指定します。
ms.openlocfilehash: 5b6e714512edcf12ded2c04f414d047b8622d305
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760555"
---
# <a name="flaggedforaction"></a><span data-ttu-id="559ab-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="559ab-103">FlaggedForAction</span></span>

<span data-ttu-id="559ab-104">**FlaggedForAction**要素を適用する場合の条件または例外の順序で受信したメッセージに表示する必要がありますアクションの値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="559ab-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="559ab-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="559ab-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="559ab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="559ab-106">Attributes and elements</span></span>

<span data-ttu-id="559ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="559ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="559ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="559ab-108">Attributes</span></span>

<span data-ttu-id="559ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="559ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="559ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="559ab-110">Child elements</span></span>

<span data-ttu-id="559ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="559ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="559ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="559ab-112">Parent elements</span></span>

|<span data-ttu-id="559ab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="559ab-113">**Element**</span></span>|<span data-ttu-id="559ab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="559ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="559ab-115">条件</span><span class="sxs-lookup"><span data-stu-id="559ab-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="559ab-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="559ab-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="559ab-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="559ab-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="559ab-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="559ab-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="559ab-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="559ab-119">Text value</span></span>

<span data-ttu-id="559ab-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="559ab-120">A text value is required.</span></span> <span data-ttu-id="559ab-121">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="559ab-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="559ab-122">Any</span><span class="sxs-lookup"><span data-stu-id="559ab-122">Any</span></span>
    
- <span data-ttu-id="559ab-123">Call</span><span class="sxs-lookup"><span data-stu-id="559ab-123">Call</span></span>
    
- <span data-ttu-id="559ab-124">DoNotForward</span><span class="sxs-lookup"><span data-stu-id="559ab-124">DoNotForward</span></span>
    
- <span data-ttu-id="559ab-125">FollowUp</span><span class="sxs-lookup"><span data-stu-id="559ab-125">FollowUp</span></span>
    
- <span data-ttu-id="559ab-126">FYI</span><span class="sxs-lookup"><span data-stu-id="559ab-126">FYI</span></span>
    
- <span data-ttu-id="559ab-127">Forward</span><span class="sxs-lookup"><span data-stu-id="559ab-127">Forward</span></span>
    
- <span data-ttu-id="559ab-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="559ab-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="559ab-129">Read</span><span class="sxs-lookup"><span data-stu-id="559ab-129">Read</span></span>
    
- <span data-ttu-id="559ab-130">Reply</span><span class="sxs-lookup"><span data-stu-id="559ab-130">Reply</span></span>
    
- <span data-ttu-id="559ab-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="559ab-131">ReplyToAll</span></span>
    
- <span data-ttu-id="559ab-132">Review</span><span class="sxs-lookup"><span data-stu-id="559ab-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="559ab-133">備考</span><span class="sxs-lookup"><span data-stu-id="559ab-133">Remarks</span></span>

<span data-ttu-id="559ab-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="559ab-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="559ab-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="559ab-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="559ab-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="559ab-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="559ab-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="559ab-137">Schema Name</span></span>  <br/> |<span data-ttu-id="559ab-138">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="559ab-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="559ab-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="559ab-139">Validation File</span></span>  <br/> |<span data-ttu-id="559ab-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="559ab-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="559ab-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="559ab-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="559ab-142">True</span><span class="sxs-lookup"><span data-stu-id="559ab-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="559ab-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="559ab-143">See also</span></span>



- [<span data-ttu-id="559ab-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="559ab-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

