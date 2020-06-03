---
title: 期間 (アイテム)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: c6a9bafd-a15b-4b04-8070-6e0a693f9683
description: Duration 要素は、予定表アイテムの期間を表します。
ms.openlocfilehash: 2434ae081fcdd0fa06f0ffbc016537691132a4cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463553"
---
# <a name="duration-items"></a><span data-ttu-id="d473c-103">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="d473c-103">Duration (Items)</span></span>

<span data-ttu-id="d473c-104">**Duration**要素は、予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="d473c-104">The **Duration** element represents the duration of a calendar item.</span></span> 
  
```xml
<Duration/>
```

 <span data-ttu-id="d473c-105">**String**</span><span class="sxs-lookup"><span data-stu-id="d473c-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d473c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d473c-106">Attributes and elements</span></span>

<span data-ttu-id="d473c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d473c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d473c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d473c-108">Attributes</span></span>

<span data-ttu-id="d473c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d473c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d473c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d473c-110">Child elements</span></span>

<span data-ttu-id="d473c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d473c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d473c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d473c-112">Parent elements</span></span>

|<span data-ttu-id="d473c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d473c-113">**Element**</span></span>|<span data-ttu-id="d473c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d473c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d473c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d473c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d473c-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d473c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d473c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d473c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d473c-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d473c-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d473c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d473c-119">Text value</span></span>

<span data-ttu-id="d473c-120">テキスト値は、予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="d473c-120">The text value represents the duration of a calendar item.</span></span> <span data-ttu-id="d473c-121">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d473c-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d473c-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d473c-122">Remarks</span></span>

<span data-ttu-id="d473c-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="d473c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d473c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d473c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d473c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d473c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d473c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d473c-126">Schema name</span></span>  <br/> |<span data-ttu-id="d473c-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d473c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d473c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d473c-128">Validation file</span></span>  <br/> |<span data-ttu-id="d473c-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d473c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d473c-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d473c-130">Can be empty</span></span>  <br/> |<span data-ttu-id="d473c-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="d473c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d473c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d473c-132">See also</span></span>

- [<span data-ttu-id="d473c-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d473c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

