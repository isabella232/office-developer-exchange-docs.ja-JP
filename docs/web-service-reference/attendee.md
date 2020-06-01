---
title: 参加者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: 出席者要素は、会議の出席者とリソースを表します。
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457649"
---
# <a name="attendee"></a><span data-ttu-id="9eedd-103">参加者</span><span class="sxs-lookup"><span data-stu-id="9eedd-103">Attendee</span></span>

<span data-ttu-id="9eedd-104">出席**者**要素は、会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="9eedd-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="9eedd-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9eedd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9eedd-106">Attributes and elements</span></span>

<span data-ttu-id="9eedd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9eedd-108">属性</span><span class="sxs-lookup"><span data-stu-id="9eedd-108">Attributes</span></span>

<span data-ttu-id="9eedd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9eedd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9eedd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9eedd-110">Child elements</span></span>

|<span data-ttu-id="9eedd-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9eedd-111">**Element**</span></span>|<span data-ttu-id="9eedd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9eedd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eedd-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="9eedd-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9eedd-114">完全に解決された電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="9eedd-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="9eedd-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="9eedd-116">会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="9eedd-117">このプロパティは、会議開催者の予定表アイテムにのみ関連しています。</span><span class="sxs-lookup"><span data-stu-id="9eedd-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9eedd-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="9eedd-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="9eedd-119">受信された最新の応答の日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
|[<span data-ttu-id="9eedd-120">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="9eedd-120">ProposedStart</span></span>](proposedstart-attendeetype.md) <br/> |<span data-ttu-id="9eedd-121">会議の出席者が提案した開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-121">Represents an attendee's proposed start time for a meeting.</span></span> <br/> |
|[<span data-ttu-id="9eedd-122">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="9eedd-122">ProposedEnd</span></span>](proposedend-attendeetype.md) <br/> |<span data-ttu-id="9eedd-123">会議の出席者が提案した終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-123">Represents an attendee's proposed end time for a meeting.</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9eedd-124">親要素</span><span class="sxs-lookup"><span data-stu-id="9eedd-124">Parent elements</span></span>

|<span data-ttu-id="9eedd-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="9eedd-125">**Element**</span></span>|<span data-ttu-id="9eedd-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="9eedd-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eedd-127">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="9eedd-127">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="9eedd-128">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-128">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9eedd-129">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="9eedd-129">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="9eedd-130">会議に出席する必要がない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-130">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9eedd-131">リソース</span><span class="sxs-lookup"><span data-stu-id="9eedd-131">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="9eedd-132">会議のスケジュールされたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="9eedd-132">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9eedd-133">注釈</span><span class="sxs-lookup"><span data-stu-id="9eedd-133">Remarks</span></span>

<span data-ttu-id="9eedd-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9eedd-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9eedd-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9eedd-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9eedd-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="9eedd-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9eedd-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9eedd-137">Schema name</span></span>  <br/> |<span data-ttu-id="9eedd-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9eedd-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="9eedd-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9eedd-139">Validation file</span></span>  <br/> |<span data-ttu-id="9eedd-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9eedd-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9eedd-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9eedd-141">Can be empty</span></span>  <br/> |<span data-ttu-id="9eedd-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="9eedd-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9eedd-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="9eedd-143">See also</span></span>

- [<span data-ttu-id="9eedd-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9eedd-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

