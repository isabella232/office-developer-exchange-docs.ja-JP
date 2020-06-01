---
title: EndDate (定期的なアイテム)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: EndDate 要素は、定期的なタスクの終了日または EndDateRecurrence パターンの種類を持つ予定表アイテムを表します。
ms.openlocfilehash: 53d9b04faf1d8f740c858080b5fcbeadf577df0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460163"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="ba538-103">EndDate (定期的なアイテム)</span><span class="sxs-lookup"><span data-stu-id="ba538-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="ba538-104">**EndDate**要素は、定期的なタスクの終了日または EndDateRecurrence パターンの種類を持つ予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ba538-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="ba538-105">**date**</span><span class="sxs-lookup"><span data-stu-id="ba538-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba538-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ba538-106">Attributes and elements</span></span>

<span data-ttu-id="ba538-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba538-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba538-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba538-108">Attributes</span></span>

<span data-ttu-id="ba538-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba538-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba538-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba538-110">Child elements</span></span>

<span data-ttu-id="ba538-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ba538-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba538-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ba538-112">Parent elements</span></span>

|<span data-ttu-id="ba538-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ba538-113">**Element**</span></span>|<span data-ttu-id="ba538-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba538-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba538-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="ba538-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="ba538-116">アイテムの定期的なパターンの開始日と終了日を示します。</span><span class="sxs-lookup"><span data-stu-id="ba538-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba538-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ba538-117">Text value</span></span>

<span data-ttu-id="ba538-118">この要素を使用する場合は、日付を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba538-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="ba538-119">この値は、00:00:00 4500 年9月1日より大きくすることはできません。</span><span class="sxs-lookup"><span data-stu-id="ba538-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba538-120">注釈</span><span class="sxs-lookup"><span data-stu-id="ba538-120">Remarks</span></span>

<span data-ttu-id="ba538-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ba538-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba538-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ba538-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba538-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba538-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba538-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba538-124">Schema name</span></span>  <br/> |<span data-ttu-id="ba538-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ba538-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba538-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba538-126">Validation file</span></span>  <br/> |<span data-ttu-id="ba538-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ba538-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba538-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ba538-128">Can be empty</span></span>  <br/> |<span data-ttu-id="ba538-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="ba538-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba538-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba538-130">See also</span></span>



- [<span data-ttu-id="ba538-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ba538-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

