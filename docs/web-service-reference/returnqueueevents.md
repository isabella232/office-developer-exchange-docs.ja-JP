---
title: ReturnQueueEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReturnQueueEvents
api_type:
- schema
ms.assetid: 69d22417-320c-4c6f-9fb4-2020f2480bb2
description: ReturnQueueEvents 要素は、タスクを実行している人が特権を持つ役割のことを示します。
ms.openlocfilehash: 02f4ca86ffa14117105ec186ae039065cb626670
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833233"
---
# <a name="returnqueueevents"></a><span data-ttu-id="a4140-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="a4140-103">ReturnQueueEvents</span></span>

<span data-ttu-id="a4140-104">**ReturnQueueEvents**要素は、タスクを実行している人が特権を持つ役割のことを示します。</span><span class="sxs-lookup"><span data-stu-id="a4140-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="a4140-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="a4140-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4140-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4140-106">Attributes and elements</span></span>

<span data-ttu-id="a4140-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4140-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4140-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4140-108">Attributes</span></span>

<span data-ttu-id="a4140-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4140-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4140-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4140-110">Child elements</span></span>

<span data-ttu-id="a4140-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a4140-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4140-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a4140-112">Parent elements</span></span>

|<span data-ttu-id="a4140-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4140-113">**Element**</span></span>|<span data-ttu-id="a4140-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4140-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4140-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a4140-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="a4140-116">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="a4140-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4140-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4140-117">Text value</span></span>

<span data-ttu-id="a4140-118">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4140-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="a4140-119">**True**の場合のことを示します、タスクを実行している人、特権を持つ役割です。**false**の値は、タスクを実行している人が特権を持つロールされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a4140-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4140-120">備考</span><span class="sxs-lookup"><span data-stu-id="a4140-120">Remarks</span></span>

<span data-ttu-id="a4140-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4140-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4140-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4140-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4140-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4140-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4140-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4140-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a4140-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a4140-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4140-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4140-126">Validation File</span></span>  <br/> |<span data-ttu-id="a4140-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4140-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4140-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4140-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4140-129">False</span><span class="sxs-lookup"><span data-stu-id="a4140-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4140-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4140-130">See also</span></span>



[<span data-ttu-id="a4140-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="a4140-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="a4140-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4140-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

