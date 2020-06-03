---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: ItemHoldPeriod 要素は、メールボックスクエリに一致するコンテンツを保持する時間の長さを指定します。
ms.openlocfilehash: 185666b72cc96dd88605b7baa6433d070e7ebc91
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452287"
---
# <a name="itemholdperiod"></a><span data-ttu-id="48a55-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="48a55-103">ItemHoldPeriod</span></span>

<span data-ttu-id="48a55-104">**ItemHoldPeriod**要素は、メールボックスクエリに一致するコンテンツを保持する時間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="48a55-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="48a55-105">**string**</span><span class="sxs-lookup"><span data-stu-id="48a55-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48a55-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="48a55-106">Attributes and elements</span></span>

<span data-ttu-id="48a55-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="48a55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48a55-108">属性</span><span class="sxs-lookup"><span data-stu-id="48a55-108">Attributes</span></span>

<span data-ttu-id="48a55-109">なし。</span><span class="sxs-lookup"><span data-stu-id="48a55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48a55-110">子要素</span><span class="sxs-lookup"><span data-stu-id="48a55-110">Child elements</span></span>

<span data-ttu-id="48a55-111">なし。</span><span class="sxs-lookup"><span data-stu-id="48a55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48a55-112">親要素</span><span class="sxs-lookup"><span data-stu-id="48a55-112">Parent elements</span></span>

[<span data-ttu-id="48a55-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="48a55-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="48a55-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="48a55-114">Text value</span></span>

<span data-ttu-id="48a55-115">テキスト値には、"無制限" または任意の[Timespan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx)値の文字列値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="48a55-115">The text value can be "Unlimited" or the string value of any [Timespan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="48a55-116">注釈</span><span class="sxs-lookup"><span data-stu-id="48a55-116">Remarks</span></span>

<span data-ttu-id="48a55-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="48a55-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="48a55-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="48a55-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48a55-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="48a55-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48a55-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="48a55-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48a55-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="48a55-121">Schema Name</span></span>  <br/> |<span data-ttu-id="48a55-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="48a55-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="48a55-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="48a55-123">Validation File</span></span>  <br/> |<span data-ttu-id="48a55-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="48a55-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48a55-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="48a55-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="48a55-126">正しい</span><span class="sxs-lookup"><span data-stu-id="48a55-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48a55-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="48a55-127">See also</span></span>



[<span data-ttu-id="48a55-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="48a55-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="48a55-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="48a55-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

