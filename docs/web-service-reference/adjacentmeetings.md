---
title: AdjacentMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: AdjacentMeetings 要素は、会議の時刻に隣接しているすべての予定表アイテムを識別します。
ms.openlocfilehash: 7c89095e24af799df22a848be06a0fd65d53be7f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463581"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="50ab6-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="50ab6-103">AdjacentMeetings</span></span>

<span data-ttu-id="50ab6-104">**AdjacentMeetings**要素は、会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="50ab6-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="50ab6-105">**非 Emptyarrayofallitemstype**</span><span class="sxs-lookup"><span data-stu-id="50ab6-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50ab6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="50ab6-106">Attributes and elements</span></span>

<span data-ttu-id="50ab6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50ab6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50ab6-108">属性</span><span class="sxs-lookup"><span data-stu-id="50ab6-108">Attributes</span></span>

<span data-ttu-id="50ab6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="50ab6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50ab6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="50ab6-110">Child elements</span></span>

|<span data-ttu-id="50ab6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="50ab6-111">**Element**</span></span>|<span data-ttu-id="50ab6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="50ab6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50ab6-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="50ab6-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="50ab6-114">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="50ab6-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50ab6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="50ab6-115">Parent elements</span></span>

|<span data-ttu-id="50ab6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="50ab6-116">**Element**</span></span>|<span data-ttu-id="50ab6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="50ab6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50ab6-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="50ab6-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="50ab6-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="50ab6-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="50ab6-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="50ab6-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="50ab6-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="50ab6-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50ab6-122">注釈</span><span class="sxs-lookup"><span data-stu-id="50ab6-122">Remarks</span></span>

<span data-ttu-id="50ab6-123">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="50ab6-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="50ab6-124">追加の子要素はスキーマに従って有効ですが、 [Calendaritem](calendaritem.md)要素は、Exchange Web サービス (EWS) が**AdjacentMeetings**要素内で返す唯一の子要素です。</span><span class="sxs-lookup"><span data-stu-id="50ab6-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="50ab6-125">このトピックでは、スキーマに従って有効な子要素は表示されませんが、EWS では返されません。</span><span class="sxs-lookup"><span data-stu-id="50ab6-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="50ab6-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="50ab6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50ab6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="50ab6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50ab6-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="50ab6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="50ab6-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="50ab6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="50ab6-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="50ab6-130">Validation File</span></span>  <br/> |<span data-ttu-id="50ab6-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="50ab6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50ab6-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="50ab6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="50ab6-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="50ab6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50ab6-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="50ab6-134">See also</span></span>

- [<span data-ttu-id="50ab6-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="50ab6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

