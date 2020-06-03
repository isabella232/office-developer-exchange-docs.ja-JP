---
title: TimeZone (Item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: aa49074a-50ca-4959-bee2-6ab90ef2f26e
description: TimeZone 要素は、タイムゾーンのテキストの説明を提供します。
ms.openlocfilehash: ba5b006804c66b32781d3e48d88e95ab36c09617
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465143"
---
# <a name="timezone-item"></a><span data-ttu-id="54f16-103">TimeZone (Item)</span><span class="sxs-lookup"><span data-stu-id="54f16-103">TimeZone (Item)</span></span>

<span data-ttu-id="54f16-104">**TimeZone**要素は、タイムゾーンのテキストの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="54f16-104">The **TimeZone** element provides a text description of a time zone.</span></span> 
  
```xml
<TimeZone/>
```

 <span data-ttu-id="54f16-105">**string**</span><span class="sxs-lookup"><span data-stu-id="54f16-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f16-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="54f16-106">Attributes and elements</span></span>

<span data-ttu-id="54f16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54f16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f16-108">属性</span><span class="sxs-lookup"><span data-stu-id="54f16-108">Attributes</span></span>

<span data-ttu-id="54f16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="54f16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54f16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="54f16-110">Child elements</span></span>

<span data-ttu-id="54f16-111">なし。</span><span class="sxs-lookup"><span data-stu-id="54f16-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54f16-112">親要素</span><span class="sxs-lookup"><span data-stu-id="54f16-112">Parent elements</span></span>

|<span data-ttu-id="54f16-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="54f16-113">**Element**</span></span>|<span data-ttu-id="54f16-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="54f16-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f16-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="54f16-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="54f16-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="54f16-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="54f16-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="54f16-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="54f16-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="54f16-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54f16-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="54f16-119">Text value</span></span>

<span data-ttu-id="54f16-120">テキスト値は、タイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="54f16-120">The text value describes a time zone.</span></span> <span data-ttu-id="54f16-121">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="54f16-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54f16-122">注釈</span><span class="sxs-lookup"><span data-stu-id="54f16-122">Remarks</span></span>

<span data-ttu-id="54f16-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="54f16-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f16-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="54f16-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f16-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="54f16-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54f16-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54f16-126">Schema name</span></span>  <br/> |<span data-ttu-id="54f16-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="54f16-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="54f16-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54f16-128">Validation file</span></span>  <br/> |<span data-ttu-id="54f16-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="54f16-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54f16-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="54f16-130">Can be empty</span></span>  <br/> |<span data-ttu-id="54f16-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="54f16-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54f16-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="54f16-132">See also</span></span>



- [<span data-ttu-id="54f16-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="54f16-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

