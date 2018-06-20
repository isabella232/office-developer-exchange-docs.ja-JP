---
title: HasBeenProcessed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasBeenProcessed
api_type:
- schema
ms.assetid: 46d4af8e-0f11-4a74-9365-1d983731fed8
description: HasBeenProcessed 要素は、あるかどうか、会議出席依頼アイテムが処理されたことを示します。
ms.openlocfilehash: cccd3b2258490fcbe902bcd391f25b0be2fe7c26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831796"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="5c070-103">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="5c070-103">HasBeenProcessed</span></span>

<span data-ttu-id="5c070-104">**HasBeenProcessed**要素は、あるかどうか、会議出席依頼アイテムが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="5c070-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="5c070-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="5c070-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c070-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c070-106">Attributes and elements</span></span>

<span data-ttu-id="5c070-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c070-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c070-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c070-108">Attributes</span></span>

<span data-ttu-id="5c070-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c070-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c070-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c070-110">Child elements</span></span>

<span data-ttu-id="5c070-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5c070-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c070-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5c070-112">Parent elements</span></span>

|<span data-ttu-id="5c070-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c070-113">**Element**</span></span>|<span data-ttu-id="5c070-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c070-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c070-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5c070-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5c070-116">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="5c070-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c070-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5c070-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5c070-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="5c070-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c070-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5c070-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5c070-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5c070-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c070-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5c070-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5c070-122">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5c070-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c070-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5c070-123">Text value</span></span>

<span data-ttu-id="5c070-124">**True**の場合、テキスト値は、会議出席依頼が処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="5c070-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5c070-125">備考</span><span class="sxs-lookup"><span data-stu-id="5c070-125">Remarks</span></span>

<span data-ttu-id="5c070-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5c070-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c070-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c070-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c070-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c070-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c070-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c070-129">Schema Name</span></span>  <br/> |<span data-ttu-id="5c070-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c070-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c070-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c070-131">Validation File</span></span>  <br/> |<span data-ttu-id="5c070-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c070-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c070-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c070-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c070-134">False</span><span class="sxs-lookup"><span data-stu-id="5c070-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c070-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c070-135">See also</span></span>



- [<span data-ttu-id="5c070-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c070-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

