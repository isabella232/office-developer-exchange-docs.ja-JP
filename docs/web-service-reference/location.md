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
ms.openlocfilehash: 0d2bc131763c4ffa399fe9397d247d89a84e0d1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832241"
---
# <a name="location"></a><span data-ttu-id="f9a8c-103">場所</span><span class="sxs-lookup"><span data-stu-id="f9a8c-103">Location</span></span>

<span data-ttu-id="f9a8c-104">**Location**要素は、会議、予定、またはペルソナの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-104">The **Location** element represents the location of a meeting, appointment, or persona.</span></span> 
  
```xml
<Location/>
```

 <span data-ttu-id="f9a8c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="f9a8c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9a8c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f9a8c-106">Attributes and elements</span></span>

<span data-ttu-id="f9a8c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9a8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9a8c-108">Attributes</span></span>

<span data-ttu-id="f9a8c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9a8c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f9a8c-110">Child elements</span></span>

<span data-ttu-id="f9a8c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9a8c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f9a8c-112">Parent elements</span></span>

|<span data-ttu-id="f9a8c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f9a8c-113">**Element**</span></span>|<span data-ttu-id="f9a8c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9a8c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9a8c-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="f9a8c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f9a8c-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f9a8c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f9a8c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f9a8c-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f9a8c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f9a8c-119">Text value</span></span>

<span data-ttu-id="f9a8c-120">会議または予定の場所を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-120">A text value that represents the location of a meeting or appointment is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f9a8c-121">備考</span><span class="sxs-lookup"><span data-stu-id="f9a8c-121">Remarks</span></span>

<span data-ttu-id="f9a8c-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9a8c-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="f9a8c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9a8c-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="f9a8c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9a8c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9a8c-125">Schema name</span></span>  <br/> |<span data-ttu-id="f9a8c-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f9a8c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9a8c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9a8c-127">Validation file</span></span>  <br/> |<span data-ttu-id="f9a8c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9a8c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9a8c-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f9a8c-129">Can be empty</span></span>  <br/> |<span data-ttu-id="f9a8c-130">False</span><span class="sxs-lookup"><span data-stu-id="f9a8c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9a8c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9a8c-131">See also</span></span>



- [<span data-ttu-id="f9a8c-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f9a8c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

