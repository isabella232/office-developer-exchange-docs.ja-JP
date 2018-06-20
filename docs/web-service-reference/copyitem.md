---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: CopyItem 要素は、Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759784"
---
# <a name="copyitem"></a><span data-ttu-id="ede00-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="ede00-103">CopyItem</span></span>

<span data-ttu-id="ede00-104">**CopyItem**要素は、Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ede00-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="ede00-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="ede00-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ede00-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ede00-106">Attributes and elements</span></span>

<span data-ttu-id="ede00-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ede00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ede00-108">属性</span><span class="sxs-lookup"><span data-stu-id="ede00-108">Attributes</span></span>

<span data-ttu-id="ede00-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ede00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ede00-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ede00-110">Child elements</span></span>

|<span data-ttu-id="ede00-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ede00-111">**Element**</span></span>|<span data-ttu-id="ede00-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ede00-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ede00-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="ede00-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="ede00-114">コピーされたアイテムのコピー先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ede00-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="ede00-115">Itemid</span><span class="sxs-lookup"><span data-stu-id="ede00-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="ede00-116">[ToFolderId](tofolderid.md)要素によって表されるフォルダーにコピーするのには特定の項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ede00-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="ede00-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="ede00-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="ede00-118">新しい項目の項目の識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ede00-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ede00-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ede00-119">Parent elements</span></span>

<span data-ttu-id="ede00-120">なし。</span><span class="sxs-lookup"><span data-stu-id="ede00-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ede00-121">備考</span><span class="sxs-lookup"><span data-stu-id="ede00-121">Remarks</span></span>

<span data-ttu-id="ede00-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ede00-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ede00-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="ede00-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ede00-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="ede00-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ede00-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ede00-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ede00-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ede00-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ede00-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ede00-127">Validation File</span></span>  <br/> |<span data-ttu-id="ede00-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ede00-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ede00-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ede00-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ede00-130">False</span><span class="sxs-lookup"><span data-stu-id="ede00-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ede00-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="ede00-131">See also</span></span>



<span data-ttu-id="ede00-132">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="ede00-132">[CopyItem operation](copyitem-operation.md)</span></span>


- [<span data-ttu-id="ede00-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ede00-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

