---
title: MeetingRequestWasSent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestWasSent
api_type:
- schema
ms.assetid: 9192400a-8eef-4147-9f94-aa8ea91b41d8
description: MeetingRequestWasSent 要素は、要求された出席者に会議出席依頼が送信されたかどうかを示します。
ms.openlocfilehash: 0a87b1d773997e08ab96726375e4c8ce010faaf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832438"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="8312d-103">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="8312d-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="8312d-104">**MeetingRequestWasSent**要素は、要求された出席者に会議出席依頼が送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8312d-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="8312d-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8312d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8312d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8312d-106">Attributes and elements</span></span>

<span data-ttu-id="8312d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8312d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8312d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8312d-108">Attributes</span></span>

<span data-ttu-id="8312d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8312d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8312d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8312d-110">Child elements</span></span>

<span data-ttu-id="8312d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8312d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8312d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8312d-112">Parent elements</span></span>

|<span data-ttu-id="8312d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8312d-113">**Element**</span></span>|<span data-ttu-id="8312d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8312d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8312d-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="8312d-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8312d-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8312d-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8312d-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8312d-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8312d-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8312d-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8312d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8312d-119">Text value</span></span>

<span data-ttu-id="8312d-120">ブール値を表す文字列値は、この要素が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="8312d-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="8312d-121">**True**の場合は、会議出席依頼が送信されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="8312d-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="8312d-122">**False**の値は、会議出席依頼が送信されていませんを示します。</span><span class="sxs-lookup"><span data-stu-id="8312d-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8312d-123">備考</span><span class="sxs-lookup"><span data-stu-id="8312d-123">Remarks</span></span>

<span data-ttu-id="8312d-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8312d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8312d-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="8312d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8312d-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="8312d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8312d-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8312d-127">Schema name</span></span>  <br/> |<span data-ttu-id="8312d-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8312d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="8312d-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8312d-129">Validation file</span></span>  <br/> |<span data-ttu-id="8312d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8312d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8312d-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8312d-131">Can be empty</span></span>  <br/> |<span data-ttu-id="8312d-132">False</span><span class="sxs-lookup"><span data-stu-id="8312d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8312d-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="8312d-133">See also</span></span>



- [<span data-ttu-id="8312d-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8312d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

