---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: '[Conflict Ting面会 Count] 要素は、予定表アイテムと競合する会議の数を表します。'
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463861"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="d13fb-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="d13fb-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="d13fb-104">[Conflict **ting面会 count** ] 要素は、予定表アイテムと競合する会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="d13fb-105">**int**</span><span class="sxs-lookup"><span data-stu-id="d13fb-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d13fb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d13fb-106">Attributes and elements</span></span>

<span data-ttu-id="d13fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d13fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="d13fb-108">Attributes</span></span>

<span data-ttu-id="d13fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d13fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d13fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d13fb-110">Child elements</span></span>

<span data-ttu-id="d13fb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d13fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d13fb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d13fb-112">Parent elements</span></span>

|<span data-ttu-id="d13fb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d13fb-113">**Element**</span></span>|<span data-ttu-id="d13fb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d13fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d13fb-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d13fb-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d13fb-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d13fb-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d13fb-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d13fb-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d13fb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d13fb-119">Text value</span></span>

<span data-ttu-id="d13fb-120">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-120">The text value represents an integer.</span></span> <span data-ttu-id="d13fb-121">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d13fb-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d13fb-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d13fb-122">Remarks</span></span>

<span data-ttu-id="d13fb-123">予定表アイテムは、少なくとも部分的に、同じ予定表フォルダー内の別の予定表アイテムと同じタイミングで発生した場合に競合していると見なされます。</span><span class="sxs-lookup"><span data-stu-id="d13fb-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="d13fb-124">予定表アイテムが予定表以外のフォルダーにある場合は、既定の予定表フォルダー内の予定表アイテムと比較されます。</span><span class="sxs-lookup"><span data-stu-id="d13fb-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="d13fb-125">会議出席依頼は、既定の予定表フォルダー内の予定表アイテムと比較されます。</span><span class="sxs-lookup"><span data-stu-id="d13fb-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="d13fb-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d13fb-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d13fb-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d13fb-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d13fb-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="d13fb-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d13fb-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d13fb-129">Schema name</span></span>  <br/> |<span data-ttu-id="d13fb-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d13fb-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d13fb-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d13fb-131">Validation file</span></span>  <br/> |<span data-ttu-id="d13fb-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d13fb-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d13fb-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d13fb-133">Can be empty</span></span>  <br/> |<span data-ttu-id="d13fb-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="d13fb-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d13fb-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="d13fb-135">See also</span></span>



- [<span data-ttu-id="d13fb-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d13fb-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

