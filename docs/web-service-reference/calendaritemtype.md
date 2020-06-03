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
ms.openlocfilehash: 05e93b6db3ae574c03f6e43c5ebec2288edec3e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527195"
---
# <a name="calendaritemtype"></a><span data-ttu-id="da8a1-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="da8a1-103">CalendarItemType</span></span>

<span data-ttu-id="da8a1-104">**Calendaritemtype**要素は、予定表アイテムの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="da8a1-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="da8a1-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="da8a1-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da8a1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="da8a1-106">Attributes and elements</span></span>

<span data-ttu-id="da8a1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da8a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da8a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="da8a1-108">Attributes</span></span>

<span data-ttu-id="da8a1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da8a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da8a1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da8a1-110">Child elements</span></span>

<span data-ttu-id="da8a1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da8a1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da8a1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da8a1-112">Parent elements</span></span>

|<span data-ttu-id="da8a1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="da8a1-113">**Element**</span></span>|<span data-ttu-id="da8a1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="da8a1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da8a1-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="da8a1-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="da8a1-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="da8a1-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da8a1-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="da8a1-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="da8a1-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="da8a1-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da8a1-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da8a1-119">Text value</span></span>

<span data-ttu-id="da8a1-120">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="da8a1-120">A text value is required if this element is used.</span></span> <span data-ttu-id="da8a1-121">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="da8a1-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="da8a1-122">**Single**アイテムは、定期的な予定表アイテムに関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="da8a1-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="da8a1-123">**発生**アイテムは、定期的な予定表アイテムの発生になります。</span><span class="sxs-lookup"><span data-stu-id="da8a1-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="da8a1-124">**例外**アイテムは、定期的な予定表アイテムの例外です。</span><span class="sxs-lookup"><span data-stu-id="da8a1-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="da8a1-125">**示す**アイテムは、一連の定期的な予定表アイテムのマスターシェイプです。</span><span class="sxs-lookup"><span data-stu-id="da8a1-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="da8a1-126">注釈</span><span class="sxs-lookup"><span data-stu-id="da8a1-126">Remarks</span></span>

<span data-ttu-id="da8a1-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="da8a1-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da8a1-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="da8a1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da8a1-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="da8a1-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da8a1-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da8a1-130">Schema name</span></span>  <br/> |<span data-ttu-id="da8a1-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="da8a1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="da8a1-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da8a1-132">Validation file</span></span>  <br/> |<span data-ttu-id="da8a1-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="da8a1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da8a1-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="da8a1-134">Can be empty</span></span>  <br/> |<span data-ttu-id="da8a1-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="da8a1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da8a1-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="da8a1-136">See also</span></span>



- [<span data-ttu-id="da8a1-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="da8a1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

