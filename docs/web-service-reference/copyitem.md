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
description: CopyItem 要素は、Exchange ストア内のメールボックス内のアイテムをコピーする要求を定義します。
ms.openlocfilehash: b9af1670fd580107de08ad3b950191399436388d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458503"
---
# <a name="copyitem"></a><span data-ttu-id="edf8a-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="edf8a-103">CopyItem</span></span>

<span data-ttu-id="edf8a-104">**Copyitem**要素は、Exchange ストア内のメールボックス内のアイテムをコピーする要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="edf8a-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="edf8a-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="edf8a-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edf8a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="edf8a-106">Attributes and elements</span></span>

<span data-ttu-id="edf8a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="edf8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edf8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="edf8a-108">Attributes</span></span>

<span data-ttu-id="edf8a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="edf8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edf8a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="edf8a-110">Child elements</span></span>

|<span data-ttu-id="edf8a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="edf8a-111">**Element**</span></span>|<span data-ttu-id="edf8a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="edf8a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edf8a-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="edf8a-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="edf8a-114">コピーされたアイテムの移動先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="edf8a-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="edf8a-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="edf8a-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="edf8a-116">[ToFolderId](tofolderid.md)要素で表されるフォルダーにコピーする、識別されたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="edf8a-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="edf8a-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="edf8a-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="edf8a-118">新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="edf8a-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="edf8a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="edf8a-119">Parent elements</span></span>

<span data-ttu-id="edf8a-120">なし。</span><span class="sxs-lookup"><span data-stu-id="edf8a-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="edf8a-121">注釈</span><span class="sxs-lookup"><span data-stu-id="edf8a-121">Remarks</span></span>

<span data-ttu-id="edf8a-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="edf8a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edf8a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="edf8a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edf8a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="edf8a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="edf8a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="edf8a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="edf8a-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="edf8a-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="edf8a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="edf8a-127">Validation File</span></span>  <br/> |<span data-ttu-id="edf8a-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="edf8a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="edf8a-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="edf8a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="edf8a-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="edf8a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edf8a-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="edf8a-131">See also</span></span>



<span data-ttu-id="edf8a-132">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="edf8a-132">[CopyItem operation](copyitem-operation.md)</span></span>


- [<span data-ttu-id="edf8a-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="edf8a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

