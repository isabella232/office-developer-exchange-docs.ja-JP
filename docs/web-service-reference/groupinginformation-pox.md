---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: GroupingInformation 要素には、複数のメールボックス間での通知にサブスクライブしているときに、アフィニティを維持するためにユーザーのメールボックスをグループ化するために使用される値が含まれています。
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831781"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="6a3e6-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="6a3e6-104">**GroupingInformation**要素には、複数のメールボックスの間で、通知を購読する場合は、[アフィニティを維持](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するためにユーザーのメールボックスをグループ化するために使用される値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="6a3e6-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="6a3e6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6a3e6-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6a3e6-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6a3e6-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6a3e6-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6a3e6-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a3e6-110">Attributes and elements</span></span>

<span data-ttu-id="6a3e6-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a3e6-112">属性</span><span class="sxs-lookup"><span data-stu-id="6a3e6-112">Attributes</span></span>

<span data-ttu-id="6a3e6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a3e6-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6a3e6-114">Child elements</span></span>

<span data-ttu-id="6a3e6-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a3e6-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6a3e6-116">Parent elements</span></span>

|<span data-ttu-id="6a3e6-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a3e6-117">**Element**</span></span>|<span data-ttu-id="6a3e6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a3e6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a3e6-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6a3e6-120">クライアントを Exchange サーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a3e6-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a3e6-121">Text value</span></span>

<span data-ttu-id="6a3e6-122">テキスト値は、他のメールボックスの**GroupingInformation**要素の値と比較されます。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="6a3e6-123">メールボックスを同じ値を持つし、同一の Exchange Web サービス (EWS) のエンドポイントを使用してグループ化できるアフィニティを維持するためにします。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="6a3e6-124">詳細については、 [Exchange でのサブスクリプションのグループとメールボックス サーバー間のアフィニティを維持](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a3e6-125">備考</span><span class="sxs-lookup"><span data-stu-id="6a3e6-125">Remarks</span></span>

<span data-ttu-id="6a3e6-126">**GroupingInformation**要素では、EXPR の値を持つ[型 (POX)](type-pox.md)の子要素を持つ**プロトコル**要素に該当する場合のみ。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6a3e6-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a3e6-127">See also</span></span>

- [<span data-ttu-id="6a3e6-128">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a3e6-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="6a3e6-129">Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。</span><span class="sxs-lookup"><span data-stu-id="6a3e6-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

