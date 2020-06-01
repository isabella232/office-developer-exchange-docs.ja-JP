---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: HasBlockedImages 要素は、アイテムに画像がブロックされているかどうかを示すブール値を指定します。
ms.openlocfilehash: 370ab4b12ae841815faa344b2fd3a6d3ddc16bcb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462795"
---
# <a name="hasblockedimages"></a><span data-ttu-id="469fb-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="469fb-103">HasBlockedImages</span></span>

<span data-ttu-id="469fb-104">**HasBlockedImages**要素は、アイテムに画像がブロックされているかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="469fb-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="469fb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="469fb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="469fb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="469fb-106">Attributes and elements</span></span>

<span data-ttu-id="469fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="469fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="469fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="469fb-108">Attributes</span></span>

<span data-ttu-id="469fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="469fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="469fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="469fb-110">Child elements</span></span>

<span data-ttu-id="469fb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="469fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="469fb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="469fb-112">Parent elements</span></span>

|<span data-ttu-id="469fb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="469fb-113">**Element**</span></span>|<span data-ttu-id="469fb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="469fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="469fb-115">Item</span><span class="sxs-lookup"><span data-stu-id="469fb-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="469fb-116">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="469fb-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="469fb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="469fb-117">Text value</span></span>

<span data-ttu-id="469fb-118">**HasBlockedImages**要素のテキスト値が**true**の場合は、アイテムに画像がブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="469fb-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="469fb-119">値が**false**の場合は、アイテムにブロックされた画像が含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="469fb-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="469fb-120">注釈</span><span class="sxs-lookup"><span data-stu-id="469fb-120">Remarks</span></span>

<span data-ttu-id="469fb-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="469fb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="469fb-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="469fb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="469fb-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="469fb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="469fb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="469fb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="469fb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="469fb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="469fb-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="469fb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="469fb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="469fb-127">Validation File</span></span>  <br/> |<span data-ttu-id="469fb-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="469fb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="469fb-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="469fb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="469fb-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="469fb-130">See also</span></span>



- [<span data-ttu-id="469fb-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="469fb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

