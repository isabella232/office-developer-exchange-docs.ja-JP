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
description: リソース要素は、会議のスケジュール設定されたリソースを表します。
ms.openlocfilehash: 31f358414e53f55b983f7633fc9c67b0ce3ab645
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833166"
---
# <a name="resources"></a><span data-ttu-id="59ba3-103">リソース</span><span class="sxs-lookup"><span data-stu-id="59ba3-103">Resources</span></span>

<span data-ttu-id="59ba3-104">**リソース**要素は、会議のスケジュール設定されたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="59ba3-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="59ba3-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="59ba3-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59ba3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="59ba3-106">Attributes and elements</span></span>

<span data-ttu-id="59ba3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59ba3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59ba3-108">属性</span><span class="sxs-lookup"><span data-stu-id="59ba3-108">Attributes</span></span>

<span data-ttu-id="59ba3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59ba3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59ba3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59ba3-110">Child elements</span></span>

|<span data-ttu-id="59ba3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="59ba3-111">**Element**</span></span>|<span data-ttu-id="59ba3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="59ba3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59ba3-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="59ba3-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="59ba3-114">出席者および会議のためのリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="59ba3-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59ba3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="59ba3-115">Parent elements</span></span>

|<span data-ttu-id="59ba3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="59ba3-116">**Element**</span></span>|<span data-ttu-id="59ba3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="59ba3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59ba3-118">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="59ba3-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="59ba3-119">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="59ba3-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="59ba3-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="59ba3-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="59ba3-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="59ba3-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59ba3-122">備考</span><span class="sxs-lookup"><span data-stu-id="59ba3-122">Remarks</span></span>

<span data-ttu-id="59ba3-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="59ba3-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59ba3-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="59ba3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59ba3-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="59ba3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59ba3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59ba3-126">Schema name</span></span>  <br/> |<span data-ttu-id="59ba3-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="59ba3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="59ba3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59ba3-128">Validation file</span></span>  <br/> |<span data-ttu-id="59ba3-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59ba3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59ba3-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="59ba3-130">Can be empty</span></span>  <br/> |<span data-ttu-id="59ba3-131">False</span><span class="sxs-lookup"><span data-stu-id="59ba3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59ba3-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="59ba3-132">See also</span></span>



- [<span data-ttu-id="59ba3-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="59ba3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

