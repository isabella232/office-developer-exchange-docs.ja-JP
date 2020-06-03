---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: IsMeeting 要素は、予定表アイテムが会議と予定のどちらであるかを示します。
ms.openlocfilehash: fd72766977567210cd08b47d0723cd73aa53a622
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465969"
---
# <a name="ismeeting"></a><span data-ttu-id="1f24a-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="1f24a-103">IsMeeting</span></span>

<span data-ttu-id="1f24a-104">**Ismeeting**要素は、予定表アイテムが会議と予定のどちらであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="1f24a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1f24a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f24a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f24a-106">Attributes and elements</span></span>

<span data-ttu-id="1f24a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f24a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f24a-108">Attributes</span></span>

<span data-ttu-id="1f24a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1f24a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f24a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1f24a-110">Child elements</span></span>

<span data-ttu-id="1f24a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1f24a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f24a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1f24a-112">Parent elements</span></span>

|<span data-ttu-id="1f24a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f24a-113">**Element**</span></span>|<span data-ttu-id="1f24a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f24a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f24a-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="1f24a-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="1f24a-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1f24a-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1f24a-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1f24a-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f24a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1f24a-119">Text value</span></span>

<span data-ttu-id="1f24a-120">この要素が含まれている場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f24a-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="1f24a-121">**True**の値は、予定表アイテムが会議であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="1f24a-122">値が**false**の場合、予定表アイテムが予定であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1f24a-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1f24a-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1f24a-123">Remarks</span></span>

<span data-ttu-id="1f24a-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f24a-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f24a-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f24a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f24a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f24a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f24a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f24a-127">Schema name</span></span>  <br/> |<span data-ttu-id="1f24a-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f24a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f24a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f24a-129">Validation file</span></span>  <br/> |<span data-ttu-id="1f24a-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1f24a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f24a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f24a-131">Can be empty</span></span>  <br/> |<span data-ttu-id="1f24a-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f24a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f24a-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f24a-133">See also</span></span>



- [<span data-ttu-id="1f24a-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f24a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

