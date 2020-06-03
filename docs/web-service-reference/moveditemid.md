---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: MovedItemId 要素は、MarkAsJunk 操作によって移動されたアイテムの id を指定します。
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468615"
---
# <a name="moveditemid"></a><span data-ttu-id="54f2c-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="54f2c-103">MovedItemId</span></span>

<span data-ttu-id="54f2c-104">**Moveditemid**要素は、 **markasjunk**操作によって移動されたアイテムの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="54f2c-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="54f2c-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="54f2c-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f2c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="54f2c-106">Attributes and elements</span></span>

<span data-ttu-id="54f2c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54f2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="54f2c-108">Attributes</span></span>

|<span data-ttu-id="54f2c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="54f2c-109">**Attribute**</span></span>|<span data-ttu-id="54f2c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="54f2c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54f2c-111">ID</span><span class="sxs-lookup"><span data-stu-id="54f2c-111">Id</span></span>  <br/> |<span data-ttu-id="54f2c-112">**Id**属性の値は、 **markasjunk**操作によって移動されるアイテムのアイテム識別子です。</span><span class="sxs-lookup"><span data-stu-id="54f2c-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="54f2c-113">移動後も、アイテムの識別子は変わりません。</span><span class="sxs-lookup"><span data-stu-id="54f2c-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="54f2c-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="54f2c-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="54f2c-115">**Changekey**属性の値は、移動されたアイテムの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="54f2c-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="54f2c-116">**Markasjunk**操作によってアイテムが移動された後に、change キーが変更されます。</span><span class="sxs-lookup"><span data-stu-id="54f2c-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="54f2c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="54f2c-117">Child elements</span></span>

<span data-ttu-id="54f2c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="54f2c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54f2c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="54f2c-119">Parent elements</span></span>

[<span data-ttu-id="54f2c-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54f2c-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="54f2c-121">注釈</span><span class="sxs-lookup"><span data-stu-id="54f2c-121">Remarks</span></span>

<span data-ttu-id="54f2c-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="54f2c-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="54f2c-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="54f2c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f2c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="54f2c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f2c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="54f2c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54f2c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54f2c-126">Schema name</span></span>  <br/> |<span data-ttu-id="54f2c-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="54f2c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54f2c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54f2c-128">Validation file</span></span>  <br/> |<span data-ttu-id="54f2c-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="54f2c-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54f2c-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="54f2c-130">Can be empty</span></span>  <br/> ||
   

