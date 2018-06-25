---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: IsAllDayEvent 要素は、予定表アイテムまたは会議出席依頼が終日のイベントを表すかどうかを示します。
ms.openlocfilehash: 81cf1e7d8338275540f264de7cbf194005e7770c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831983"
---
# <a name="isalldayevent"></a><span data-ttu-id="7c987-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="7c987-103">IsAllDayEvent</span></span>

<span data-ttu-id="7c987-104">**IsAllDayEvent**要素は、予定表アイテムまたは会議出席依頼が終日のイベントを表すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c987-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="7c987-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="7c987-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c987-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c987-106">Attributes and elements</span></span>

<span data-ttu-id="7c987-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c987-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c987-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c987-108">Attributes</span></span>

<span data-ttu-id="7c987-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c987-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c987-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c987-110">Child elements</span></span>

<span data-ttu-id="7c987-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7c987-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c987-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7c987-112">Parent elements</span></span>

|<span data-ttu-id="7c987-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c987-113">**Element**</span></span>|<span data-ttu-id="7c987-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c987-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c987-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="7c987-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7c987-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7c987-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c987-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7c987-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7c987-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7c987-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c987-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7c987-119">Text value</span></span>

<span data-ttu-id="7c987-120">ブール値を表す文字列値は、この要素が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="7c987-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="7c987-121">**True**の場合は、項目が終日のイベントであることを示します。</span><span class="sxs-lookup"><span data-stu-id="7c987-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="7c987-122">**False**の値は、アイテムがユーザーの作業時間よりも小さい範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="7c987-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7c987-123">備考</span><span class="sxs-lookup"><span data-stu-id="7c987-123">Remarks</span></span>

<span data-ttu-id="7c987-124">終日のイベントは、期間の作業時間の定義されているメールボックスにまたがっています。</span><span class="sxs-lookup"><span data-stu-id="7c987-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="7c987-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7c987-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c987-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c987-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c987-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c987-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c987-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c987-128">Schema name</span></span>  <br/> |<span data-ttu-id="7c987-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7c987-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c987-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c987-130">Validation file</span></span>  <br/> |<span data-ttu-id="7c987-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c987-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c987-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7c987-132">Can be empty</span></span>  <br/> |<span data-ttu-id="7c987-133">False</span><span class="sxs-lookup"><span data-stu-id="7c987-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c987-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c987-134">See also</span></span>



- [<span data-ttu-id="7c987-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c987-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

