---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: IsOrganizer 要素は、このユーザーが会議の開催者であるかどうかを示すブール値を指定します。
ms.openlocfilehash: 5fd775cfc0a296c08d19d0468d96aa36ba67ddd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832063"
---
# <a name="isorganizer"></a><span data-ttu-id="57e37-103">IsOrganizer</span><span class="sxs-lookup"><span data-stu-id="57e37-103">IsOrganizer</span></span>

<span data-ttu-id="57e37-104">**IsOrganizer**要素は、このユーザーが会議の開催者であるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="57e37-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="57e37-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="57e37-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57e37-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57e37-106">Attributes and elements</span></span>

<span data-ttu-id="57e37-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57e37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57e37-108">属性</span><span class="sxs-lookup"><span data-stu-id="57e37-108">Attributes</span></span>

<span data-ttu-id="57e37-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57e37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57e37-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57e37-110">Child elements</span></span>

<span data-ttu-id="57e37-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57e37-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57e37-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57e37-112">Parent elements</span></span>

|<span data-ttu-id="57e37-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="57e37-113">**Element**</span></span>|<span data-ttu-id="57e37-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="57e37-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57e37-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="57e37-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="57e37-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57e37-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="57e37-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="57e37-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="57e37-118">会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="57e37-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57e37-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57e37-119">Text value</span></span>

<span data-ttu-id="57e37-120">の**場合は true** 、 **IsOrganizer**要素のテキスト値は、予定表アイテムまたは会議のメッセージがユーザーによって作成されたものであることを示します。</span><span class="sxs-lookup"><span data-stu-id="57e37-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="57e37-121">**False**の値は、予定表アイテムまたは会議のメッセージでは、bv、ユーザーは作成されなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="57e37-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="57e37-122">備考</span><span class="sxs-lookup"><span data-stu-id="57e37-122">Remarks</span></span>

<span data-ttu-id="57e37-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57e37-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57e37-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57e37-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57e37-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="57e37-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57e37-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="57e37-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57e37-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57e37-127">Schema Name</span></span>  <br/> |<span data-ttu-id="57e37-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="57e37-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="57e37-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57e37-129">Validation File</span></span>  <br/> |<span data-ttu-id="57e37-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="57e37-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="57e37-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="57e37-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="57e37-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="57e37-132">See also</span></span>



- [<span data-ttu-id="57e37-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="57e37-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

