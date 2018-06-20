---
title: 通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: 通知の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報の配列が含まれています。
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832550"
---
# <a name="notifications"></a><span data-ttu-id="46a2f-103">通知</span><span class="sxs-lookup"><span data-stu-id="46a2f-103">Notifications</span></span>

<span data-ttu-id="46a2f-104">**通知**の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="46a2f-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="46a2f-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="46a2f-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46a2f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="46a2f-106">Attributes and elements</span></span>

<span data-ttu-id="46a2f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46a2f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46a2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="46a2f-108">Attributes</span></span>

<span data-ttu-id="46a2f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="46a2f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46a2f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="46a2f-110">Child elements</span></span>

|<span data-ttu-id="46a2f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="46a2f-111">**Element**</span></span>|<span data-ttu-id="46a2f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="46a2f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46a2f-113">通知</span><span class="sxs-lookup"><span data-stu-id="46a2f-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="46a2f-114">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="46a2f-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46a2f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="46a2f-115">Parent elements</span></span>

|<span data-ttu-id="46a2f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="46a2f-116">**Element**</span></span>|<span data-ttu-id="46a2f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="46a2f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46a2f-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="46a2f-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="46a2f-119">状態および 1 つの結果が含まれています[GetStreamingEvents の操作](getstreamingevents-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="46a2f-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46a2f-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="46a2f-120">Text value</span></span>

<span data-ttu-id="46a2f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="46a2f-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46a2f-122">備考</span><span class="sxs-lookup"><span data-stu-id="46a2f-122">Remarks</span></span>

<span data-ttu-id="46a2f-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="46a2f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46a2f-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="46a2f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46a2f-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="46a2f-125">Namespace</span></span>  <br/> |<span data-ttu-id="46a2f-126">http://schemas.microsoft.com/exchange/services/2006/messages と http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="46a2f-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="46a2f-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46a2f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="46a2f-128">メッセージ スキーマです。タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="46a2f-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="46a2f-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46a2f-129">Validation File</span></span>  <br/> |<span data-ttu-id="46a2f-130">Messages.xsd です。Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46a2f-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46a2f-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46a2f-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="46a2f-132">False</span><span class="sxs-lookup"><span data-stu-id="46a2f-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46a2f-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="46a2f-133">See also</span></span>



<span data-ttu-id="46a2f-134">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="46a2f-134">[GetFolder operation](getfolder-operation.md)</span></span>
  
[<span data-ttu-id="46a2f-135">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46a2f-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="46a2f-136">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46a2f-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="46a2f-137">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46a2f-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="46a2f-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="46a2f-138">Subscribe operation</span></span>](subscribe-operation.md)

