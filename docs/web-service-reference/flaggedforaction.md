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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466242"
---
# <a name="flaggedforaction"></a><span data-ttu-id="73c29-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="73c29-103">FlaggedForAction</span></span>

<span data-ttu-id="73c29-104">**Flaggedforaction**要素は、条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c29-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="73c29-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="73c29-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73c29-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="73c29-106">Attributes and elements</span></span>

<span data-ttu-id="73c29-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73c29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73c29-108">属性</span><span class="sxs-lookup"><span data-stu-id="73c29-108">Attributes</span></span>

<span data-ttu-id="73c29-109">なし。</span><span class="sxs-lookup"><span data-stu-id="73c29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73c29-110">子要素</span><span class="sxs-lookup"><span data-stu-id="73c29-110">Child elements</span></span>

<span data-ttu-id="73c29-111">なし。</span><span class="sxs-lookup"><span data-stu-id="73c29-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73c29-112">親要素</span><span class="sxs-lookup"><span data-stu-id="73c29-112">Parent elements</span></span>

|<span data-ttu-id="73c29-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="73c29-113">**Element**</span></span>|<span data-ttu-id="73c29-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="73c29-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73c29-115">条件</span><span class="sxs-lookup"><span data-stu-id="73c29-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="73c29-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="73c29-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="73c29-117">例外</span><span class="sxs-lookup"><span data-stu-id="73c29-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="73c29-118">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="73c29-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73c29-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="73c29-119">Text value</span></span>

<span data-ttu-id="73c29-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="73c29-120">A text value is required.</span></span> <span data-ttu-id="73c29-121">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="73c29-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="73c29-122">任意</span><span class="sxs-lookup"><span data-stu-id="73c29-122">Any</span></span>
    
- <span data-ttu-id="73c29-123">コール</span><span class="sxs-lookup"><span data-stu-id="73c29-123">Call</span></span>
    
- <span data-ttu-id="73c29-124">交換</span><span class="sxs-lookup"><span data-stu-id="73c29-124">DoNotForward</span></span>
    
- <span data-ttu-id="73c29-125">フォローアップ</span><span class="sxs-lookup"><span data-stu-id="73c29-125">FollowUp</span></span>
    
- <span data-ttu-id="73c29-126">注意</span><span class="sxs-lookup"><span data-stu-id="73c29-126">FYI</span></span>
    
- <span data-ttu-id="73c29-127">転送</span><span class="sxs-lookup"><span data-stu-id="73c29-127">Forward</span></span>
    
- <span data-ttu-id="73c29-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="73c29-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="73c29-129">Read</span><span class="sxs-lookup"><span data-stu-id="73c29-129">Read</span></span>
    
- <span data-ttu-id="73c29-130">返信</span><span class="sxs-lookup"><span data-stu-id="73c29-130">Reply</span></span>
    
- <span data-ttu-id="73c29-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="73c29-131">ReplyToAll</span></span>
    
- <span data-ttu-id="73c29-132">レビュー</span><span class="sxs-lookup"><span data-stu-id="73c29-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="73c29-133">注釈</span><span class="sxs-lookup"><span data-stu-id="73c29-133">Remarks</span></span>

<span data-ttu-id="73c29-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="73c29-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73c29-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="73c29-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73c29-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="73c29-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73c29-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73c29-137">Schema Name</span></span>  <br/> |<span data-ttu-id="73c29-138">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="73c29-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73c29-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73c29-139">Validation File</span></span>  <br/> |<span data-ttu-id="73c29-140">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="73c29-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73c29-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73c29-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="73c29-142">正しい</span><span class="sxs-lookup"><span data-stu-id="73c29-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73c29-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="73c29-143">See also</span></span>



- [<span data-ttu-id="73c29-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="73c29-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

