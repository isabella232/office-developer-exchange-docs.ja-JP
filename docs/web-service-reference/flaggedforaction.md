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
description: FlaggedForAction 要素は、条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。
ms.openlocfilehash: f996dc4bcf30db32e1d73fb302ab137f0a6ad4d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466242"
---
# <a name="flaggedforaction"></a><span data-ttu-id="2bc93-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="2bc93-103">FlaggedForAction</span></span>

<span data-ttu-id="2bc93-104">**Flaggedforaction**要素は、条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="2bc93-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="2bc93-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="2bc93-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bc93-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2bc93-106">Attributes and elements</span></span>

<span data-ttu-id="2bc93-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2bc93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bc93-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bc93-108">Attributes</span></span>

<span data-ttu-id="2bc93-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2bc93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bc93-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2bc93-110">Child elements</span></span>

<span data-ttu-id="2bc93-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2bc93-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2bc93-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2bc93-112">Parent elements</span></span>

|<span data-ttu-id="2bc93-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2bc93-113">**Element**</span></span>|<span data-ttu-id="2bc93-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2bc93-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bc93-115">条件</span><span class="sxs-lookup"><span data-stu-id="2bc93-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="2bc93-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="2bc93-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="2bc93-117">例外</span><span class="sxs-lookup"><span data-stu-id="2bc93-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="2bc93-118">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="2bc93-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2bc93-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2bc93-119">Text value</span></span>

<span data-ttu-id="2bc93-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="2bc93-120">A text value is required.</span></span> <span data-ttu-id="2bc93-121">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2bc93-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="2bc93-122">任意</span><span class="sxs-lookup"><span data-stu-id="2bc93-122">Any</span></span>
    
- <span data-ttu-id="2bc93-123">コール</span><span class="sxs-lookup"><span data-stu-id="2bc93-123">Call</span></span>
    
- <span data-ttu-id="2bc93-124">交換</span><span class="sxs-lookup"><span data-stu-id="2bc93-124">DoNotForward</span></span>
    
- <span data-ttu-id="2bc93-125">フォローアップ</span><span class="sxs-lookup"><span data-stu-id="2bc93-125">FollowUp</span></span>
    
- <span data-ttu-id="2bc93-126">注意</span><span class="sxs-lookup"><span data-stu-id="2bc93-126">FYI</span></span>
    
- <span data-ttu-id="2bc93-127">転送</span><span class="sxs-lookup"><span data-stu-id="2bc93-127">Forward</span></span>
    
- <span data-ttu-id="2bc93-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="2bc93-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="2bc93-129">Read</span><span class="sxs-lookup"><span data-stu-id="2bc93-129">Read</span></span>
    
- <span data-ttu-id="2bc93-130">返信</span><span class="sxs-lookup"><span data-stu-id="2bc93-130">Reply</span></span>
    
- <span data-ttu-id="2bc93-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="2bc93-131">ReplyToAll</span></span>
    
- <span data-ttu-id="2bc93-132">レビュー</span><span class="sxs-lookup"><span data-stu-id="2bc93-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2bc93-133">注釈</span><span class="sxs-lookup"><span data-stu-id="2bc93-133">Remarks</span></span>

<span data-ttu-id="2bc93-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2bc93-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bc93-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2bc93-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bc93-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="2bc93-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2bc93-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2bc93-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2bc93-138">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2bc93-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2bc93-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2bc93-139">Validation File</span></span>  <br/> |<span data-ttu-id="2bc93-140">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2bc93-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bc93-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2bc93-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bc93-142">正しい</span><span class="sxs-lookup"><span data-stu-id="2bc93-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bc93-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bc93-143">See also</span></span>



- [<span data-ttu-id="2bc93-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2bc93-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

