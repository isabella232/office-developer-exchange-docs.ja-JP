---
title: MeetingRequestWasSent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestWasSent
api_type:
- schema
ms.assetid: 9192400a-8eef-4147-9f94-aa8ea91b41d8
description: MeetingRequestWasSent 要素は、会議出席依頼が出席者に送信されたかどうかを示します。
ms.openlocfilehash: d5005eb86d5f8d2f438a69e634f0617c2311d720
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465766"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="7658e-103">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="7658e-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="7658e-104">**MeetingRequestWasSent**要素は、会議出席依頼が出席者に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7658e-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="7658e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7658e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7658e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7658e-106">Attributes and elements</span></span>

<span data-ttu-id="7658e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7658e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7658e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7658e-108">Attributes</span></span>

<span data-ttu-id="7658e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7658e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7658e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7658e-110">Child elements</span></span>

<span data-ttu-id="7658e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7658e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7658e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7658e-112">Parent elements</span></span>

|<span data-ttu-id="7658e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7658e-113">**Element**</span></span>|<span data-ttu-id="7658e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7658e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7658e-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7658e-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7658e-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7658e-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7658e-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7658e-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7658e-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7658e-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7658e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7658e-119">Text value</span></span>

<span data-ttu-id="7658e-120">この要素が含まれている場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7658e-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="7658e-121">**True**の値は、会議出席依頼が送信されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="7658e-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="7658e-122">値が**false**の場合は、会議出席依頼が送信されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="7658e-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7658e-123">注釈</span><span class="sxs-lookup"><span data-stu-id="7658e-123">Remarks</span></span>

<span data-ttu-id="7658e-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7658e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7658e-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7658e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7658e-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="7658e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7658e-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7658e-127">Schema name</span></span>  <br/> |<span data-ttu-id="7658e-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7658e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7658e-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7658e-129">Validation file</span></span>  <br/> |<span data-ttu-id="7658e-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7658e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7658e-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7658e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="7658e-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="7658e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7658e-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7658e-133">See also</span></span>



- [<span data-ttu-id="7658e-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7658e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

