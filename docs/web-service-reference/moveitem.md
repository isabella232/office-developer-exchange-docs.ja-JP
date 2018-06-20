---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: MoveItem 要素は、Exchange ストア内のアイテムを移動する要求を定義します。
ms.openlocfilehash: cd7f35bdabe8a596f4c186df1c8cd54e0ea1c540
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832486"
---
# <a name="moveitem"></a><span data-ttu-id="dd3db-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="dd3db-103">MoveItem</span></span>

<span data-ttu-id="dd3db-104">**MoveItem**要素は、Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="dd3db-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="dd3db-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="dd3db-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd3db-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd3db-106">Attributes and elements</span></span>

<span data-ttu-id="dd3db-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd3db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd3db-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd3db-108">Attributes</span></span>

<span data-ttu-id="dd3db-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd3db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd3db-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd3db-110">Child elements</span></span>

|<span data-ttu-id="dd3db-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd3db-111">**Element**</span></span>|<span data-ttu-id="dd3db-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd3db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd3db-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="dd3db-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="dd3db-114">移動された項目のコピー先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="dd3db-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="dd3db-115">Itemid</span><span class="sxs-lookup"><span data-stu-id="dd3db-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="dd3db-116">[ToFolderId](tofolderid.md)要素によって表されるフォルダーに移動する特定の項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd3db-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="dd3db-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="dd3db-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="dd3db-118">新しい項目の項目の識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dd3db-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd3db-119">親要素</span><span class="sxs-lookup"><span data-stu-id="dd3db-119">Parent elements</span></span>

<span data-ttu-id="dd3db-120">なし。</span><span class="sxs-lookup"><span data-stu-id="dd3db-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="dd3db-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dd3db-121">Text value</span></span>

<span data-ttu-id="dd3db-122">なし。</span><span class="sxs-lookup"><span data-stu-id="dd3db-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd3db-123">備考</span><span class="sxs-lookup"><span data-stu-id="dd3db-123">Remarks</span></span>

<span data-ttu-id="dd3db-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dd3db-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd3db-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd3db-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd3db-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd3db-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd3db-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd3db-127">Schema Name</span></span>  <br/> |<span data-ttu-id="dd3db-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dd3db-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd3db-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd3db-129">Validation File</span></span>  <br/> |<span data-ttu-id="dd3db-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd3db-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd3db-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dd3db-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd3db-132">False</span><span class="sxs-lookup"><span data-stu-id="dd3db-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd3db-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd3db-133">See also</span></span>



<span data-ttu-id="dd3db-134">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dd3db-134">[MoveItem operation](moveitem-operation.md)</span></span>


- [<span data-ttu-id="dd3db-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd3db-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

