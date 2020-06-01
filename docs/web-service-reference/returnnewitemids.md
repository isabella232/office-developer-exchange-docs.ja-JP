---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: ReturnNewItemIds 要素は、新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。
ms.openlocfilehash: 003676c4c034454aa551e42bf3af976183117b8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465115"
---
# <a name="returnnewitemids"></a><span data-ttu-id="6d42e-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="6d42e-103">ReturnNewItemIds</span></span>

<span data-ttu-id="6d42e-104">**Returnnewitemids**要素は、新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="6d42e-105">**xs: boolean**</span><span class="sxs-lookup"><span data-stu-id="6d42e-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d42e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6d42e-106">Attributes and elements</span></span>

<span data-ttu-id="6d42e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d42e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d42e-108">Attributes</span></span>

<span data-ttu-id="6d42e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d42e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d42e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d42e-110">Child elements</span></span>

<span data-ttu-id="6d42e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6d42e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d42e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6d42e-112">Parent elements</span></span>

|<span data-ttu-id="6d42e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d42e-113">**Element**</span></span>|<span data-ttu-id="6d42e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d42e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d42e-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="6d42e-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="6d42e-116">Exchange ストア内のメールボックス内のアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d42e-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="6d42e-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="6d42e-118">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d42e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6d42e-119">Text value</span></span>

<span data-ttu-id="6d42e-120">**Returnnewitemids**要素のテキスト値が**true の場合**は、新しいアイテムの識別子が応答で返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="6d42e-121">値が**false**の場合、新しいアイテムの識別子が応答で返されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6d42e-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6d42e-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6d42e-122">Remarks</span></span>

<span data-ttu-id="6d42e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6d42e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d42e-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6d42e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d42e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d42e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d42e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d42e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6d42e-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6d42e-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="6d42e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d42e-128">Validation File</span></span>  <br/> |<span data-ttu-id="6d42e-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6d42e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d42e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d42e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d42e-131">いいえ</span><span class="sxs-lookup"><span data-stu-id="6d42e-131">False</span></span>  <br/> |
   

