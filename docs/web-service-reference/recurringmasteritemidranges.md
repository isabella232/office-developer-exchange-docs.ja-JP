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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833016"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="7e9cc-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="7e9cc-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="7e9cc-104">**RecurringMasterItemIdRanges**要素は、出現範囲の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="7e9cc-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="7e9cc-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e9cc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e9cc-106">Attributes and elements</span></span>

<span data-ttu-id="7e9cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e9cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e9cc-108">Attributes</span></span>

|<span data-ttu-id="7e9cc-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7e9cc-109">**Attribute**</span></span>|<span data-ttu-id="7e9cc-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e9cc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e9cc-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="7e9cc-111">**Id**</span></span> <br/> |<span data-ttu-id="7e9cc-112">**Id**属性のテキスト値は、定期的なマスター アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="7e9cc-113">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="7e9cc-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="7e9cc-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="7e9cc-115">**変更キー**属性のテキスト値は、マスターの定期的なアイテムのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="7e9cc-116">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e9cc-117">子要素</span><span class="sxs-lookup"><span data-stu-id="7e9cc-117">Child elements</span></span>

[<span data-ttu-id="7e9cc-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="7e9cc-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="7e9cc-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7e9cc-119">Parent elements</span></span>

<span data-ttu-id="7e9cc-120">[Itemid](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="7e9cc-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e9cc-121">備考</span><span class="sxs-lookup"><span data-stu-id="7e9cc-121">Remarks</span></span>

<span data-ttu-id="7e9cc-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e9cc-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e9cc-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e9cc-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e9cc-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e9cc-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e9cc-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e9cc-126">Schema name</span></span>  <br/> |<span data-ttu-id="7e9cc-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e9cc-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e9cc-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e9cc-128">Validation file</span></span>  <br/> |<span data-ttu-id="7e9cc-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e9cc-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e9cc-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e9cc-130">Can be empty</span></span>  <br/> ||
   

