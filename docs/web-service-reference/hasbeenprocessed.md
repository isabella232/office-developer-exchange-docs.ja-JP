---
title: Hasが処理されました
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
description: Hasが処理された要素は、会議メッセージアイテムが処理されたかどうかを示します。
ms.openlocfilehash: 7251ca86e07a0b72c186c65094b6469331dfd12e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462894"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="90a94-103">Hasが処理されました</span><span class="sxs-lookup"><span data-stu-id="90a94-103">HasBeenProcessed</span></span>

<span data-ttu-id="90a94-104">**Hasが処理**された要素は、会議メッセージアイテムが処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90a94-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="90a94-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="90a94-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90a94-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="90a94-106">Attributes and elements</span></span>

<span data-ttu-id="90a94-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90a94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90a94-108">属性</span><span class="sxs-lookup"><span data-stu-id="90a94-108">Attributes</span></span>

<span data-ttu-id="90a94-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90a94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90a94-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90a94-110">Child elements</span></span>

<span data-ttu-id="90a94-111">なし。</span><span class="sxs-lookup"><span data-stu-id="90a94-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90a94-112">親要素</span><span class="sxs-lookup"><span data-stu-id="90a94-112">Parent elements</span></span>

|<span data-ttu-id="90a94-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="90a94-113">**Element**</span></span>|<span data-ttu-id="90a94-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="90a94-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90a94-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="90a94-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="90a94-116">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="90a94-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="90a94-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="90a94-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="90a94-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="90a94-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="90a94-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="90a94-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="90a94-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="90a94-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="90a94-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="90a94-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="90a94-122">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="90a94-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90a94-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="90a94-123">Text value</span></span>

<span data-ttu-id="90a94-124">テキスト値が**true の場合**は、会議メッセージが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="90a94-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="90a94-125">注釈</span><span class="sxs-lookup"><span data-stu-id="90a94-125">Remarks</span></span>

<span data-ttu-id="90a94-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="90a94-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90a94-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="90a94-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90a94-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="90a94-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90a94-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90a94-129">Schema Name</span></span>  <br/> |<span data-ttu-id="90a94-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="90a94-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="90a94-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90a94-131">Validation File</span></span>  <br/> |<span data-ttu-id="90a94-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="90a94-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90a94-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="90a94-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="90a94-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="90a94-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90a94-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="90a94-135">See also</span></span>



- [<span data-ttu-id="90a94-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="90a94-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

