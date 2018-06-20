---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: RecurringMasterItemId (ItemIdType) の要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833010"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="fd5aa-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="fd5aa-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="fd5aa-104">**RecurringMasterItemId (ItemIdType)** の要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="fd5aa-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="fd5aa-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd5aa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fd5aa-106">Attributes and elements</span></span>

<span data-ttu-id="fd5aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd5aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd5aa-108">Attributes</span></span>

****

|<span data-ttu-id="fd5aa-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fd5aa-109">**Attribute**</span></span>|<span data-ttu-id="fd5aa-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd5aa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd5aa-111">ID</span><span class="sxs-lookup"><span data-stu-id="fd5aa-111">Id</span></span>  <br/> |<span data-ttu-id="fd5aa-112">マスターの定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="fd5aa-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fd5aa-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="fd5aa-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="fd5aa-115">マスターの定期的なアイテムの 1 回の特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="fd5aa-116">さらに、定期的なマスター アイテムは、1 回の会議と同じキーの変更が格納されるためにも識別されます。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="fd5aa-117">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fd5aa-118">子要素</span><span class="sxs-lookup"><span data-stu-id="fd5aa-118">Child elements</span></span>

<span data-ttu-id="fd5aa-119">なし。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd5aa-120">親要素</span><span class="sxs-lookup"><span data-stu-id="fd5aa-120">Parent elements</span></span>

[<span data-ttu-id="fd5aa-121">Reminder</span><span class="sxs-lookup"><span data-stu-id="fd5aa-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="fd5aa-122">備考</span><span class="sxs-lookup"><span data-stu-id="fd5aa-122">Remarks</span></span>

<span data-ttu-id="fd5aa-123">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="fd5aa-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fd5aa-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd5aa-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="fd5aa-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd5aa-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="fd5aa-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd5aa-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd5aa-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fd5aa-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fd5aa-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd5aa-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd5aa-129">Validation File</span></span>  <br/> |<span data-ttu-id="fd5aa-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd5aa-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd5aa-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd5aa-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd5aa-132">True</span><span class="sxs-lookup"><span data-stu-id="fd5aa-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd5aa-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd5aa-133">See also</span></span>



[<span data-ttu-id="fd5aa-134">Reminder</span><span class="sxs-lookup"><span data-stu-id="fd5aa-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="fd5aa-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fd5aa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

