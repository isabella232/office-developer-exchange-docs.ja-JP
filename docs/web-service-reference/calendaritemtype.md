---
title: CalendarItemType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: CalendarItemType 要素は、予定表アイテムの種類を表します。
ms.openlocfilehash: 3fe95c86ea24e6dfeb4740ead5e787bd63b5190d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759589"
---
# <a name="calendaritemtype"></a><span data-ttu-id="5ff98-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="5ff98-103">CalendarItemType</span></span>

<span data-ttu-id="5ff98-104">**CalendarItemType**要素は、予定表アイテムの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="5ff98-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="5ff98-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="5ff98-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ff98-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5ff98-106">Attributes and elements</span></span>

<span data-ttu-id="5ff98-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ff98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ff98-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ff98-108">Attributes</span></span>

<span data-ttu-id="5ff98-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5ff98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ff98-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5ff98-110">Child elements</span></span>

<span data-ttu-id="5ff98-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5ff98-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5ff98-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5ff98-112">Parent elements</span></span>

|<span data-ttu-id="5ff98-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ff98-113">**Element**</span></span>|<span data-ttu-id="5ff98-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ff98-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ff98-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5ff98-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5ff98-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="5ff98-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ff98-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="5ff98-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5ff98-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5ff98-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ff98-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5ff98-119">Text value</span></span>

<span data-ttu-id="5ff98-120">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="5ff98-120">A text value is required if this element is used.</span></span> <span data-ttu-id="5ff98-121">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="5ff98-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="5ff98-122">**1 つ**アイテムが定期的な予定表アイテムに関連付けられているではありません。</span><span class="sxs-lookup"><span data-stu-id="5ff98-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5ff98-123">**出現**アイテムは、定期的な予定表アイテムの発生です。</span><span class="sxs-lookup"><span data-stu-id="5ff98-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5ff98-124">**例外**アイテムは、定期的な予定表アイテムの例外です。</span><span class="sxs-lookup"><span data-stu-id="5ff98-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5ff98-125">**RecurringMaster**アイテムは、一連の定期的な予定表アイテムのマスターです。</span><span class="sxs-lookup"><span data-stu-id="5ff98-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="5ff98-126">備考</span><span class="sxs-lookup"><span data-stu-id="5ff98-126">Remarks</span></span>

<span data-ttu-id="5ff98-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5ff98-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ff98-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="5ff98-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ff98-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="5ff98-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ff98-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ff98-130">Schema name</span></span>  <br/> |<span data-ttu-id="5ff98-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5ff98-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ff98-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ff98-132">Validation file</span></span>  <br/> |<span data-ttu-id="5ff98-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5ff98-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ff98-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5ff98-134">Can be empty</span></span>  <br/> |<span data-ttu-id="5ff98-135">False</span><span class="sxs-lookup"><span data-stu-id="5ff98-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ff98-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ff98-136">See also</span></span>



- [<span data-ttu-id="5ff98-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ff98-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

