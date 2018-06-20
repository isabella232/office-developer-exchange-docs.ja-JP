---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: ReturnNewItemIds 要素は、新しい項目の項目の識別子が応答で返されるかどうかを示します。
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833232"
---
# <a name="returnnewitemids"></a><span data-ttu-id="bd06d-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="bd06d-103">ReturnNewItemIds</span></span>

<span data-ttu-id="bd06d-104">**ReturnNewItemIds**要素は、新しい項目の項目の識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="bd06d-105">**xs:boolean**</span><span class="sxs-lookup"><span data-stu-id="bd06d-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd06d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bd06d-106">Attributes and elements</span></span>

<span data-ttu-id="bd06d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd06d-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd06d-108">Attributes</span></span>

<span data-ttu-id="bd06d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd06d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd06d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd06d-110">Child elements</span></span>

<span data-ttu-id="bd06d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bd06d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd06d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bd06d-112">Parent elements</span></span>

|<span data-ttu-id="bd06d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bd06d-113">**Element**</span></span>|<span data-ttu-id="bd06d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd06d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd06d-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="bd06d-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="bd06d-116">Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd06d-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="bd06d-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="bd06d-118">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd06d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bd06d-119">Text value</span></span>

<span data-ttu-id="bd06d-120">の**場合は true** 、 **ReturnNewItemIds**要素のテキスト値は、応答に新しいアイテムの識別子が返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="bd06d-121">**False**の値は、応答に新しいアイテムの識別子が返されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="bd06d-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bd06d-122">備考</span><span class="sxs-lookup"><span data-stu-id="bd06d-122">Remarks</span></span>

<span data-ttu-id="bd06d-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bd06d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd06d-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="bd06d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd06d-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="bd06d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd06d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd06d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="bd06d-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bd06d-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="bd06d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd06d-128">Validation File</span></span>  <br/> |<span data-ttu-id="bd06d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bd06d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd06d-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd06d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd06d-131">いいえ</span><span class="sxs-lookup"><span data-stu-id="bd06d-131">False</span></span>  <br/> |
   

