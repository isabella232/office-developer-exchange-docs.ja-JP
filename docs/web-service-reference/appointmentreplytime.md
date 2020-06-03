---
title: AppointmentReplyTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentReplyTime
api_type:
- schema
ms.assetid: 7784468c-c863-488a-864b-ce4d6c671dbe
description: AppointmentReplyTime 要素は、出席者が会議出席依頼に返信した日付と時刻を表します。
ms.openlocfilehash: 188cd5fbaaefa52e4324143a2ee89ae8dbca7742
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463497"
---
# <a name="appointmentreplytime"></a><span data-ttu-id="d912c-103">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="d912c-103">AppointmentReplyTime</span></span>

<span data-ttu-id="d912c-104">**AppointmentReplyTime**要素は、出席者が会議出席依頼に返信した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="d912c-104">The **AppointmentReplyTime** element represents the date and time that an attendee replied to a meeting request.</span></span> 
  
```xml
<AppointmentReplyTime/>
```

 <span data-ttu-id="d912c-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="d912c-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d912c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d912c-106">Attributes and elements</span></span>

<span data-ttu-id="d912c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d912c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d912c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d912c-108">Attributes</span></span>

<span data-ttu-id="d912c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d912c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d912c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d912c-110">Child elements</span></span>

<span data-ttu-id="d912c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d912c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d912c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d912c-112">Parent elements</span></span>

|<span data-ttu-id="d912c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d912c-113">**Element**</span></span>|<span data-ttu-id="d912c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d912c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d912c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d912c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d912c-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d912c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d912c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d912c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d912c-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d912c-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d912c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d912c-119">Text value</span></span>

<span data-ttu-id="d912c-120">日付と時刻を表す文字列。</span><span class="sxs-lookup"><span data-stu-id="d912c-120">A string that represents a date and time.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d912c-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d912c-121">Remarks</span></span>

<span data-ttu-id="d912c-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d912c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d912c-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d912c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d912c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d912c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d912c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d912c-125">Schema name</span></span>  <br/> |<span data-ttu-id="d912c-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d912c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d912c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d912c-127">Validation file</span></span>  <br/> |<span data-ttu-id="d912c-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d912c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d912c-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d912c-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d912c-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="d912c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d912c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d912c-131">See also</span></span>

- [<span data-ttu-id="d912c-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d912c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

