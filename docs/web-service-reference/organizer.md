---
title: 開催者
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
description: 開催者要素は、会議の開催者を表します。
ms.openlocfilehash: c1188c9b3a894e86a08b8869045c3647e394f506
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462417"
---
# <a name="organizer"></a><span data-ttu-id="756ee-103">開催者</span><span class="sxs-lookup"><span data-stu-id="756ee-103">Organizer</span></span>

<span data-ttu-id="756ee-104">**開催者**要素は、会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="756ee-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="756ee-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="756ee-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="756ee-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="756ee-106">Attributes and elements</span></span>

<span data-ttu-id="756ee-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="756ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="756ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="756ee-108">Attributes</span></span>

<span data-ttu-id="756ee-109">なし。</span><span class="sxs-lookup"><span data-stu-id="756ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="756ee-110">子要素</span><span class="sxs-lookup"><span data-stu-id="756ee-110">Child elements</span></span>

|<span data-ttu-id="756ee-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="756ee-111">**Element**</span></span>|<span data-ttu-id="756ee-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="756ee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="756ee-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="756ee-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="756ee-114">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="756ee-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="756ee-115">親要素</span><span class="sxs-lookup"><span data-stu-id="756ee-115">Parent elements</span></span>

|<span data-ttu-id="756ee-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="756ee-116">**Element**</span></span>|<span data-ttu-id="756ee-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="756ee-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="756ee-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="756ee-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="756ee-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="756ee-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="756ee-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="756ee-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="756ee-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="756ee-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="756ee-122">注釈</span><span class="sxs-lookup"><span data-stu-id="756ee-122">Remarks</span></span>

<span data-ttu-id="756ee-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="756ee-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="756ee-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="756ee-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="756ee-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="756ee-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="756ee-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="756ee-126">Schema name</span></span>  <br/> |<span data-ttu-id="756ee-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="756ee-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="756ee-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="756ee-128">Validation file</span></span>  <br/> |<span data-ttu-id="756ee-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="756ee-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="756ee-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="756ee-130">Can be empty</span></span>  <br/> |<span data-ttu-id="756ee-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="756ee-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="756ee-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="756ee-132">See also</span></span>

- [<span data-ttu-id="756ee-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="756ee-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

