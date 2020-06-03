---
title: 範囲
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Range 要素は、定期的な予定表アイテムの予定表アイテムの出現範囲を指定します。
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465311"
---
# <a name="range"></a><span data-ttu-id="72059-103">範囲</span><span class="sxs-lookup"><span data-stu-id="72059-103">Range</span></span>

<span data-ttu-id="72059-104">**Range**要素は、定期的な予定表アイテムの予定表アイテムの出現範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="72059-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="72059-105">**OccurrencesRangeType**</span><span class="sxs-lookup"><span data-stu-id="72059-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72059-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="72059-106">Attributes and elements</span></span>

<span data-ttu-id="72059-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72059-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72059-108">属性</span><span class="sxs-lookup"><span data-stu-id="72059-108">Attributes</span></span>

|<span data-ttu-id="72059-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="72059-109">**Attribute**</span></span>|<span data-ttu-id="72059-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="72059-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="72059-111">**Start**</span><span class="sxs-lookup"><span data-stu-id="72059-111">**Start**</span></span> <br/> |<span data-ttu-id="72059-112">**Start**属性のテキスト値は、定期的なアイテムの範囲の開始日です。</span><span class="sxs-lookup"><span data-stu-id="72059-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="72059-113">これは**dateTime**値です。</span><span class="sxs-lookup"><span data-stu-id="72059-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="72059-114">**End**</span><span class="sxs-lookup"><span data-stu-id="72059-114">**End**</span></span> <br/> |<span data-ttu-id="72059-115">**End**属性のテキスト値は、定期的なアイテムの範囲の終了日です。</span><span class="sxs-lookup"><span data-stu-id="72059-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="72059-116">これは**dateTime**値です。</span><span class="sxs-lookup"><span data-stu-id="72059-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="72059-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="72059-117">**Count**</span></span> <br/> |<span data-ttu-id="72059-118">**Count**属性のテキスト値は、定期的なアイテムの出現回数です。</span><span class="sxs-lookup"><span data-stu-id="72059-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="72059-119">これは**整数**値です。</span><span class="sxs-lookup"><span data-stu-id="72059-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="72059-120">**CompareOriginalStartTime**</span><span class="sxs-lookup"><span data-stu-id="72059-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="72059-121">**Compareoriginalstarttime**属性のテキスト値が**true**になっている場合は、クライアントが元の開始時刻を新しい開始時刻と比較する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="72059-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="72059-122">値が**false**の場合は、クライアントが元の開始時刻と新しい開始時刻を比較する必要がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="72059-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="72059-123">子要素</span><span class="sxs-lookup"><span data-stu-id="72059-123">Child elements</span></span>

<span data-ttu-id="72059-124">なし。</span><span class="sxs-lookup"><span data-stu-id="72059-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72059-125">親要素</span><span class="sxs-lookup"><span data-stu-id="72059-125">Parent elements</span></span>

[<span data-ttu-id="72059-126">Ranges</span><span class="sxs-lookup"><span data-stu-id="72059-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="72059-127">注釈</span><span class="sxs-lookup"><span data-stu-id="72059-127">Remarks</span></span>

<span data-ttu-id="72059-128">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="72059-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="72059-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="72059-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72059-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="72059-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72059-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="72059-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72059-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72059-132">Schema name</span></span>  <br/> |<span data-ttu-id="72059-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="72059-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="72059-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72059-134">Validation file</span></span>  <br/> |<span data-ttu-id="72059-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="72059-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72059-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="72059-136">Can be empty</span></span>  <br/> ||
   

