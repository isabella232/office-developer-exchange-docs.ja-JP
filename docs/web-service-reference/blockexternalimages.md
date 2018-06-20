---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: BlockExternalImages 要素は、HTML テキストの本体で外部の画像がブロックされているかどうかを指定します。
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759504"
---
# <a name="blockexternalimages"></a><span data-ttu-id="4864b-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="4864b-103">BlockExternalImages</span></span>

<span data-ttu-id="4864b-104">**BlockExternalImages**要素は、HTML テキストの本体で外部の画像がブロックされているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4864b-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="4864b-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="4864b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4864b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4864b-106">Attributes and elements</span></span>

<span data-ttu-id="4864b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4864b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4864b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4864b-108">Attributes</span></span>

<span data-ttu-id="4864b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4864b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4864b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4864b-110">Child elements</span></span>

<span data-ttu-id="4864b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4864b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4864b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4864b-112">Parent elements</span></span>

|<span data-ttu-id="4864b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4864b-113">**Element**</span></span>|<span data-ttu-id="4864b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4864b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4864b-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="4864b-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="4864b-116">GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="4864b-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="4864b-117">ItemShape</span><span class="sxs-lookup"><span data-stu-id="4864b-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="4864b-118">GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="4864b-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4864b-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4864b-119">Text value</span></span>

<span data-ttu-id="4864b-120">**True** **BlockExternalImages**要素のテキスト値は、HTML の本文で、外部の画像がブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="4864b-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="4864b-121">**False**の値は、外部の画像が許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="4864b-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4864b-122">備考</span><span class="sxs-lookup"><span data-stu-id="4864b-122">Remarks</span></span>

<span data-ttu-id="4864b-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4864b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4864b-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4864b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4864b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="4864b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4864b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="4864b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4864b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4864b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4864b-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4864b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4864b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4864b-129">Validation File</span></span>  <br/> |<span data-ttu-id="4864b-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4864b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4864b-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4864b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4864b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4864b-132">See also</span></span>



- [<span data-ttu-id="4864b-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4864b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

