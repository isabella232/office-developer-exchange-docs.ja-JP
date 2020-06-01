---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: AllowNewTimeProposal 要素は、新しい会議日時を出席者の会議のために提案できるかどうかを示します。
ms.openlocfilehash: b3f2c569bced08c66144680a4fddd6e8bac0cecf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464806"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="34de8-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="34de8-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="34de8-104">**Allownewtimeproposal**要素は、新しい会議日時を出席者の会議のために提案できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="34de8-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="34de8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="34de8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34de8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="34de8-106">Attributes and elements</span></span>

<span data-ttu-id="34de8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="34de8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34de8-108">属性</span><span class="sxs-lookup"><span data-stu-id="34de8-108">Attributes</span></span>

<span data-ttu-id="34de8-109">なし</span><span class="sxs-lookup"><span data-stu-id="34de8-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34de8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="34de8-110">Child elements</span></span>

<span data-ttu-id="34de8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="34de8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34de8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="34de8-112">Parent elements</span></span>

|<span data-ttu-id="34de8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="34de8-113">**Element**</span></span>|<span data-ttu-id="34de8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="34de8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34de8-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="34de8-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="34de8-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="34de8-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="34de8-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="34de8-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="34de8-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="34de8-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34de8-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="34de8-119">Text value</span></span>

<span data-ttu-id="34de8-120">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="34de8-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="34de8-121">**True**の値は、会議時間の新しい提案を作成できることを示します。値が**false**の場合は、新しい時間提案が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="34de8-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="34de8-122">開催者は、会議出席依頼にこの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="34de8-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="34de8-123">注釈</span><span class="sxs-lookup"><span data-stu-id="34de8-123">Remarks</span></span>

<span data-ttu-id="34de8-124">AllowNewTimeProposal プロパティは、開催者の予定表アイテムに対しては読み取り/書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="34de8-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="34de8-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="34de8-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="34de8-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="34de8-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="34de8-127">Exchange Web サービスは新しい時間提案メッセージをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="34de8-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="34de8-128">新しい時間提案メッセージに関連するプロパティを取得するには、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="34de8-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="34de8-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="34de8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34de8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="34de8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34de8-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="34de8-131">Schema name</span></span>  <br/> |<span data-ttu-id="34de8-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="34de8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="34de8-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="34de8-133">Validation file</span></span>  <br/> |<span data-ttu-id="34de8-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="34de8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34de8-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="34de8-135">Can be empty</span></span>  <br/> |<span data-ttu-id="34de8-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="34de8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34de8-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="34de8-137">See also</span></span>

- [<span data-ttu-id="34de8-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="34de8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

