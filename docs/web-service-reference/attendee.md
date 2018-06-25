---
title: Attendee
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
description: 出席者の要素では、出席者および会議のためのリソースを表します。
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759457"
---
# <a name="attendee"></a><span data-ttu-id="9027e-103">Attendee</span><span class="sxs-lookup"><span data-stu-id="9027e-103">Attendee</span></span>

<span data-ttu-id="9027e-104">**出席者**の要素では、出席者および会議のためのリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="9027e-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="9027e-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9027e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9027e-106">Attributes and elements</span></span>

<span data-ttu-id="9027e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9027e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9027e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9027e-108">Attributes</span></span>

<span data-ttu-id="9027e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9027e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9027e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9027e-110">Child elements</span></span>

|<span data-ttu-id="9027e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9027e-111">**Element**</span></span>|<span data-ttu-id="9027e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9027e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9027e-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="9027e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9027e-114">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="9027e-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="9027e-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="9027e-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="9027e-116">会議を受信する受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="9027e-117">このプロパティは、会議の開催者の予定表アイテムに関連するだけです。</span><span class="sxs-lookup"><span data-stu-id="9027e-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9027e-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="9027e-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="9027e-119">日付と時刻を受信した最新の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9027e-120">親要素</span><span class="sxs-lookup"><span data-stu-id="9027e-120">Parent elements</span></span>

|<span data-ttu-id="9027e-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="9027e-121">**Element**</span></span>|<span data-ttu-id="9027e-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="9027e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9027e-123">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="9027e-123">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="9027e-124">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-124">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9027e-125">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="9027e-125">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="9027e-126">出席者が会議に出席する必要がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-126">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9027e-127">リソース</span><span class="sxs-lookup"><span data-stu-id="9027e-127">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="9027e-128">会議のスケジュール設定されたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="9027e-128">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9027e-129">備考</span><span class="sxs-lookup"><span data-stu-id="9027e-129">Remarks</span></span>

<span data-ttu-id="9027e-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9027e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9027e-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="9027e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9027e-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="9027e-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9027e-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9027e-133">Schema name</span></span>  <br/> |<span data-ttu-id="9027e-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9027e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="9027e-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9027e-135">Validation file</span></span>  <br/> |<span data-ttu-id="9027e-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9027e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9027e-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9027e-137">Can be empty</span></span>  <br/> |<span data-ttu-id="9027e-138">False</span><span class="sxs-lookup"><span data-stu-id="9027e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9027e-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="9027e-139">See also</span></span>

- [<span data-ttu-id="9027e-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9027e-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

