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
ms.openlocfilehash: 9ab818f4f67c32c01101cc595ccb92424a872ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759302"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="c559b-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="c559b-103">AdjacentMeetings</span></span>

<span data-ttu-id="c559b-104">**AdjacentMeetings**要素は、会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c559b-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="c559b-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="c559b-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c559b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c559b-106">Attributes and elements</span></span>

<span data-ttu-id="c559b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c559b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c559b-108">属性</span><span class="sxs-lookup"><span data-stu-id="c559b-108">Attributes</span></span>

<span data-ttu-id="c559b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c559b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c559b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c559b-110">Child elements</span></span>

|<span data-ttu-id="c559b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c559b-111">**Element**</span></span>|<span data-ttu-id="c559b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c559b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c559b-113">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c559b-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c559b-114">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c559b-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c559b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c559b-115">Parent elements</span></span>

|<span data-ttu-id="c559b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c559b-116">**Element**</span></span>|<span data-ttu-id="c559b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c559b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c559b-118">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c559b-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c559b-119">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c559b-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c559b-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c559b-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c559b-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c559b-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c559b-122">備考</span><span class="sxs-lookup"><span data-stu-id="c559b-122">Remarks</span></span>

<span data-ttu-id="c559b-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c559b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c559b-124">追加の子要素は、スキーマの有効な[カレンダー項目](calendaritem.md)要素は、 **AdjacentMeetings**要素内で Exchange Web サービス (EWS) から返される唯一の子要素です。</span><span class="sxs-lookup"><span data-stu-id="c559b-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="c559b-125">このトピックでは、スキーマでは有効が EWS では返されませんが、子要素が指定されていません。</span><span class="sxs-lookup"><span data-stu-id="c559b-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c559b-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="c559b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c559b-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="c559b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c559b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c559b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c559b-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c559b-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c559b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c559b-130">Validation File</span></span>  <br/> |<span data-ttu-id="c559b-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c559b-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c559b-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c559b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c559b-133">False</span><span class="sxs-lookup"><span data-stu-id="c559b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c559b-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="c559b-134">See also</span></span>

- [<span data-ttu-id="c559b-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c559b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

