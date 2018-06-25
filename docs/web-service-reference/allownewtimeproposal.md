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
description: AllowNewTimeProposal 要素は、かどうか会議の新しい日時を提案できるは会議の出席者でことを示します。
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759311"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="3b388-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="3b388-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="3b388-104">**AllowNewTimeProposal**要素は、かどうか会議の新しい日時を提案できるは会議の出席者でことを示します。</span><span class="sxs-lookup"><span data-stu-id="3b388-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="3b388-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="3b388-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b388-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3b388-106">Attributes and elements</span></span>

<span data-ttu-id="3b388-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3b388-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b388-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b388-108">Attributes</span></span>

<span data-ttu-id="3b388-109">なし</span><span class="sxs-lookup"><span data-stu-id="3b388-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b388-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3b388-110">Child elements</span></span>

<span data-ttu-id="3b388-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3b388-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b388-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3b388-112">Parent elements</span></span>

|<span data-ttu-id="3b388-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3b388-113">**Element**</span></span>|<span data-ttu-id="3b388-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b388-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b388-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3b388-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3b388-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="3b388-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3b388-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="3b388-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3b388-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3b388-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b388-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3b388-119">Text value</span></span>

<span data-ttu-id="3b388-120">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b388-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="3b388-121">**True**の場合は、会議の時間の新しい提案を作成することができることを示します**false**の値は、新しい日時の指定が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="3b388-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="3b388-122">開催者は、会議出席依頼でこの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="3b388-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3b388-123">備考</span><span class="sxs-lookup"><span data-stu-id="3b388-123">Remarks</span></span>

<span data-ttu-id="3b388-124">AllowNewTimeProposal プロパティは、開催者の予定表アイテムの読み取り-書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="3b388-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="3b388-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3b388-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="3b388-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3b388-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="3b388-127">Exchange Web サービスでは、新しい時間の提案のメッセージをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="3b388-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="3b388-128">新しい時間の提案のメッセージに関連するプロパティを取得するには、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="3b388-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3b388-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="3b388-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b388-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="3b388-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b388-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3b388-131">Schema name</span></span>  <br/> |<span data-ttu-id="3b388-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3b388-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b388-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3b388-133">Validation file</span></span>  <br/> |<span data-ttu-id="3b388-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b388-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b388-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3b388-135">Can be empty</span></span>  <br/> |<span data-ttu-id="3b388-136">False</span><span class="sxs-lookup"><span data-stu-id="3b388-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b388-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b388-137">See also</span></span>

- [<span data-ttu-id="3b388-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3b388-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

