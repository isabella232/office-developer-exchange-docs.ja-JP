---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: VotingResponse 要素は、送信された投票を指定します。 この要素があるだけ返信要求メッセージへの応答で、承認への応答ではなく。
ms.openlocfilehash: 865b24a4f7ec1cc7b53d4928b04f071cddf5fbfc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839996"
---
# <a name="votingresponse"></a><span data-ttu-id="65d67-104">VotingResponse</span><span class="sxs-lookup"><span data-stu-id="65d67-104">VotingResponse</span></span>

<span data-ttu-id="65d67-105">**VotingResponse**要素は、送信された投票を指定します。</span><span class="sxs-lookup"><span data-stu-id="65d67-105">The **VotingResponse** element specifies the submitted vote.</span></span> <span data-ttu-id="65d67-106">この要素があるだけ返信要求メッセージへの応答で、承認への応答ではなく。</span><span class="sxs-lookup"><span data-stu-id="65d67-106">This element is only present on responses to voting request messages, not on responses to approvals.</span></span> 
  
```XML
<VotingResponse />
```

 <span data-ttu-id="65d67-107">**string**</span><span class="sxs-lookup"><span data-stu-id="65d67-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65d67-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="65d67-108">Attributes and elements</span></span>

<span data-ttu-id="65d67-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="65d67-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65d67-110">属性</span><span class="sxs-lookup"><span data-stu-id="65d67-110">Attributes</span></span>

<span data-ttu-id="65d67-111">なし。</span><span class="sxs-lookup"><span data-stu-id="65d67-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65d67-112">子要素</span><span class="sxs-lookup"><span data-stu-id="65d67-112">Child elements</span></span>

<span data-ttu-id="65d67-113">なし。</span><span class="sxs-lookup"><span data-stu-id="65d67-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="65d67-114">親要素</span><span class="sxs-lookup"><span data-stu-id="65d67-114">Parent elements</span></span>

[<span data-ttu-id="65d67-115">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="65d67-115">VotingInformation</span></span>](votinginformation.md)
  
## <a name="text-value"></a><span data-ttu-id="65d67-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="65d67-116">Text value</span></span>

<span data-ttu-id="65d67-117">**VotingResponse**要素のテキスト値は、票を送信します。</span><span class="sxs-lookup"><span data-stu-id="65d67-117">The text value of the **VotingResponse** element is the vote submitted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="65d67-118">備考</span><span class="sxs-lookup"><span data-stu-id="65d67-118">Remarks</span></span>

<span data-ttu-id="65d67-119">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="65d67-119">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="65d67-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="65d67-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65d67-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="65d67-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65d67-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="65d67-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65d67-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="65d67-123">Schema Name</span></span>  <br/> |<span data-ttu-id="65d67-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="65d67-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="65d67-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="65d67-125">Validation File</span></span>  <br/> |<span data-ttu-id="65d67-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65d67-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65d67-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="65d67-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="65d67-128">True</span><span class="sxs-lookup"><span data-stu-id="65d67-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65d67-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="65d67-129">See also</span></span>



[<span data-ttu-id="65d67-130">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="65d67-130">VotingInformation</span></span>](votinginformation.md)


- [<span data-ttu-id="65d67-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="65d67-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

