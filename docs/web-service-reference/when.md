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
description: When 要素は、予定表または会議アイテムがいつ発生したかに関する情報を提供します。
ms.openlocfilehash: 7c5f85184f966d909960bf1d79f5b8d33c67b51a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461857"
---
# <a name="when"></a><span data-ttu-id="604a4-103">日時</span><span class="sxs-lookup"><span data-stu-id="604a4-103">When</span></span>

<span data-ttu-id="604a4-104">**When**要素は、予定表または会議アイテムがいつ発生したかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="604a4-104">The **When** element provides information about when a calendar or meeting item occurs.</span></span> 
  
```xml
<When/>
```

 <span data-ttu-id="604a4-105">**String**</span><span class="sxs-lookup"><span data-stu-id="604a4-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="604a4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="604a4-106">Attributes and elements</span></span>

<span data-ttu-id="604a4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="604a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="604a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="604a4-108">Attributes</span></span>

<span data-ttu-id="604a4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="604a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="604a4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="604a4-110">Child elements</span></span>

<span data-ttu-id="604a4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="604a4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="604a4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="604a4-112">Parent elements</span></span>

|<span data-ttu-id="604a4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="604a4-113">**Element**</span></span>|<span data-ttu-id="604a4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="604a4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="604a4-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="604a4-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="604a4-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="604a4-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="604a4-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="604a4-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="604a4-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="604a4-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="604a4-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="604a4-119">Text value</span></span>

<span data-ttu-id="604a4-120">テキスト値は、予定表アイテムがいつ発生したかを示す文字列です。</span><span class="sxs-lookup"><span data-stu-id="604a4-120">The text value is a string that describes when a calendar item occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="604a4-121">注釈</span><span class="sxs-lookup"><span data-stu-id="604a4-121">Remarks</span></span>

<span data-ttu-id="604a4-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="604a4-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="604a4-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="604a4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="604a4-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="604a4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="604a4-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="604a4-125">Schema name</span></span>  <br/> |<span data-ttu-id="604a4-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="604a4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="604a4-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="604a4-127">Validation file</span></span>  <br/> |<span data-ttu-id="604a4-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="604a4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="604a4-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="604a4-129">Can be empty</span></span>  <br/> |<span data-ttu-id="604a4-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="604a4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="604a4-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="604a4-131">See also</span></span>



- [<span data-ttu-id="604a4-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="604a4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

