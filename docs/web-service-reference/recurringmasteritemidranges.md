---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: RecurringMasterItemIdRanges 要素は、出現範囲の配列を指定します。
ms.openlocfilehash: 60d987f475bed5d630a1238550e4d14578ebd0d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833016"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="65e2d-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="65e2d-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="65e2d-104">**RecurringMasterItemIdRanges**要素は、出現範囲の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="65e2d-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="65e2d-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="65e2d-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65e2d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="65e2d-106">Attributes and elements</span></span>

<span data-ttu-id="65e2d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="65e2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65e2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="65e2d-108">Attributes</span></span>

|<span data-ttu-id="65e2d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="65e2d-109">**Attribute**</span></span>|<span data-ttu-id="65e2d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="65e2d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65e2d-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="65e2d-111">**Id**</span></span> <br/> |<span data-ttu-id="65e2d-112">**Id**属性のテキスト値は、定期的なマスター アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="65e2d-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="65e2d-113">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="65e2d-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="65e2d-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="65e2d-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="65e2d-115">**変更キー**属性のテキスト値は、マスターの定期的なアイテムのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="65e2d-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="65e2d-116">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="65e2d-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="65e2d-117">子要素</span><span class="sxs-lookup"><span data-stu-id="65e2d-117">Child elements</span></span>

[<span data-ttu-id="65e2d-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="65e2d-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="65e2d-119">親要素</span><span class="sxs-lookup"><span data-stu-id="65e2d-119">Parent elements</span></span>

<span data-ttu-id="65e2d-120">[Itemid](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="65e2d-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65e2d-121">備考</span><span class="sxs-lookup"><span data-stu-id="65e2d-121">Remarks</span></span>

<span data-ttu-id="65e2d-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="65e2d-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="65e2d-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="65e2d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65e2d-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="65e2d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65e2d-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="65e2d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65e2d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="65e2d-126">Schema name</span></span>  <br/> |<span data-ttu-id="65e2d-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="65e2d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="65e2d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="65e2d-128">Validation file</span></span>  <br/> |<span data-ttu-id="65e2d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65e2d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65e2d-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="65e2d-130">Can be empty</span></span>  <br/> ||
   

