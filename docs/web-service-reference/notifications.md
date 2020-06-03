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
description: 通知要素には、サブスクリプションに関する情報の配列と、最後の通知以降に発生したイベントが含まれます。
ms.openlocfilehash: 88fc56ba6e672e3dea7a1d31f7cc1fda018b9a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462620"
---
# <a name="notifications"></a><span data-ttu-id="6a360-103">通知</span><span class="sxs-lookup"><span data-stu-id="6a360-103">Notifications</span></span>

<span data-ttu-id="6a360-104">**通知**要素には、サブスクリプションに関する情報の配列と、最後の通知以降に発生したイベントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6a360-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="6a360-105">**非 Emptyarrayofnotificationstype**</span><span class="sxs-lookup"><span data-stu-id="6a360-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a360-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a360-106">Attributes and elements</span></span>

<span data-ttu-id="6a360-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a360-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a360-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a360-108">Attributes</span></span>

<span data-ttu-id="6a360-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a360-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a360-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a360-110">Child elements</span></span>

|<span data-ttu-id="6a360-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6a360-111">**Element**</span></span>|<span data-ttu-id="6a360-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a360-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a360-113">通知</span><span class="sxs-lookup"><span data-stu-id="6a360-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6a360-114">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6a360-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a360-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6a360-115">Parent elements</span></span>

|<span data-ttu-id="6a360-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a360-116">**Element**</span></span>|<span data-ttu-id="6a360-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a360-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a360-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6a360-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="6a360-119">1つの[Getstreamingevents 操作](getstreamingevents-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="6a360-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a360-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a360-120">Text value</span></span>

<span data-ttu-id="6a360-121">なし。</span><span class="sxs-lookup"><span data-stu-id="6a360-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a360-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6a360-122">Remarks</span></span>

<span data-ttu-id="6a360-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a360-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a360-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a360-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a360-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a360-125">Namespace</span></span>  <br/> |<span data-ttu-id="6a360-126">https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="6a360-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="6a360-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a360-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6a360-128">メッセージスキーマ。Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a360-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="6a360-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a360-129">Validation File</span></span>  <br/> |<span data-ttu-id="6a360-130">メッセージ .xsd。型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6a360-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a360-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a360-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a360-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="6a360-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a360-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a360-133">See also</span></span>



[<span data-ttu-id="6a360-134">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6a360-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="6a360-135">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6a360-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="6a360-136">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6a360-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="6a360-137">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6a360-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="6a360-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6a360-138">Subscribe operation</span></span>](subscribe-operation.md)

