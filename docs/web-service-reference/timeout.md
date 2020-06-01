---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: Timeout 要素は、クライアントからの GetEvents 要求なしに、サブスクリプションがアイドル状態のままになることができる期間 (分単位) を表します。
ms.openlocfilehash: 6f3228cd480bf0eaf259c4f321bc74d0845b9bba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459897"
---
# <a name="timeout"></a><span data-ttu-id="57f5f-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="57f5f-103">Timeout</span></span>

<span data-ttu-id="57f5f-104">**Timeout**要素は、クライアントからの GetEvents 要求なしに、サブスクリプションがアイドル状態のままになることができる期間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="57f5f-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="57f5f-105">**int**</span><span class="sxs-lookup"><span data-stu-id="57f5f-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57f5f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="57f5f-106">Attributes and elements</span></span>

<span data-ttu-id="57f5f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57f5f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57f5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="57f5f-108">Attributes</span></span>

<span data-ttu-id="57f5f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57f5f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57f5f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57f5f-110">Child elements</span></span>

<span data-ttu-id="57f5f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57f5f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57f5f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57f5f-112">Parent elements</span></span>

|<span data-ttu-id="57f5f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="57f5f-113">**Element**</span></span>|<span data-ttu-id="57f5f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="57f5f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57f5f-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="57f5f-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="57f5f-116">プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="57f5f-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57f5f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57f5f-117">Text value</span></span>

<span data-ttu-id="57f5f-118">この要素を使用する場合は、整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="57f5f-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="57f5f-119">この要素で使用できる値は、1 ~ 1440 の範囲です。</span><span class="sxs-lookup"><span data-stu-id="57f5f-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="57f5f-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="57f5f-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57f5f-121">注釈</span><span class="sxs-lookup"><span data-stu-id="57f5f-121">Remarks</span></span>

<span data-ttu-id="57f5f-122">サブスクリプションのタイムアウトタイマーは、GetEvents 要求が正常にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="57f5f-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="57f5f-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="57f5f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="57f5f-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="57f5f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57f5f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="57f5f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57f5f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57f5f-126">Schema name</span></span>  <br/> |<span data-ttu-id="57f5f-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="57f5f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="57f5f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57f5f-128">Validation file</span></span>  <br/> |<span data-ttu-id="57f5f-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="57f5f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57f5f-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="57f5f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="57f5f-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="57f5f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57f5f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="57f5f-132">See also</span></span>



[<span data-ttu-id="57f5f-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="57f5f-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="57f5f-134">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="57f5f-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="57f5f-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="57f5f-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

