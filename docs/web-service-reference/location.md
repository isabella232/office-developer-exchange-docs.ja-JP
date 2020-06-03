---
title: Location
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 3fcf7133-ae1c-47b4-a187-660045f71df0
description: Location 要素は、会議、予定、またはペルソナの場所を表します。
ms.openlocfilehash: 0063d5da23eb731835599f3e931e3c0cb2843ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458090"
---
# <a name="location"></a><span data-ttu-id="0ac23-103">場所</span><span class="sxs-lookup"><span data-stu-id="0ac23-103">Location</span></span>

<span data-ttu-id="0ac23-104">**Location**要素は、会議、予定、またはペルソナの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="0ac23-104">The **Location** element represents the location of a meeting, appointment, or persona.</span></span> 
  
```xml
<Location/>
```

 <span data-ttu-id="0ac23-105">**string**</span><span class="sxs-lookup"><span data-stu-id="0ac23-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ac23-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0ac23-106">Attributes and elements</span></span>

<span data-ttu-id="0ac23-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0ac23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ac23-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ac23-108">Attributes</span></span>

<span data-ttu-id="0ac23-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0ac23-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ac23-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0ac23-110">Child elements</span></span>

<span data-ttu-id="0ac23-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0ac23-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ac23-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0ac23-112">Parent elements</span></span>

|<span data-ttu-id="0ac23-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ac23-113">**Element**</span></span>|<span data-ttu-id="0ac23-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ac23-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ac23-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0ac23-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0ac23-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0ac23-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0ac23-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0ac23-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0ac23-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="0ac23-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ac23-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0ac23-119">Text value</span></span>

<span data-ttu-id="0ac23-120">会議または予定の場所を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ac23-120">A text value that represents the location of a meeting or appointment is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ac23-121">注釈</span><span class="sxs-lookup"><span data-stu-id="0ac23-121">Remarks</span></span>

<span data-ttu-id="0ac23-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0ac23-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ac23-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0ac23-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ac23-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ac23-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ac23-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0ac23-125">Schema name</span></span>  <br/> |<span data-ttu-id="0ac23-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0ac23-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ac23-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0ac23-127">Validation file</span></span>  <br/> |<span data-ttu-id="0ac23-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0ac23-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ac23-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0ac23-129">Can be empty</span></span>  <br/> |<span data-ttu-id="0ac23-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="0ac23-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ac23-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ac23-131">See also</span></span>



- [<span data-ttu-id="0ac23-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0ac23-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

