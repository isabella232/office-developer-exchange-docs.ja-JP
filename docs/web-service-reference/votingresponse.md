---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: VotingResponse 要素は、送信される投票を指定します。 この要素は、承認に対する応答に対してではなく、投票要求メッセージへの応答にのみ存在します。
ms.openlocfilehash: ed7caff79d1ff2946800630c167350fe866e29dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466466"
---
# <a name="votingresponse"></a><span data-ttu-id="54e04-104">VotingResponse</span><span class="sxs-lookup"><span data-stu-id="54e04-104">VotingResponse</span></span>

<span data-ttu-id="54e04-105">**VotingResponse**要素は、送信される投票を指定します。</span><span class="sxs-lookup"><span data-stu-id="54e04-105">The **VotingResponse** element specifies the submitted vote.</span></span> <span data-ttu-id="54e04-106">この要素は、承認に対する応答に対してではなく、投票要求メッセージへの応答にのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="54e04-106">This element is only present on responses to voting request messages, not on responses to approvals.</span></span> 
  
```XML
<VotingResponse />
```

 <span data-ttu-id="54e04-107">**string**</span><span class="sxs-lookup"><span data-stu-id="54e04-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54e04-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="54e04-108">Attributes and elements</span></span>

<span data-ttu-id="54e04-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54e04-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54e04-110">属性</span><span class="sxs-lookup"><span data-stu-id="54e04-110">Attributes</span></span>

<span data-ttu-id="54e04-111">なし。</span><span class="sxs-lookup"><span data-stu-id="54e04-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54e04-112">子要素</span><span class="sxs-lookup"><span data-stu-id="54e04-112">Child elements</span></span>

<span data-ttu-id="54e04-113">なし。</span><span class="sxs-lookup"><span data-stu-id="54e04-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54e04-114">親要素</span><span class="sxs-lookup"><span data-stu-id="54e04-114">Parent elements</span></span>

[<span data-ttu-id="54e04-115">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="54e04-115">VotingInformation</span></span>](votinginformation.md)
  
## <a name="text-value"></a><span data-ttu-id="54e04-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="54e04-116">Text value</span></span>

<span data-ttu-id="54e04-117">**VotingResponse**要素のテキスト値は、送信される投票です。</span><span class="sxs-lookup"><span data-stu-id="54e04-117">The text value of the **VotingResponse** element is the vote submitted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="54e04-118">注釈</span><span class="sxs-lookup"><span data-stu-id="54e04-118">Remarks</span></span>

<span data-ttu-id="54e04-119">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="54e04-119">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="54e04-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="54e04-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54e04-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="54e04-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54e04-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="54e04-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54e04-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54e04-123">Schema Name</span></span>  <br/> |<span data-ttu-id="54e04-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="54e04-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="54e04-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54e04-125">Validation File</span></span>  <br/> |<span data-ttu-id="54e04-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="54e04-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54e04-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="54e04-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="54e04-128">正しい</span><span class="sxs-lookup"><span data-stu-id="54e04-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54e04-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="54e04-129">See also</span></span>



[<span data-ttu-id="54e04-130">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="54e04-130">VotingInformation</span></span>](votinginformation.md)


- [<span data-ttu-id="54e04-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="54e04-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

