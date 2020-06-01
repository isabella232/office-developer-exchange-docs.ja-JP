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
ms.openlocfilehash: 45b7a66068dc00f6e60b7380240bea6836282fd4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466564"
---
# <a name="isorganizer"></a><span data-ttu-id="e3b1a-103">IsOrganizer</span><span class="sxs-lookup"><span data-stu-id="e3b1a-103">IsOrganizer</span></span>

<span data-ttu-id="e3b1a-104">**Isorganizer**要素は、このユーザーが会議の開催者であるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="e3b1a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e3b1a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3b1a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e3b1a-106">Attributes and elements</span></span>

<span data-ttu-id="e3b1a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3b1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3b1a-108">Attributes</span></span>

<span data-ttu-id="e3b1a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3b1a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3b1a-110">Child elements</span></span>

<span data-ttu-id="e3b1a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e3b1a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e3b1a-112">Parent elements</span></span>

|<span data-ttu-id="e3b1a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3b1a-113">**Element**</span></span>|<span data-ttu-id="e3b1a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3b1a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3b1a-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="e3b1a-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e3b1a-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e3b1a-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e3b1a-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e3b1a-118">会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3b1a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e3b1a-119">Text value</span></span>

<span data-ttu-id="e3b1a-120">**Isorganizer**要素のテキスト値が**true の場合**は、予定表アイテムまたは会議メッセージがユーザーによって作成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="e3b1a-121">値が**false**の場合、予定表アイテムまたは会議メッセージがユーザー bv 作成されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e3b1a-122">注釈</span><span class="sxs-lookup"><span data-stu-id="e3b1a-122">Remarks</span></span>

<span data-ttu-id="e3b1a-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e3b1a-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3b1a-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e3b1a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3b1a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3b1a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3b1a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3b1a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e3b1a-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e3b1a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e3b1a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3b1a-129">Validation File</span></span>  <br/> |<span data-ttu-id="e3b1a-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e3b1a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3b1a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e3b1a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e3b1a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3b1a-132">See also</span></span>



- [<span data-ttu-id="e3b1a-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e3b1a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

