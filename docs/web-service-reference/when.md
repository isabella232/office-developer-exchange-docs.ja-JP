---
title: 日時
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- When
api_type:
- schema
ms.assetid: c7df1333-a33d-4cc6-a08a-34b68843f47d
description: When 要素が、予定表アイテムまたは会議アイテムが発生したときに関する情報を提供します。
ms.openlocfilehash: 519712ed10958cf556c8fb29372326ade3c31c90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840028"
---
# <a name="when"></a><span data-ttu-id="09dc3-103">日時</span><span class="sxs-lookup"><span data-stu-id="09dc3-103">When</span></span>

<span data-ttu-id="09dc3-104">**When**要素では、予定または会議アイテムが発生したときに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="09dc3-104">The **When** element provides information about when a calendar or meeting item occurs.</span></span> 
  
```xml
<When/>
```

 <span data-ttu-id="09dc3-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="09dc3-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09dc3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="09dc3-106">Attributes and elements</span></span>

<span data-ttu-id="09dc3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09dc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09dc3-108">属性</span><span class="sxs-lookup"><span data-stu-id="09dc3-108">Attributes</span></span>

<span data-ttu-id="09dc3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="09dc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09dc3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="09dc3-110">Child elements</span></span>

<span data-ttu-id="09dc3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="09dc3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09dc3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="09dc3-112">Parent elements</span></span>

|<span data-ttu-id="09dc3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="09dc3-113">**Element**</span></span>|<span data-ttu-id="09dc3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="09dc3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09dc3-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="09dc3-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="09dc3-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="09dc3-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="09dc3-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="09dc3-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="09dc3-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="09dc3-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09dc3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09dc3-119">Text value</span></span>

<span data-ttu-id="09dc3-120">テキスト値は、予定表アイテムが発生した場合を説明する文字列です。</span><span class="sxs-lookup"><span data-stu-id="09dc3-120">The text value is a string that describes when a calendar item occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09dc3-121">備考</span><span class="sxs-lookup"><span data-stu-id="09dc3-121">Remarks</span></span>

<span data-ttu-id="09dc3-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="09dc3-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09dc3-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="09dc3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09dc3-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="09dc3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09dc3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09dc3-125">Schema name</span></span>  <br/> |<span data-ttu-id="09dc3-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="09dc3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="09dc3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09dc3-127">Validation file</span></span>  <br/> |<span data-ttu-id="09dc3-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09dc3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09dc3-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="09dc3-129">Can be empty</span></span>  <br/> |<span data-ttu-id="09dc3-130">False</span><span class="sxs-lookup"><span data-stu-id="09dc3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09dc3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="09dc3-131">See also</span></span>



- [<span data-ttu-id="09dc3-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="09dc3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

