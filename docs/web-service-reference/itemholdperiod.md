---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: ItemHoldPeriod 要素は、メールボックスのクエリに一致するコンテンツを保持する時間数を指定します。
ms.openlocfilehash: 212d765aa3f0493dd4f3051de483fa08a6fa8ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832144"
---
# <a name="itemholdperiod"></a><span data-ttu-id="715bc-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="715bc-103">ItemHoldPeriod</span></span>

<span data-ttu-id="715bc-104">**ItemHoldPeriod**要素は、メールボックスのクエリに一致するコンテンツを保持する時間数を指定します。</span><span class="sxs-lookup"><span data-stu-id="715bc-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="715bc-105">**string**</span><span class="sxs-lookup"><span data-stu-id="715bc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="715bc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="715bc-106">Attributes and elements</span></span>

<span data-ttu-id="715bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="715bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="715bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="715bc-108">Attributes</span></span>

<span data-ttu-id="715bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="715bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="715bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="715bc-110">Child elements</span></span>

<span data-ttu-id="715bc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="715bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="715bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="715bc-112">Parent elements</span></span>

[<span data-ttu-id="715bc-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="715bc-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="715bc-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="715bc-114">Text value</span></span>

<span data-ttu-id="715bc-115">テキスト値には「無制限」または任意の[Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx)値の文字列値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="715bc-115">The text value can be "Unlimited" or the string value of any [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="715bc-116">備考</span><span class="sxs-lookup"><span data-stu-id="715bc-116">Remarks</span></span>

<span data-ttu-id="715bc-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="715bc-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="715bc-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="715bc-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="715bc-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="715bc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="715bc-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="715bc-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="715bc-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="715bc-121">Schema Name</span></span>  <br/> |<span data-ttu-id="715bc-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="715bc-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="715bc-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="715bc-123">Validation File</span></span>  <br/> |<span data-ttu-id="715bc-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="715bc-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="715bc-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="715bc-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="715bc-126">True</span><span class="sxs-lookup"><span data-stu-id="715bc-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="715bc-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="715bc-127">See also</span></span>



[<span data-ttu-id="715bc-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="715bc-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="715bc-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="715bc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

