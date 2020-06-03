---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: GroupingInformation 要素には、ユーザーのメールボックスをグループ化して、複数のメールボックス間で通知をサブスクライブするときのアフィニティを維持するために使用される値が含まれています。
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530079"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="753f6-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="753f6-104">**Groupinginformation**要素には、ユーザーのメールボックスをグループ化して、複数のメールボックス間で通知をサブスクライブするときの[アフィニティを維持](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するために使用される値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="753f6-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="753f6-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="753f6-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="753f6-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="753f6-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="753f6-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="753f6-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="753f6-110">Attributes and elements</span></span>

<span data-ttu-id="753f6-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="753f6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="753f6-112">属性</span><span class="sxs-lookup"><span data-stu-id="753f6-112">Attributes</span></span>

<span data-ttu-id="753f6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="753f6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="753f6-114">子要素</span><span class="sxs-lookup"><span data-stu-id="753f6-114">Child elements</span></span>

<span data-ttu-id="753f6-115">なし。</span><span class="sxs-lookup"><span data-stu-id="753f6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="753f6-116">親要素</span><span class="sxs-lookup"><span data-stu-id="753f6-116">Parent elements</span></span>

|<span data-ttu-id="753f6-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="753f6-117">**Element**</span></span>|<span data-ttu-id="753f6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="753f6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="753f6-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="753f6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="753f6-120">クライアントを Exchange サーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="753f6-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="753f6-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="753f6-121">Text value</span></span>

<span data-ttu-id="753f6-122">テキスト値は、他のメールボックスの**Groupinginformation**要素の値と比較されます。</span><span class="sxs-lookup"><span data-stu-id="753f6-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="753f6-123">同じ値を持つメールボックスは、同じ Exchange Web サービス (EWS) エンドポイントを使用して、アフィニティを維持するためにまとめてグループ化することができます。</span><span class="sxs-lookup"><span data-stu-id="753f6-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="753f6-124">詳細については、「 [Exchange のサブスクリプショングループとメールボックスサーバー間のアフィニティを維持する](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="753f6-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="753f6-125">注釈</span><span class="sxs-lookup"><span data-stu-id="753f6-125">Remarks</span></span>

<span data-ttu-id="753f6-126">**Groupinginformation**要素は、値が "EXPR" である[Type (POX)](type-pox.md)子要素を持つ**プロトコル**要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="753f6-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="753f6-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="753f6-127">See also</span></span>

- [<span data-ttu-id="753f6-128">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="753f6-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="753f6-129">サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する</span><span class="sxs-lookup"><span data-stu-id="753f6-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

