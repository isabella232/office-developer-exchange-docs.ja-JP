---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: RecurringMasterItemIdRanges 要素は、発生範囲の配列を指定します。
ms.openlocfilehash: 784676844c5c58c65b8cc6177843bf26d351b7d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528756"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="37bca-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="37bca-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="37bca-104">**RecurringMasterItemIdRanges**要素は、発生範囲の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="37bca-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="37bca-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="37bca-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37bca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="37bca-106">Attributes and elements</span></span>

<span data-ttu-id="37bca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="37bca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37bca-108">属性</span><span class="sxs-lookup"><span data-stu-id="37bca-108">Attributes</span></span>

|<span data-ttu-id="37bca-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="37bca-109">**Attribute**</span></span>|<span data-ttu-id="37bca-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="37bca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="37bca-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="37bca-111">**Id**</span></span> <br/> |<span data-ttu-id="37bca-112">**Id**属性のテキスト値は、定期的なマスターアイテムの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="37bca-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="37bca-113">これは、**文字列型 (string** ) の値です。</span><span class="sxs-lookup"><span data-stu-id="37bca-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="37bca-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="37bca-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="37bca-115">**Changekey**属性のテキスト値は、定期的なマスターアイテムの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="37bca-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="37bca-116">これは、**文字列型 (string** ) の値です。</span><span class="sxs-lookup"><span data-stu-id="37bca-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="37bca-117">子要素</span><span class="sxs-lookup"><span data-stu-id="37bca-117">Child elements</span></span>

[<span data-ttu-id="37bca-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="37bca-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="37bca-119">親要素</span><span class="sxs-lookup"><span data-stu-id="37bca-119">Parent elements</span></span>

<span data-ttu-id="37bca-120">[Itemids](itemids.md)  | [Globalitemids](globalitemids.md)  | [DraftItemIds](draftitemids.md)  | [ContactIds](contactids.md)  | [Groupids](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="37bca-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37bca-121">注釈</span><span class="sxs-lookup"><span data-stu-id="37bca-121">Remarks</span></span>

<span data-ttu-id="37bca-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="37bca-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="37bca-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="37bca-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37bca-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="37bca-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37bca-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="37bca-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37bca-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="37bca-126">Schema name</span></span>  <br/> |<span data-ttu-id="37bca-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="37bca-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="37bca-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="37bca-128">Validation file</span></span>  <br/> |<span data-ttu-id="37bca-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="37bca-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37bca-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="37bca-130">Can be empty</span></span>  <br/> ||
   

