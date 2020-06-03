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
description: '[Conflict Tingmeeting] 要素は、会議時間と競合するすべての予定表アイテムを識別します。'
ms.openlocfilehash: dc897c9dc33117d379d89bb9bb41104ca02def1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460177"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="46c3d-103">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="46c3d-103">ConflictingMeetings</span></span>

<span data-ttu-id="46c3d-104">[Conflict **tingmeeting** ] 要素は、会議時間と競合するすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="46c3d-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="46c3d-105">**非 Emptyarrayofallitemstype**</span><span class="sxs-lookup"><span data-stu-id="46c3d-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46c3d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="46c3d-106">Attributes and elements</span></span>

<span data-ttu-id="46c3d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46c3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46c3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="46c3d-108">Attributes</span></span>

<span data-ttu-id="46c3d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="46c3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46c3d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="46c3d-110">Child elements</span></span>

|<span data-ttu-id="46c3d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="46c3d-111">**Element**</span></span>|<span data-ttu-id="46c3d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="46c3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46c3d-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="46c3d-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="46c3d-114">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="46c3d-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46c3d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="46c3d-115">Parent elements</span></span>

|<span data-ttu-id="46c3d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="46c3d-116">**Element**</span></span>|<span data-ttu-id="46c3d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="46c3d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46c3d-118">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="46c3d-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="46c3d-119">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="46c3d-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46c3d-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="46c3d-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="46c3d-121">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="46c3d-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46c3d-122">注釈</span><span class="sxs-lookup"><span data-stu-id="46c3d-122">Remarks</span></span>

<span data-ttu-id="46c3d-123">この要素を使用する場合は、1つ以上の子要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="46c3d-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="46c3d-124">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="46c3d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="46c3d-125">追加の子要素はスキーマに従って有効になりますが、 [Calendaritem](calendaritem.md)要素は、Exchange Web サービス (EWS) が競合している**会議**要素内で返す唯一の子要素です。</span><span class="sxs-lookup"><span data-stu-id="46c3d-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="46c3d-126">このトピックでは、スキーマに従って有効な子要素は表示されませんが、EWS では返されません。</span><span class="sxs-lookup"><span data-stu-id="46c3d-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="46c3d-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="46c3d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46c3d-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="46c3d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46c3d-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46c3d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="46c3d-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="46c3d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="46c3d-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46c3d-131">Validation File</span></span>  <br/> |<span data-ttu-id="46c3d-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="46c3d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46c3d-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46c3d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="46c3d-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="46c3d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46c3d-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="46c3d-135">See also</span></span>



- [<span data-ttu-id="46c3d-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="46c3d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

