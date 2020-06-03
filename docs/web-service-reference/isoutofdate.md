---
title: IsOutOfDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOutOfDate
api_type:
- schema
ms.assetid: 2b6005a6-56a9-4848-b998-32908c13e2e2
description: IsOutOfDate 要素は、会議メッセージ、要求、応答、または取り消しが期限切れであるかどうかを示します。
ms.openlocfilehash: b50b021e48789ba63016582450404b5da3ff86e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466550"
---
# <a name="isoutofdate"></a><span data-ttu-id="74f82-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="74f82-103">IsOutOfDate</span></span>

<span data-ttu-id="74f82-104">**IsOutOfDate**要素は、会議メッセージ、要求、応答、または取り消しが期限切れであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74f82-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="74f82-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="74f82-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74f82-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74f82-106">Attributes and elements</span></span>

<span data-ttu-id="74f82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74f82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74f82-108">属性</span><span class="sxs-lookup"><span data-stu-id="74f82-108">Attributes</span></span>

<span data-ttu-id="74f82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74f82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74f82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74f82-110">Child elements</span></span>

<span data-ttu-id="74f82-111">なし。</span><span class="sxs-lookup"><span data-stu-id="74f82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74f82-112">親要素</span><span class="sxs-lookup"><span data-stu-id="74f82-112">Parent elements</span></span>

|<span data-ttu-id="74f82-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="74f82-113">**Element**</span></span>|<span data-ttu-id="74f82-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="74f82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74f82-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="74f82-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="74f82-116">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="74f82-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="74f82-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="74f82-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="74f82-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="74f82-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="74f82-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="74f82-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="74f82-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="74f82-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="74f82-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="74f82-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="74f82-122">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="74f82-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74f82-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="74f82-123">Text value</span></span>

<span data-ttu-id="74f82-124">テキスト値が**true の場合**は、会議アイテムが古くなっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="74f82-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="74f82-125">注釈</span><span class="sxs-lookup"><span data-stu-id="74f82-125">Remarks</span></span>

<span data-ttu-id="74f82-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="74f82-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74f82-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74f82-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74f82-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="74f82-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74f82-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74f82-129">Schema Name</span></span>  <br/> |<span data-ttu-id="74f82-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="74f82-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="74f82-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74f82-131">Validation File</span></span>  <br/> |<span data-ttu-id="74f82-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="74f82-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74f82-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74f82-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="74f82-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="74f82-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74f82-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="74f82-135">See also</span></span>



- [<span data-ttu-id="74f82-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="74f82-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

