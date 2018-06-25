---
title: Range
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: 範囲の要素は、繰り返しの予定表アイテムの予定表アイテムの出現回数の範囲を指定します。
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832946"
---
# <a name="range"></a><span data-ttu-id="ee4a6-103">Range</span><span class="sxs-lookup"><span data-stu-id="ee4a6-103">Range</span></span>

<span data-ttu-id="ee4a6-104">**範囲**の要素は、繰り返しの予定表アイテムの予定表アイテムの出現回数の範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="ee4a6-105">**OccurrencesRangeType**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee4a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ee4a6-106">Attributes and elements</span></span>

<span data-ttu-id="ee4a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee4a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee4a6-108">Attributes</span></span>

|<span data-ttu-id="ee4a6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-109">**Attribute**</span></span>|<span data-ttu-id="ee4a6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee4a6-111">**Start**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-111">**Start**</span></span> <br/> |<span data-ttu-id="ee4a6-112">**開始**属性のテキスト値は、定期的なアイテムの範囲の開始日です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="ee4a6-113">これは、 **dateTime**値です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="ee4a6-114">**End**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-114">**End**</span></span> <br/> |<span data-ttu-id="ee4a6-115">**最終**属性のテキスト値は、定期的なアイテムの範囲の終了日です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="ee4a6-116">これは、 **dateTime**値です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="ee4a6-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-117">**Count**</span></span> <br/> |<span data-ttu-id="ee4a6-118">**数**の属性のテキスト値は、定期的なアイテムの数です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="ee4a6-119">これは、**整数**値です。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="ee4a6-120">**CompareOriginalStartTime**</span><span class="sxs-lookup"><span data-stu-id="ee4a6-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="ee4a6-121">**True**の**CompareOriginalStartTime**属性のテキスト値は、クライアントが新しい開始時刻を元の開始時刻を比較する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="ee4a6-122">**False**の値は、クライアントが新しい開始時刻を元の開始時刻を比較する必要がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ee4a6-123">子要素</span><span class="sxs-lookup"><span data-stu-id="ee4a6-123">Child elements</span></span>

<span data-ttu-id="ee4a6-124">なし。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee4a6-125">親要素</span><span class="sxs-lookup"><span data-stu-id="ee4a6-125">Parent elements</span></span>

[<span data-ttu-id="ee4a6-126">Ranges</span><span class="sxs-lookup"><span data-stu-id="ee4a6-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="ee4a6-127">備考</span><span class="sxs-lookup"><span data-stu-id="ee4a6-127">Remarks</span></span>

<span data-ttu-id="ee4a6-128">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ee4a6-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee4a6-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="ee4a6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee4a6-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="ee4a6-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee4a6-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ee4a6-132">Schema name</span></span>  <br/> |<span data-ttu-id="ee4a6-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ee4a6-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee4a6-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ee4a6-134">Validation file</span></span>  <br/> |<span data-ttu-id="ee4a6-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ee4a6-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee4a6-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-136">Can be empty</span></span>  <br/> ||
   

