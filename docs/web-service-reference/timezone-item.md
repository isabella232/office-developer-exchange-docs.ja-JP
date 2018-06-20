---
title: タイムゾーン (アイテム)
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
description: タイム ゾーン要素では、タイム ゾーンの説明を提供します。
ms.openlocfilehash: e3792d136849b19c38e85e877b19bea046676fb5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839709"
---
# <a name="timezone-item"></a><span data-ttu-id="5c370-103">タイムゾーン (アイテム)</span><span class="sxs-lookup"><span data-stu-id="5c370-103">TimeZone (Item)</span></span>

<span data-ttu-id="5c370-104">**タイム ゾーン**要素では、タイム ゾーンの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5c370-104">The **TimeZone** element provides a text description of a time zone.</span></span> 
  
```xml
<TimeZone/>
```

 <span data-ttu-id="5c370-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5c370-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c370-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c370-106">Attributes and elements</span></span>

<span data-ttu-id="5c370-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c370-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c370-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c370-108">Attributes</span></span>

<span data-ttu-id="5c370-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c370-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c370-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c370-110">Child elements</span></span>

<span data-ttu-id="5c370-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5c370-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c370-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5c370-112">Parent elements</span></span>

|<span data-ttu-id="5c370-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c370-113">**Element**</span></span>|<span data-ttu-id="5c370-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c370-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c370-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="5c370-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5c370-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5c370-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c370-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5c370-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5c370-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5c370-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c370-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5c370-119">Text value</span></span>

<span data-ttu-id="5c370-120">テキスト値では、タイム ゾーンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5c370-120">The text value describes a time zone.</span></span> <span data-ttu-id="5c370-121">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5c370-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c370-122">備考</span><span class="sxs-lookup"><span data-stu-id="5c370-122">Remarks</span></span>

<span data-ttu-id="5c370-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5c370-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c370-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c370-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c370-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c370-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c370-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c370-126">Schema name</span></span>  <br/> |<span data-ttu-id="5c370-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c370-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c370-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c370-128">Validation file</span></span>  <br/> |<span data-ttu-id="5c370-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c370-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c370-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5c370-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5c370-131">False</span><span class="sxs-lookup"><span data-stu-id="5c370-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c370-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c370-132">See also</span></span>



- [<span data-ttu-id="5c370-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c370-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

