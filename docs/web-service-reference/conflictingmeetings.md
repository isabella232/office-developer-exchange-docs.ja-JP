---
title: ConflictingMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetings
api_type:
- schema
ms.assetid: cfff7a11-7b3a-4995-9815-afedd45ebb0f
description: ConflictingMeetings 要素は、会議の時間と競合するすべての予定表アイテムを識別します。
ms.openlocfilehash: 1d2558dba41ec3e7ae2711bb2dc26f54cada827a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759654"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="2fca4-103">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="2fca4-103">ConflictingMeetings</span></span>

<span data-ttu-id="2fca4-104">**ConflictingMeetings**要素は、会議の時間と競合するすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="2fca4-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="2fca4-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="2fca4-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fca4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2fca4-106">Attributes and elements</span></span>

<span data-ttu-id="2fca4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2fca4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fca4-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fca4-108">Attributes</span></span>

<span data-ttu-id="2fca4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2fca4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fca4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2fca4-110">Child elements</span></span>

|<span data-ttu-id="2fca4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2fca4-111">**Element**</span></span>|<span data-ttu-id="2fca4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fca4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fca4-113">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="2fca4-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2fca4-114">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2fca4-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fca4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2fca4-115">Parent elements</span></span>

|<span data-ttu-id="2fca4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2fca4-116">**Element**</span></span>|<span data-ttu-id="2fca4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fca4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fca4-118">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2fca4-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2fca4-119">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="2fca4-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2fca4-120">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="2fca4-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2fca4-121">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2fca4-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2fca4-122">備考</span><span class="sxs-lookup"><span data-stu-id="2fca4-122">Remarks</span></span>

<span data-ttu-id="2fca4-123">この要素を使用する場合 1 つまたは複数の子要素が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fca4-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="2fca4-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2fca4-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2fca4-125">追加の子要素は、スキーマの有効な[カレンダー項目](calendaritem.md)要素は、 **ConflictingMeetings**要素内で Exchange Web サービス (EWS) から返される唯一の子要素です。</span><span class="sxs-lookup"><span data-stu-id="2fca4-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="2fca4-126">このトピックでは、スキーマでは有効が EWS では返されませんが、子要素が指定されていません。</span><span class="sxs-lookup"><span data-stu-id="2fca4-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2fca4-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="2fca4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fca4-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="2fca4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fca4-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2fca4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="2fca4-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2fca4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="2fca4-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2fca4-131">Validation File</span></span>  <br/> |<span data-ttu-id="2fca4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2fca4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fca4-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2fca4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fca4-134">False</span><span class="sxs-lookup"><span data-stu-id="2fca4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fca4-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="2fca4-135">See also</span></span>



- [<span data-ttu-id="2fca4-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2fca4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

