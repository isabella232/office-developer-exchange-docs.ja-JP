---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: IsMeeting 要素は、予定表アイテムが会議や予定があるかどうかを示します。
ms.openlocfilehash: bb1349a8690450882e6beac0ccd84a8d03272a7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832051"
---
# <a name="ismeeting"></a><span data-ttu-id="97b47-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="97b47-103">IsMeeting</span></span>

<span data-ttu-id="97b47-104">**IsMeeting**要素は、予定表アイテムが会議や予定があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="97b47-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="97b47-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="97b47-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97b47-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="97b47-106">Attributes and elements</span></span>

<span data-ttu-id="97b47-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97b47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97b47-108">属性</span><span class="sxs-lookup"><span data-stu-id="97b47-108">Attributes</span></span>

<span data-ttu-id="97b47-109">なし。</span><span class="sxs-lookup"><span data-stu-id="97b47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97b47-110">子要素</span><span class="sxs-lookup"><span data-stu-id="97b47-110">Child elements</span></span>

<span data-ttu-id="97b47-111">なし。</span><span class="sxs-lookup"><span data-stu-id="97b47-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97b47-112">親要素</span><span class="sxs-lookup"><span data-stu-id="97b47-112">Parent elements</span></span>

|<span data-ttu-id="97b47-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="97b47-113">**Element**</span></span>|<span data-ttu-id="97b47-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="97b47-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97b47-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="97b47-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="97b47-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="97b47-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="97b47-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="97b47-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="97b47-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="97b47-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97b47-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="97b47-119">Text value</span></span>

<span data-ttu-id="97b47-120">ブール値を表す文字列値は、この要素が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="97b47-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="97b47-121">**True**の場合は、予定表アイテムが会議であることを示します。</span><span class="sxs-lookup"><span data-stu-id="97b47-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="97b47-122">値が**false**の場合、予定表アイテムが予定であることを示します。</span><span class="sxs-lookup"><span data-stu-id="97b47-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="97b47-123">備考</span><span class="sxs-lookup"><span data-stu-id="97b47-123">Remarks</span></span>

<span data-ttu-id="97b47-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="97b47-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97b47-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="97b47-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97b47-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="97b47-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97b47-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="97b47-127">Schema name</span></span>  <br/> |<span data-ttu-id="97b47-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="97b47-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="97b47-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="97b47-129">Validation file</span></span>  <br/> |<span data-ttu-id="97b47-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97b47-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97b47-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97b47-131">Can be empty</span></span>  <br/> |<span data-ttu-id="97b47-132">False</span><span class="sxs-lookup"><span data-stu-id="97b47-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97b47-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="97b47-133">See also</span></span>



- [<span data-ttu-id="97b47-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="97b47-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

