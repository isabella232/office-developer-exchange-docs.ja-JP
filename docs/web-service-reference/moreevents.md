---
title: イベント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: イベント要素は、クライアントに配信するキューにその他のイベントがあるかどうかを示します。
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832489"
---
# <a name="moreevents"></a><span data-ttu-id="fd41c-103">イベント</span><span class="sxs-lookup"><span data-stu-id="fd41c-103">MoreEvents</span></span>

<span data-ttu-id="fd41c-104">**イベント**要素は、クライアントに配信するキューにその他のイベントがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fd41c-104">The **MoreEvents** element indicates whether there are more events in the queue to be delivered to the client.</span></span> 
  
```xml
<MoreEvents/>
```

 <span data-ttu-id="fd41c-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="fd41c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd41c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fd41c-106">Attributes and elements</span></span>

<span data-ttu-id="fd41c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd41c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd41c-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd41c-108">Attributes</span></span>

<span data-ttu-id="fd41c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fd41c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd41c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fd41c-110">Child elements</span></span>

<span data-ttu-id="fd41c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fd41c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd41c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fd41c-112">Parent elements</span></span>

|<span data-ttu-id="fd41c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd41c-113">**Element**</span></span>|<span data-ttu-id="fd41c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd41c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd41c-115">通知</span><span class="sxs-lookup"><span data-stu-id="fd41c-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fd41c-116">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd41c-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd41c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fd41c-117">Text value</span></span>

<span data-ttu-id="fd41c-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="fd41c-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="fd41c-119">**True**の場合より多くのイベントがキューにあることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd41c-119">A value of **true** indicates that more events are in the queue.</span></span> <span data-ttu-id="fd41c-120">**False**の値は、これ以上イベントがキューにあることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd41c-120">A value of **false** indicates that no more events are in the queue.</span></span> <span data-ttu-id="fd41c-121">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fd41c-121">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fd41c-122">備考</span><span class="sxs-lookup"><span data-stu-id="fd41c-122">Remarks</span></span>

<span data-ttu-id="fd41c-123">プルの通知の場合はこの要素の値が**true**を示しますクライアントに残りのイベントを取得する別の GetEvents 要求を発行すること。</span><span class="sxs-lookup"><span data-stu-id="fd41c-123">In the case of Pull notifications, a **true** value in this element indicates to the client that another GetEvents request should be issued to get the remaining events.</span></span> <span data-ttu-id="fd41c-124">仮定するとクライアントの仕様では、イベント通知の最小待機時間を必要とする、GetEvents 要求する必要がありますまで続行する継続的な連続、 **false** **イベント**の値が返されます。</span><span class="sxs-lookup"><span data-stu-id="fd41c-124">Assuming that the client specifications require minimum latency for event notifications, GetEvents requests should continue in a continuous succession until a **false** **MoreEvents** value is returned.</span></span> 
  
<span data-ttu-id="fd41c-125">場合は、プッシュ通知**イベント**の**真**の値を示しますクライアントに別の通知要求が残りのイベントを提供するクライアントに送信されること。</span><span class="sxs-lookup"><span data-stu-id="fd41c-125">In the case of Push notifications, a **true** value for **MoreEvents** indicates to the client that another notification request will be sent to the client to deliver the remaining events.</span></span> <span data-ttu-id="fd41c-126">プル通知と同様に、これらのフォロー アップの要求は引き続き継続的な連続してクライアント アクセス サーバー上のイベント キューが空になるまでです。</span><span class="sxs-lookup"><span data-stu-id="fd41c-126">Similar to Pull notifications, these follow-up requests will continue in continuous succession until the event queue on the Client Access server is empty.</span></span> 
  
<span data-ttu-id="fd41c-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="fd41c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd41c-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="fd41c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd41c-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="fd41c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd41c-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd41c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fd41c-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fd41c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd41c-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd41c-132">Validation File</span></span>  <br/> |<span data-ttu-id="fd41c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd41c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd41c-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd41c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd41c-135">False</span><span class="sxs-lookup"><span data-stu-id="fd41c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd41c-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd41c-136">See also</span></span>



[<span data-ttu-id="fd41c-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="fd41c-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="fd41c-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="fd41c-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="fd41c-139">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="fd41c-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

