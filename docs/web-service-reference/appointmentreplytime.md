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
description: AppointmentReplyTime 要素は、出席者が会議出席依頼に返信するときの日時を表します。
ms.openlocfilehash: 4d524bdc36ee642dcf8186294d412d6849b59ade
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759416"
---
# <a name="appointmentreplytime"></a><span data-ttu-id="d013b-103">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="d013b-103">AppointmentReplyTime</span></span>

<span data-ttu-id="d013b-104">**AppointmentReplyTime**要素は、出席者が会議出席依頼に返信するときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="d013b-104">The **AppointmentReplyTime** element represents the date and time that an attendee replied to a meeting request.</span></span> 
  
```xml
<AppointmentReplyTime/>
```

 <span data-ttu-id="d013b-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="d013b-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d013b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d013b-106">Attributes and elements</span></span>

<span data-ttu-id="d013b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d013b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d013b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d013b-108">Attributes</span></span>

<span data-ttu-id="d013b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d013b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d013b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d013b-110">Child elements</span></span>

<span data-ttu-id="d013b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d013b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d013b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d013b-112">Parent elements</span></span>

|<span data-ttu-id="d013b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d013b-113">**Element**</span></span>|<span data-ttu-id="d013b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d013b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d013b-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="d013b-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d013b-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d013b-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d013b-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d013b-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d013b-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d013b-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d013b-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d013b-119">Text value</span></span>

<span data-ttu-id="d013b-120">日付と時刻を表す文字列。</span><span class="sxs-lookup"><span data-stu-id="d013b-120">A string that represents a date and time.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d013b-121">備考</span><span class="sxs-lookup"><span data-stu-id="d013b-121">Remarks</span></span>

<span data-ttu-id="d013b-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d013b-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d013b-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="d013b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d013b-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="d013b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d013b-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d013b-125">Schema name</span></span>  <br/> |<span data-ttu-id="d013b-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d013b-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d013b-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d013b-127">Validation file</span></span>  <br/> |<span data-ttu-id="d013b-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d013b-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d013b-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d013b-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d013b-130">False</span><span class="sxs-lookup"><span data-stu-id="d013b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d013b-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d013b-131">See also</span></span>

- [<span data-ttu-id="d013b-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d013b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

