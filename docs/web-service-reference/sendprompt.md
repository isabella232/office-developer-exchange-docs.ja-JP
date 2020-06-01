---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: SendPrompt 要素は、投票オプションに対して許可されるアクションの種類を指定します。
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462102"
---
# <a name="sendprompt"></a><span data-ttu-id="8eb6b-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="8eb6b-103">SendPrompt</span></span>

<span data-ttu-id="8eb6b-104">**Sendprompt**要素は、投票オプションに対して許可されるアクションの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="8eb6b-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="8eb6b-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8eb6b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8eb6b-106">Attributes and elements</span></span>

<span data-ttu-id="8eb6b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8eb6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8eb6b-108">Attributes</span></span>

<span data-ttu-id="8eb6b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8eb6b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8eb6b-110">Child elements</span></span>

<span data-ttu-id="8eb6b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8eb6b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8eb6b-112">Parent elements</span></span>

[<span data-ttu-id="8eb6b-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="8eb6b-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="8eb6b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8eb6b-114">Text value</span></span>

<span data-ttu-id="8eb6b-115">**Sendprompt**要素のテキスト値は、投票オプションのアクションです。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="8eb6b-116">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="8eb6b-117">**値**</span><span class="sxs-lookup"><span data-stu-id="8eb6b-117">**Value**</span></span>|<span data-ttu-id="8eb6b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8eb6b-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8eb6b-119">なし</span><span class="sxs-lookup"><span data-stu-id="8eb6b-119">None</span></span>  <br/> |<span data-ttu-id="8eb6b-120">何も実行しません。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-120">No action.</span></span>  <br/> |
|<span data-ttu-id="8eb6b-121">送信</span><span class="sxs-lookup"><span data-stu-id="8eb6b-121">Send</span></span>  <br/> |<span data-ttu-id="8eb6b-122">応答はすぐに送信されます。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="8eb6b-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="8eb6b-123">VotingOption</span></span>  <br/> |<span data-ttu-id="8eb6b-124">承認者は、承認または拒否の際にコメントを入力できます。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8eb6b-125">注釈</span><span class="sxs-lookup"><span data-stu-id="8eb6b-125">Remarks</span></span>

<span data-ttu-id="8eb6b-126">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="8eb6b-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8eb6b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8eb6b-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8eb6b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8eb6b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="8eb6b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8eb6b-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8eb6b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8eb6b-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8eb6b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8eb6b-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8eb6b-132">Validation File</span></span>  <br/> |<span data-ttu-id="8eb6b-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8eb6b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8eb6b-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8eb6b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8eb6b-135">正しい</span><span class="sxs-lookup"><span data-stu-id="8eb6b-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8eb6b-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="8eb6b-136">See also</span></span>



[<span data-ttu-id="8eb6b-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="8eb6b-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="8eb6b-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8eb6b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

