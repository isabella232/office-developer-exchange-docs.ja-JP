---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: SendPrompt 要素は、返信のオプションで使用できるアクションの種類を指定します。
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833346"
---
# <a name="sendprompt"></a><span data-ttu-id="673c2-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="673c2-103">SendPrompt</span></span>

<span data-ttu-id="673c2-104">**SendPrompt**要素は、返信のオプションで使用できるアクションの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="673c2-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="673c2-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="673c2-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="673c2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="673c2-106">Attributes and elements</span></span>

<span data-ttu-id="673c2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="673c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="673c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="673c2-108">Attributes</span></span>

<span data-ttu-id="673c2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="673c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="673c2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="673c2-110">Child elements</span></span>

<span data-ttu-id="673c2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="673c2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="673c2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="673c2-112">Parent elements</span></span>

[<span data-ttu-id="673c2-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="673c2-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="673c2-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="673c2-114">Text value</span></span>

<span data-ttu-id="673c2-115">**SendPrompt**要素のテキスト値は、返信のオプション操作です。</span><span class="sxs-lookup"><span data-stu-id="673c2-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="673c2-116">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="673c2-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="673c2-117">**値**</span><span class="sxs-lookup"><span data-stu-id="673c2-117">**Value**</span></span>|<span data-ttu-id="673c2-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="673c2-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="673c2-119">なし</span><span class="sxs-lookup"><span data-stu-id="673c2-119">None</span></span>  <br/> |<span data-ttu-id="673c2-120">操作はありません。</span><span class="sxs-lookup"><span data-stu-id="673c2-120">No action.</span></span>  <br/> |
|<span data-ttu-id="673c2-121">送信</span><span class="sxs-lookup"><span data-stu-id="673c2-121">Send</span></span>  <br/> |<span data-ttu-id="673c2-122">応答が直ちに送信されます。</span><span class="sxs-lookup"><span data-stu-id="673c2-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="673c2-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="673c2-123">VotingOption</span></span>  <br/> |<span data-ttu-id="673c2-124">承認者は、承認または却下の中にコメントを入力できます。</span><span class="sxs-lookup"><span data-stu-id="673c2-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="673c2-125">備考</span><span class="sxs-lookup"><span data-stu-id="673c2-125">Remarks</span></span>

<span data-ttu-id="673c2-126">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="673c2-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="673c2-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="673c2-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="673c2-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="673c2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="673c2-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="673c2-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="673c2-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="673c2-130">Schema Name</span></span>  <br/> |<span data-ttu-id="673c2-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="673c2-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="673c2-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="673c2-132">Validation File</span></span>  <br/> |<span data-ttu-id="673c2-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="673c2-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="673c2-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="673c2-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="673c2-135">True</span><span class="sxs-lookup"><span data-stu-id="673c2-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="673c2-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="673c2-136">See also</span></span>



[<span data-ttu-id="673c2-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="673c2-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="673c2-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="673c2-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

