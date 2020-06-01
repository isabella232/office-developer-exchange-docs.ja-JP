---
title: その他のイベント
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
description: More Events 要素は、キュー内にクライアントに配信されるイベントが他にもあるかどうかを示します。
ms.openlocfilehash: fd12dd2e2e64ce1711e553ba5eb29bd0eb64c892
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462732"
---
# <a name="moreevents"></a><span data-ttu-id="d4691-103">その他のイベント</span><span class="sxs-lookup"><span data-stu-id="d4691-103">MoreEvents</span></span>

<span data-ttu-id="d4691-104">More **events**要素は、キュー内にクライアントに配信されるイベントが他にもあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d4691-104">The **MoreEvents** element indicates whether there are more events in the queue to be delivered to the client.</span></span> 
  
```xml
<MoreEvents/>
```

 <span data-ttu-id="d4691-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d4691-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4691-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d4691-106">Attributes and elements</span></span>

<span data-ttu-id="d4691-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4691-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4691-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4691-108">Attributes</span></span>

<span data-ttu-id="d4691-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4691-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4691-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4691-110">Child elements</span></span>

<span data-ttu-id="d4691-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d4691-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4691-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d4691-112">Parent elements</span></span>

|<span data-ttu-id="d4691-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4691-113">**Element**</span></span>|<span data-ttu-id="d4691-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4691-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4691-115">通知</span><span class="sxs-lookup"><span data-stu-id="d4691-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d4691-116">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d4691-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4691-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d4691-117">Text value</span></span>

<span data-ttu-id="d4691-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="d4691-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="d4691-119">値が**true の場合**は、キューに追加されたイベントがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="d4691-119">A value of **true** indicates that more events are in the queue.</span></span> <span data-ttu-id="d4691-120">値が**false**の場合は、キューにこれ以上イベントがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d4691-120">A value of **false** indicates that no more events are in the queue.</span></span> <span data-ttu-id="d4691-121">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d4691-121">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d4691-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d4691-122">Remarks</span></span>

<span data-ttu-id="d4691-123">プル通知の場合、この要素の**true**値は、残りのイベントを取得するために別の GetEvents 要求を発行する必要があることをクライアントに示します。</span><span class="sxs-lookup"><span data-stu-id="d4691-123">In the case of Pull notifications, a **true** value in this element indicates to the client that another GetEvents request should be issued to get the remaining events.</span></span> <span data-ttu-id="d4691-124">クライアント仕様でイベント通知の最小待機時間が要求されていると仮定すると、GetEvents 要求**は、それ**よりも長い**イベント**値が返されるまで連続した連続で続行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4691-124">Assuming that the client specifications require minimum latency for event notifications, GetEvents requests should continue in a continuous succession until a **false** **MoreEvents** value is returned.</span></span> 
  
<span data-ttu-id="d4691-125">プッシュ通知の場合、[その他のイベントの**true**値] は、他の通知要求がクライアントに送信され、残りのイベントが配信されること**を示します**。</span><span class="sxs-lookup"><span data-stu-id="d4691-125">In the case of Push notifications, a **true** value for **MoreEvents** indicates to the client that another notification request will be sent to the client to deliver the remaining events.</span></span> <span data-ttu-id="d4691-126">プル通知と同様に、これらのフォローアップ要求は、クライアントアクセスサーバーのイベントキューが空になるまで連続して継続して続行されます。</span><span class="sxs-lookup"><span data-stu-id="d4691-126">Similar to Pull notifications, these follow-up requests will continue in continuous succession until the event queue on the Client Access server is empty.</span></span> 
  
<span data-ttu-id="d4691-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d4691-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4691-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d4691-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4691-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4691-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4691-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4691-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d4691-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d4691-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4691-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4691-132">Validation File</span></span>  <br/> |<span data-ttu-id="d4691-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d4691-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4691-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d4691-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4691-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="d4691-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4691-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4691-136">See also</span></span>



[<span data-ttu-id="d4691-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d4691-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d4691-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d4691-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d4691-139">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d4691-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

