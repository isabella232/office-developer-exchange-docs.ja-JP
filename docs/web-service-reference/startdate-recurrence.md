---
title: 開始日 (繰り返し)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: 開始要素では、定期的な仕事または予定表アイテムの開始日を表します。
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833551"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="8d256-103">開始日 (繰り返し)</span><span class="sxs-lookup"><span data-stu-id="8d256-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="8d256-104">**開始**要素では、定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="8d256-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="8d256-105">**日付**</span><span class="sxs-lookup"><span data-stu-id="8d256-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8d256-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d256-106">Attributes and elements</span></span>

<span data-ttu-id="8d256-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d256-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d256-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d256-108">Attributes</span></span>

<span data-ttu-id="8d256-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d256-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d256-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d256-110">Child elements</span></span>

<span data-ttu-id="8d256-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8d256-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d256-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d256-112">Parent elements</span></span>

|<span data-ttu-id="8d256-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d256-113">**Element**</span></span>|<span data-ttu-id="8d256-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d256-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d256-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d256-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="8d256-116">開始日と終了日の項目の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8d256-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8d256-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d256-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="8d256-118">定義された終了日がない項目の定期的なパターンの開始日について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d256-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="8d256-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d256-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="8d256-120">開始日と定期的なアイテムの出現回数を説明します。</span><span class="sxs-lookup"><span data-stu-id="8d256-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d256-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d256-121">Text value</span></span>

<span data-ttu-id="8d256-122">日付を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="8d256-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="8d256-123">1601、4 月、1 より小さい値を指定できません 00時 00分: 00 です。</span><span class="sxs-lookup"><span data-stu-id="8d256-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d256-124">備考</span><span class="sxs-lookup"><span data-stu-id="8d256-124">Remarks</span></span>

<span data-ttu-id="8d256-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8d256-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d256-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d256-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d256-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d256-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d256-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d256-128">Schema name</span></span>  <br/> |<span data-ttu-id="8d256-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8d256-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d256-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d256-130">Validation file</span></span>  <br/> |<span data-ttu-id="8d256-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d256-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d256-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d256-132">Can be empty</span></span>  <br/> |<span data-ttu-id="8d256-133">False</span><span class="sxs-lookup"><span data-stu-id="8d256-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d256-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d256-134">See also</span></span>

- [<span data-ttu-id="8d256-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d256-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

