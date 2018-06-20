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
description: MeetingWorkspaceUrl 要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。 会議ワークスペースは、共有の Web サイトの会議を計画し、結果を追跡します。
ms.openlocfilehash: 7d84547eafe4e77fb23a792fbf15633dbf93d775
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832436"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="31797-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="31797-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="31797-105">**MeetingWorkspaceUrl**要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="31797-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="31797-106">会議ワークスペースは、共有の Web サイトの会議を計画し、結果を追跡します。</span><span class="sxs-lookup"><span data-stu-id="31797-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="31797-107">**string**</span><span class="sxs-lookup"><span data-stu-id="31797-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31797-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31797-108">Attributes and elements</span></span>

<span data-ttu-id="31797-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31797-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31797-110">属性</span><span class="sxs-lookup"><span data-stu-id="31797-110">Attributes</span></span>

<span data-ttu-id="31797-111">なし。</span><span class="sxs-lookup"><span data-stu-id="31797-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31797-112">子要素</span><span class="sxs-lookup"><span data-stu-id="31797-112">Child elements</span></span>

<span data-ttu-id="31797-113">なし。</span><span class="sxs-lookup"><span data-stu-id="31797-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31797-114">親要素</span><span class="sxs-lookup"><span data-stu-id="31797-114">Parent elements</span></span>

|<span data-ttu-id="31797-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="31797-115">**Element**</span></span>|<span data-ttu-id="31797-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="31797-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31797-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="31797-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="31797-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="31797-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="31797-119">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="31797-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="31797-120">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="31797-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31797-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="31797-121">Text value</span></span>

<span data-ttu-id="31797-122">URL を表す文字列値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="31797-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31797-123">備考</span><span class="sxs-lookup"><span data-stu-id="31797-123">Remarks</span></span>

<span data-ttu-id="31797-124">MeetingWorkspaceUrl プロパティは、開催者の予定表アイテムの読み取り-書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="31797-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="31797-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="31797-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="31797-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="31797-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31797-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="31797-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31797-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="31797-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31797-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31797-129">Schema name</span></span>  <br/> |<span data-ttu-id="31797-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="31797-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="31797-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31797-131">Validation file</span></span>  <br/> |<span data-ttu-id="31797-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31797-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31797-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31797-133">Can be empty</span></span>  <br/> |<span data-ttu-id="31797-134">False</span><span class="sxs-lookup"><span data-stu-id="31797-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31797-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="31797-135">See also</span></span>



- [<span data-ttu-id="31797-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="31797-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

