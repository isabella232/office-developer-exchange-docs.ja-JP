---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: RecurringMasterItemId (ItemIdType) 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。
ms.openlocfilehash: c725998ad3a728ef1f47ff6491592b461753b895
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468440"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="6c6c3-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="6c6c3-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="6c6c3-104">**RecurringMasterItemId (ItemIdType)** 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="6c6c3-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="6c6c3-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c6c3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c6c3-106">Attributes and elements</span></span>

<span data-ttu-id="6c6c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c6c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c6c3-108">Attributes</span></span>

****

|<span data-ttu-id="6c6c3-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6c6c3-109">**Attribute**</span></span>|<span data-ttu-id="6c6c3-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c6c3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c6c3-111">ID</span><span class="sxs-lookup"><span data-stu-id="6c6c3-111">Id</span></span>  <br/> |<span data-ttu-id="6c6c3-112">定期的なアイテムのマスターアイテムの1つの発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6c6c3-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6c6c3-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6c6c3-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6c6c3-115">定期的なアイテムの1つのオカレンスの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6c6c3-116">また、定期的なマスターアイテムと単一のオカレンスに同じ変更キーが含まれているため、これらも確認されます。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="6c6c3-117">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6c6c3-118">子要素</span><span class="sxs-lookup"><span data-stu-id="6c6c3-118">Child elements</span></span>

<span data-ttu-id="6c6c3-119">なし。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c6c3-120">親要素</span><span class="sxs-lookup"><span data-stu-id="6c6c3-120">Parent elements</span></span>

[<span data-ttu-id="6c6c3-121">Reminder</span><span class="sxs-lookup"><span data-stu-id="6c6c3-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="6c6c3-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6c6c3-122">Remarks</span></span>

<span data-ttu-id="6c6c3-123">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6c6c3-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6c6c3-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c6c3-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c6c3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c6c3-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c6c3-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c6c3-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c6c3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6c6c3-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c6c3-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c6c3-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c6c3-129">Validation File</span></span>  <br/> |<span data-ttu-id="6c6c3-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c6c3-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c6c3-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c6c3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c6c3-132">正しい</span><span class="sxs-lookup"><span data-stu-id="6c6c3-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c6c3-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c6c3-133">See also</span></span>



[<span data-ttu-id="6c6c3-134">Reminder</span><span class="sxs-lookup"><span data-stu-id="6c6c3-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="6c6c3-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c6c3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

