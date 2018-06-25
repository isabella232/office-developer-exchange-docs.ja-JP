---
title: IsCancelled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: IsCancelled 要素では、予定または会議がキャンセルされたかどうかを示します。
ms.openlocfilehash: 594b8a9ccb535f074a8cf1da060373f640231a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831993"
---
# <a name="iscancelled"></a><span data-ttu-id="c41d9-103">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="c41d9-103">IsCancelled</span></span>

<span data-ttu-id="c41d9-104">**IsCancelled**要素では、予定または会議がキャンセルされたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="c41d9-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c41d9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c41d9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c41d9-106">Attributes and elements</span></span>

<span data-ttu-id="c41d9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c41d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="c41d9-108">Attributes</span></span>

<span data-ttu-id="c41d9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c41d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c41d9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c41d9-110">Child elements</span></span>

<span data-ttu-id="c41d9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c41d9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c41d9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c41d9-112">Parent elements</span></span>

|<span data-ttu-id="c41d9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c41d9-113">**Element**</span></span>|<span data-ttu-id="c41d9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c41d9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c41d9-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c41d9-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c41d9-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c41d9-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c41d9-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c41d9-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c41d9-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c41d9-119">Text value</span></span>

<span data-ttu-id="c41d9-120">ブール値を表す文字列値は、この要素が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="c41d9-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="c41d9-121">**True**の場合は、予定表アイテムがキャンセルされたことを示します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="c41d9-122">**False**の値は、予定表アイテムがキャンセルされなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="c41d9-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c41d9-123">備考</span><span class="sxs-lookup"><span data-stu-id="c41d9-123">Remarks</span></span>

<span data-ttu-id="c41d9-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c41d9-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c41d9-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="c41d9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c41d9-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="c41d9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c41d9-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c41d9-127">Schema name</span></span>  <br/> |<span data-ttu-id="c41d9-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c41d9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c41d9-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c41d9-129">Validation file</span></span>  <br/> |<span data-ttu-id="c41d9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c41d9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c41d9-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c41d9-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c41d9-132">False</span><span class="sxs-lookup"><span data-stu-id="c41d9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c41d9-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="c41d9-133">See also</span></span>



- [<span data-ttu-id="c41d9-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c41d9-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

