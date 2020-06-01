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
description: ReturnQueueEvents 要素は、タスクを実行しているユーザーが特権の役割を持っていることを示します。
ms.openlocfilehash: 9d07bc8c3d32f1cd532febaf4ae04e4a2d31d243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466592"
---
# <a name="returnqueueevents"></a><span data-ttu-id="afe2c-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="afe2c-103">ReturnQueueEvents</span></span>

<span data-ttu-id="afe2c-104">**Returnqueueevents**要素は、タスクを実行しているユーザーが特権の役割を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="afe2c-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="afe2c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="afe2c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afe2c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="afe2c-106">Attributes and elements</span></span>

<span data-ttu-id="afe2c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afe2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afe2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="afe2c-108">Attributes</span></span>

<span data-ttu-id="afe2c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afe2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afe2c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afe2c-110">Child elements</span></span>

<span data-ttu-id="afe2c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="afe2c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afe2c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="afe2c-112">Parent elements</span></span>

|<span data-ttu-id="afe2c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="afe2c-113">**Element**</span></span>|<span data-ttu-id="afe2c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="afe2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afe2c-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="afe2c-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="afe2c-116">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="afe2c-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afe2c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="afe2c-117">Text value</span></span>

<span data-ttu-id="afe2c-118">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="afe2c-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="afe2c-119">値が**true の場合**は、タスクを実行しているユーザーが特権ロールに含まれていることを示します。値が**false**の場合は、タスクを実行しているユーザーが特権ロールに含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="afe2c-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="afe2c-120">注釈</span><span class="sxs-lookup"><span data-stu-id="afe2c-120">Remarks</span></span>

<span data-ttu-id="afe2c-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="afe2c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afe2c-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="afe2c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afe2c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="afe2c-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="afe2c-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afe2c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="afe2c-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="afe2c-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="afe2c-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afe2c-126">Validation File</span></span>  <br/> |<span data-ttu-id="afe2c-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="afe2c-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="afe2c-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afe2c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="afe2c-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="afe2c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afe2c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="afe2c-130">See also</span></span>



[<span data-ttu-id="afe2c-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="afe2c-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="afe2c-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="afe2c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

