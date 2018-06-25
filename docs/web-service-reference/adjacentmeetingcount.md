---
title: AdjacentMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetingCount
api_type:
- schema
ms.assetid: 35045024-f6e1-47d1-89be-f100b7b4f3c7
description: AdjacentMeetingCount 要素は、会議の時刻に隣接している予定表アイテムの合計数を表します。
ms.openlocfilehash: a00468bec392498745fe778b627259a79d6027bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759300"
---
# <a name="adjacentmeetingcount"></a><span data-ttu-id="94ec8-103">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="94ec8-103">AdjacentMeetingCount</span></span>

<span data-ttu-id="94ec8-104">**AdjacentMeetingCount**要素は、会議の時刻に隣接している予定表アイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="94ec8-104">The **AdjacentMeetingCount** element represents the total number of calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetingCount/>
```

 <span data-ttu-id="94ec8-105">**Int**</span><span class="sxs-lookup"><span data-stu-id="94ec8-105">**Int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94ec8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="94ec8-106">Attributes and elements</span></span>

<span data-ttu-id="94ec8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94ec8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94ec8-108">属性</span><span class="sxs-lookup"><span data-stu-id="94ec8-108">Attributes</span></span>

<span data-ttu-id="94ec8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="94ec8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94ec8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="94ec8-110">Child elements</span></span>

<span data-ttu-id="94ec8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="94ec8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94ec8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="94ec8-112">Parent elements</span></span>

|<span data-ttu-id="94ec8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="94ec8-113">**Element**</span></span>|<span data-ttu-id="94ec8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="94ec8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94ec8-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="94ec8-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="94ec8-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="94ec8-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="94ec8-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="94ec8-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="94ec8-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="94ec8-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94ec8-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="94ec8-119">Text value</span></span>

<span data-ttu-id="94ec8-120">整数値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="94ec8-120">A text value that represents an integer is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94ec8-121">備考</span><span class="sxs-lookup"><span data-stu-id="94ec8-121">Remarks</span></span>

<span data-ttu-id="94ec8-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="94ec8-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94ec8-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="94ec8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94ec8-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="94ec8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94ec8-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94ec8-125">Schema name</span></span>  <br/> |<span data-ttu-id="94ec8-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="94ec8-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="94ec8-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94ec8-127">Validation file</span></span>  <br/> |<span data-ttu-id="94ec8-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94ec8-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94ec8-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="94ec8-129">Can be empty</span></span>  <br/> |<span data-ttu-id="94ec8-130">False</span><span class="sxs-lookup"><span data-stu-id="94ec8-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94ec8-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="94ec8-131">See also</span></span>

- [<span data-ttu-id="94ec8-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="94ec8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

