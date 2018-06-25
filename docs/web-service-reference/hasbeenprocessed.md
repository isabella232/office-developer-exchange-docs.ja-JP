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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831796"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="79a98-103">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="79a98-103">HasBeenProcessed</span></span>

<span data-ttu-id="79a98-104">**HasBeenProcessed**要素は、あるかどうか、会議出席依頼アイテムが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="79a98-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="79a98-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="79a98-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79a98-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="79a98-106">Attributes and elements</span></span>

<span data-ttu-id="79a98-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79a98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79a98-108">属性</span><span class="sxs-lookup"><span data-stu-id="79a98-108">Attributes</span></span>

<span data-ttu-id="79a98-109">なし。</span><span class="sxs-lookup"><span data-stu-id="79a98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79a98-110">子要素</span><span class="sxs-lookup"><span data-stu-id="79a98-110">Child elements</span></span>

<span data-ttu-id="79a98-111">なし。</span><span class="sxs-lookup"><span data-stu-id="79a98-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79a98-112">親要素</span><span class="sxs-lookup"><span data-stu-id="79a98-112">Parent elements</span></span>

|<span data-ttu-id="79a98-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="79a98-113">**Element**</span></span>|<span data-ttu-id="79a98-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="79a98-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79a98-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="79a98-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="79a98-116">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="79a98-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79a98-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="79a98-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="79a98-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="79a98-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79a98-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="79a98-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="79a98-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="79a98-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79a98-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="79a98-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="79a98-122">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="79a98-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79a98-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="79a98-123">Text value</span></span>

<span data-ttu-id="79a98-124">**True**の場合、テキスト値は、会議出席依頼が処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="79a98-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="79a98-125">備考</span><span class="sxs-lookup"><span data-stu-id="79a98-125">Remarks</span></span>

<span data-ttu-id="79a98-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="79a98-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79a98-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="79a98-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79a98-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="79a98-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79a98-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79a98-129">Schema Name</span></span>  <br/> |<span data-ttu-id="79a98-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="79a98-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="79a98-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79a98-131">Validation File</span></span>  <br/> |<span data-ttu-id="79a98-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79a98-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79a98-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="79a98-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="79a98-134">False</span><span class="sxs-lookup"><span data-stu-id="79a98-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79a98-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="79a98-135">See also</span></span>



- [<span data-ttu-id="79a98-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="79a98-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

