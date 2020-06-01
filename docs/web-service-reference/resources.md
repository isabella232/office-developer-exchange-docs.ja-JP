---
title: リソース
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resources
api_type:
- schema
ms.assetid: a2133cf2-7c62-4f1c-b3aa-75f14d30dd74
description: Resources 要素は、会議のスケジュールされたリソースを表します。
ms.openlocfilehash: 67b4ed93a67a48945845887aa2d08b5bfe0102d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455591"
---
# <a name="resources"></a><span data-ttu-id="4fb62-103">リソース</span><span class="sxs-lookup"><span data-stu-id="4fb62-103">Resources</span></span>

<span data-ttu-id="4fb62-104">**Resources**要素は、会議のスケジュールされたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="4fb62-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="4fb62-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="4fb62-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fb62-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4fb62-106">Attributes and elements</span></span>

<span data-ttu-id="4fb62-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4fb62-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fb62-108">属性</span><span class="sxs-lookup"><span data-stu-id="4fb62-108">Attributes</span></span>

<span data-ttu-id="4fb62-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4fb62-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fb62-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4fb62-110">Child elements</span></span>

|<span data-ttu-id="4fb62-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4fb62-111">**Element**</span></span>|<span data-ttu-id="4fb62-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fb62-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fb62-113">出席者</span><span class="sxs-lookup"><span data-stu-id="4fb62-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="4fb62-114">会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="4fb62-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fb62-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4fb62-115">Parent elements</span></span>

|<span data-ttu-id="4fb62-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4fb62-116">**Element**</span></span>|<span data-ttu-id="4fb62-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fb62-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fb62-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4fb62-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4fb62-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4fb62-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4fb62-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4fb62-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4fb62-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="4fb62-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fb62-122">注釈</span><span class="sxs-lookup"><span data-stu-id="4fb62-122">Remarks</span></span>

<span data-ttu-id="4fb62-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4fb62-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fb62-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4fb62-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fb62-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fb62-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fb62-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4fb62-126">Schema name</span></span>  <br/> |<span data-ttu-id="4fb62-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4fb62-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fb62-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4fb62-128">Validation file</span></span>  <br/> |<span data-ttu-id="4fb62-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4fb62-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fb62-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4fb62-130">Can be empty</span></span>  <br/> |<span data-ttu-id="4fb62-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="4fb62-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fb62-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4fb62-132">See also</span></span>



- [<span data-ttu-id="4fb62-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4fb62-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

