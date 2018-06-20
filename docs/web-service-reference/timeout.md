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
description: タイムアウト要素は、サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。
ms.openlocfilehash: 0a26002689e131959f09318b01d97ffb73b605f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839698"
---
# <a name="timeout"></a><span data-ttu-id="8916d-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="8916d-103">Timeout</span></span>

<span data-ttu-id="8916d-104">**タイムアウト**要素は、サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。</span><span class="sxs-lookup"><span data-stu-id="8916d-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="8916d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="8916d-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8916d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8916d-106">Attributes and elements</span></span>

<span data-ttu-id="8916d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8916d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8916d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8916d-108">Attributes</span></span>

<span data-ttu-id="8916d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8916d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8916d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8916d-110">Child elements</span></span>

<span data-ttu-id="8916d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8916d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8916d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8916d-112">Parent elements</span></span>

|<span data-ttu-id="8916d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8916d-113">**Element**</span></span>|<span data-ttu-id="8916d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8916d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8916d-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8916d-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="8916d-116">プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="8916d-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8916d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8916d-117">Text value</span></span>

<span data-ttu-id="8916d-118">整数値を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="8916d-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="8916d-119">この要素の値は、1 から 1440 の範囲です。</span><span class="sxs-lookup"><span data-stu-id="8916d-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="8916d-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="8916d-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8916d-121">備考</span><span class="sxs-lookup"><span data-stu-id="8916d-121">Remarks</span></span>

<span data-ttu-id="8916d-122">GetEvents 要求が成功して、サブスクリプションのタイムアウト タイマーがリセットされます。</span><span class="sxs-lookup"><span data-stu-id="8916d-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="8916d-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8916d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8916d-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="8916d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8916d-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="8916d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8916d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8916d-126">Schema name</span></span>  <br/> |<span data-ttu-id="8916d-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8916d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8916d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8916d-128">Validation file</span></span>  <br/> |<span data-ttu-id="8916d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8916d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8916d-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8916d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="8916d-131">False</span><span class="sxs-lookup"><span data-stu-id="8916d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8916d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="8916d-132">See also</span></span>



[<span data-ttu-id="8916d-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="8916d-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="8916d-134">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="8916d-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="8916d-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="8916d-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

