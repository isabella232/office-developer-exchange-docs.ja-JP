---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: MovedItemId 要素は、MarkAsJunk 操作によって移動されたアイテムの識別子を指定します。
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832484"
---
# <a name="moveditemid"></a><span data-ttu-id="ab539-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="ab539-103">MovedItemId</span></span>

<span data-ttu-id="ab539-104">**MovedItemId**要素は、 **MarkAsJunk**操作によって移動されたアイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab539-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="ab539-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="ab539-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab539-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ab539-106">Attributes and elements</span></span>

<span data-ttu-id="ab539-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ab539-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab539-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab539-108">Attributes</span></span>

|<span data-ttu-id="ab539-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ab539-109">**Attribute**</span></span>|<span data-ttu-id="ab539-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ab539-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ab539-111">ID</span><span class="sxs-lookup"><span data-stu-id="ab539-111">Id</span></span>  <br/> |<span data-ttu-id="ab539-112">**Id**属性の値は、 **MarkAsJunk**操作によって移動された項目の項目の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ab539-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="ab539-113">アイテム識別子は変わりません、移動した後です。</span><span class="sxs-lookup"><span data-stu-id="ab539-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="ab539-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="ab539-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="ab539-115">**変更キー**属性の値は、移動された項目のキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="ab539-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="ab539-116">キーの変更は、 **MarkAsJunk**操作でアイテムを移動した後に変更します。</span><span class="sxs-lookup"><span data-stu-id="ab539-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ab539-117">子要素</span><span class="sxs-lookup"><span data-stu-id="ab539-117">Child elements</span></span>

<span data-ttu-id="ab539-118">なし。</span><span class="sxs-lookup"><span data-stu-id="ab539-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab539-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ab539-119">Parent elements</span></span>

[<span data-ttu-id="ab539-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ab539-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="ab539-121">備考</span><span class="sxs-lookup"><span data-stu-id="ab539-121">Remarks</span></span>

<span data-ttu-id="ab539-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ab539-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ab539-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ab539-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab539-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="ab539-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab539-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="ab539-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ab539-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ab539-126">Schema name</span></span>  <br/> |<span data-ttu-id="ab539-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ab539-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ab539-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ab539-128">Validation file</span></span>  <br/> |<span data-ttu-id="ab539-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ab539-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ab539-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ab539-130">Can be empty</span></span>  <br/> ||
   

