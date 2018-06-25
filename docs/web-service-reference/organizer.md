---
title: Organizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Organizer
api_type:
- schema
ms.assetid: 63892b57-3805-4d60-b9f7-20552a69c241
description: 開催者の要素は、会議の開催者を表します。
ms.openlocfilehash: b723578a1b52cd5f6e9bd869a15430453adfa291
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832662"
---
# <a name="organizer"></a><span data-ttu-id="ac38c-103">Organizer</span><span class="sxs-lookup"><span data-stu-id="ac38c-103">Organizer</span></span>

<span data-ttu-id="ac38c-104">**開催者**の要素は、会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="ac38c-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="ac38c-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="ac38c-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ac38c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ac38c-106">Attributes and elements</span></span>

<span data-ttu-id="ac38c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac38c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac38c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac38c-108">Attributes</span></span>

<span data-ttu-id="ac38c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ac38c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac38c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ac38c-110">Child elements</span></span>

|<span data-ttu-id="ac38c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac38c-111">**Element**</span></span>|<span data-ttu-id="ac38c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac38c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac38c-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="ac38c-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ac38c-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="ac38c-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac38c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ac38c-115">Parent elements</span></span>

|<span data-ttu-id="ac38c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac38c-116">**Element**</span></span>|<span data-ttu-id="ac38c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac38c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac38c-118">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="ac38c-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ac38c-119">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ac38c-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ac38c-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ac38c-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ac38c-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="ac38c-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ac38c-122">備考</span><span class="sxs-lookup"><span data-stu-id="ac38c-122">Remarks</span></span>

<span data-ttu-id="ac38c-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ac38c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac38c-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="ac38c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac38c-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="ac38c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac38c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac38c-126">Schema name</span></span>  <br/> |<span data-ttu-id="ac38c-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ac38c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac38c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac38c-128">Validation file</span></span>  <br/> |<span data-ttu-id="ac38c-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ac38c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac38c-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ac38c-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ac38c-131">False</span><span class="sxs-lookup"><span data-stu-id="ac38c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac38c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac38c-132">See also</span></span>

- [<span data-ttu-id="ac38c-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ac38c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

