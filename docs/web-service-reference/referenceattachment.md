---
title: ReferenceAttachment
ms.date: 7/7/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b9bde862-6b75-4a81-8033-00a47be4dc2f
description: ReferenceAttachment 要素は、XXX を指定します。
ms.openlocfilehash: 10f6cd1e007514300eeefaf5cc9f212cee32f516
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833029"
---
# <a name="referenceattachment"></a><span data-ttu-id="a17d4-103">ReferenceAttachment</span><span class="sxs-lookup"><span data-stu-id="a17d4-103">ReferenceAttachment</span></span>

<span data-ttu-id="a17d4-104">**ReferenceAttachment**要素は、XXX を指定します。</span><span class="sxs-lookup"><span data-stu-id="a17d4-104">The **ReferenceAttachment** element specifies XXX.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="a17d4-105">**ReferenceAttachmen**</span><span class="sxs-lookup"><span data-stu-id="a17d4-105">**ReferenceAttachmen**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a17d4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a17d4-106">Attributes and elements</span></span>

<span data-ttu-id="a17d4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a17d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a17d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="a17d4-108">Attributes</span></span>

|<span data-ttu-id="a17d4-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a17d4-109">**Attribute**</span></span>|<span data-ttu-id="a17d4-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a17d4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a17d4-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="a17d4-111">**Id**</span></span> <br/> |<span data-ttu-id="a17d4-112">**Id**属性のテキスト値は、定期的なマスター アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a17d4-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="a17d4-113">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="a17d4-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="a17d4-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="a17d4-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="a17d4-115">**変更キー**属性のテキスト値は、マスターの定期的なアイテムのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="a17d4-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="a17d4-116">これは、**文字列**値です。</span><span class="sxs-lookup"><span data-stu-id="a17d4-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a17d4-117">子要素</span><span class="sxs-lookup"><span data-stu-id="a17d4-117">Child elements</span></span>

<span data-ttu-id="a17d4-118">範囲</span><span class="sxs-lookup"><span data-stu-id="a17d4-118">Ranges</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a17d4-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a17d4-119">Parent elements</span></span>

<span data-ttu-id="a17d4-120">Itemid |GlobalItemIds |DraftItemIds |ContactIds |GroupIds</span><span class="sxs-lookup"><span data-stu-id="a17d4-120">ItemIds | GlobalItemIds | DraftItemIds| ContactIds | GroupIds</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a17d4-121">備考</span><span class="sxs-lookup"><span data-stu-id="a17d4-121">Remarks</span></span>

<span data-ttu-id="a17d4-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a17d4-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a17d4-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a17d4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a17d4-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="a17d4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a17d4-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="a17d4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a17d4-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a17d4-126">Schema name</span></span>  <br/> |<span data-ttu-id="a17d4-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a17d4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a17d4-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a17d4-128">Validation file</span></span>  <br/> |<span data-ttu-id="a17d4-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a17d4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a17d4-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a17d4-130">Can be empty</span></span>  <br/> ||
   

