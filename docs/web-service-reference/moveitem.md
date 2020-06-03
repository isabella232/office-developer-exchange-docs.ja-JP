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
ms.openlocfilehash: 61dbb91cc20a71f50999241b3daa21bf8ebfbcc8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530402"
---
# <a name="moveitem"></a><span data-ttu-id="015cc-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="015cc-103">MoveItem</span></span>

<span data-ttu-id="015cc-104">**Moveitem**要素は、Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="015cc-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="015cc-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="015cc-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="015cc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="015cc-106">Attributes and elements</span></span>

<span data-ttu-id="015cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="015cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="015cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="015cc-108">Attributes</span></span>

<span data-ttu-id="015cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="015cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="015cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="015cc-110">Child elements</span></span>

|<span data-ttu-id="015cc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="015cc-111">**Element**</span></span>|<span data-ttu-id="015cc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="015cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="015cc-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="015cc-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="015cc-114">移動されたアイテムの移動先のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="015cc-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="015cc-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="015cc-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="015cc-116">[ToFolderId](tofolderid.md)要素によって表されるフォルダーに移動する、識別されたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="015cc-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="015cc-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="015cc-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="015cc-118">新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="015cc-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="015cc-119">親要素</span><span class="sxs-lookup"><span data-stu-id="015cc-119">Parent elements</span></span>

<span data-ttu-id="015cc-120">なし。</span><span class="sxs-lookup"><span data-stu-id="015cc-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="015cc-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="015cc-121">Text value</span></span>

<span data-ttu-id="015cc-122">なし。</span><span class="sxs-lookup"><span data-stu-id="015cc-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="015cc-123">注釈</span><span class="sxs-lookup"><span data-stu-id="015cc-123">Remarks</span></span>

<span data-ttu-id="015cc-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="015cc-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="015cc-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="015cc-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="015cc-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="015cc-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="015cc-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="015cc-127">Schema Name</span></span>  <br/> |<span data-ttu-id="015cc-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="015cc-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="015cc-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="015cc-129">Validation File</span></span>  <br/> |<span data-ttu-id="015cc-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="015cc-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="015cc-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="015cc-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="015cc-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="015cc-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="015cc-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="015cc-133">See also</span></span>



[<span data-ttu-id="015cc-134">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="015cc-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="015cc-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="015cc-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

