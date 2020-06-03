---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: MeetingWorkspaceUrl 要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。 会議ワークスペースは、会議を計画し、結果を追跡するための共有の Web サイトです。
ms.openlocfilehash: cd4396e590ab1471278bd44b9a4e0009fe326eaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466284"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="88aec-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="88aec-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="88aec-105">**MeetingWorkspaceUrl**要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="88aec-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="88aec-106">会議ワークスペースは、会議を計画し、結果を追跡するための共有の Web サイトです。</span><span class="sxs-lookup"><span data-stu-id="88aec-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="88aec-107">**string**</span><span class="sxs-lookup"><span data-stu-id="88aec-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88aec-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="88aec-108">Attributes and elements</span></span>

<span data-ttu-id="88aec-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="88aec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88aec-110">属性</span><span class="sxs-lookup"><span data-stu-id="88aec-110">Attributes</span></span>

<span data-ttu-id="88aec-111">なし。</span><span class="sxs-lookup"><span data-stu-id="88aec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88aec-112">子要素</span><span class="sxs-lookup"><span data-stu-id="88aec-112">Child elements</span></span>

<span data-ttu-id="88aec-113">なし。</span><span class="sxs-lookup"><span data-stu-id="88aec-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88aec-114">親要素</span><span class="sxs-lookup"><span data-stu-id="88aec-114">Parent elements</span></span>

|<span data-ttu-id="88aec-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="88aec-115">**Element**</span></span>|<span data-ttu-id="88aec-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="88aec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88aec-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="88aec-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="88aec-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="88aec-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="88aec-119">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="88aec-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="88aec-120">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="88aec-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88aec-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="88aec-121">Text value</span></span>

<span data-ttu-id="88aec-122">この要素を使用する場合は、URL を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="88aec-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88aec-123">注釈</span><span class="sxs-lookup"><span data-stu-id="88aec-123">Remarks</span></span>

<span data-ttu-id="88aec-124">MeetingWorkspaceUrl プロパティは、開催者の予定表アイテムの読み取り/書き込みが可能です。</span><span class="sxs-lookup"><span data-stu-id="88aec-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="88aec-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="88aec-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="88aec-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="88aec-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88aec-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="88aec-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88aec-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="88aec-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88aec-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="88aec-129">Schema name</span></span>  <br/> |<span data-ttu-id="88aec-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="88aec-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="88aec-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="88aec-131">Validation file</span></span>  <br/> |<span data-ttu-id="88aec-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="88aec-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88aec-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="88aec-133">Can be empty</span></span>  <br/> |<span data-ttu-id="88aec-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="88aec-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88aec-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="88aec-135">See also</span></span>



- [<span data-ttu-id="88aec-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="88aec-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

