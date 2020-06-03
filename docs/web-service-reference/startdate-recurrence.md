---
title: StartDate (定期的な予定)
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
description: StartDate 要素は、定期的な仕事または予定表アイテムの開始日を表します。
ms.openlocfilehash: 4514f126b1de31c64a2650b9e7cb6b7412a726c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457208"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="9f7bd-103">StartDate (定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="9f7bd-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="9f7bd-104">**StartDate**要素は、定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="9f7bd-105">**Date**</span><span class="sxs-lookup"><span data-stu-id="9f7bd-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f7bd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f7bd-106">Attributes and elements</span></span>

<span data-ttu-id="9f7bd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f7bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f7bd-108">Attributes</span></span>

<span data-ttu-id="9f7bd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f7bd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f7bd-110">Child elements</span></span>

<span data-ttu-id="9f7bd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f7bd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9f7bd-112">Parent elements</span></span>

|<span data-ttu-id="9f7bd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f7bd-113">**Element**</span></span>|<span data-ttu-id="9f7bd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f7bd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f7bd-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9f7bd-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="9f7bd-116">アイテムの定期的なパターンの開始日と終了日を示します。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="9f7bd-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="9f7bd-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="9f7bd-118">定義済みの終了日を持たないアイテムの定期的なパターンの開始日を示します。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="9f7bd-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9f7bd-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="9f7bd-120">定期的なアイテムの開始日と発生回数を表します。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9f7bd-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9f7bd-121">Text value</span></span>

<span data-ttu-id="9f7bd-122">この要素を使用する場合は、日付を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="9f7bd-123">この値は、Apr、1、1601 00:00:00 より小さくすることはできません。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f7bd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="9f7bd-124">Remarks</span></span>

<span data-ttu-id="9f7bd-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f7bd-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f7bd-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f7bd-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f7bd-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f7bd-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f7bd-128">Schema name</span></span>  <br/> |<span data-ttu-id="9f7bd-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f7bd-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f7bd-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f7bd-130">Validation file</span></span>  <br/> |<span data-ttu-id="9f7bd-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9f7bd-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f7bd-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f7bd-132">Can be empty</span></span>  <br/> |<span data-ttu-id="9f7bd-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="9f7bd-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f7bd-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f7bd-134">See also</span></span>

- [<span data-ttu-id="9f7bd-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f7bd-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

