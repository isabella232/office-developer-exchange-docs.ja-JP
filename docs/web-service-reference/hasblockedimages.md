---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: HasBlockedImages 要素は、アイテムの画像がブロックされているかどうかを示すブール値を指定します。
ms.openlocfilehash: fbe9967c898016aeef27e3c86e8a1cf603bd87fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831795"
---
# <a name="hasblockedimages"></a><span data-ttu-id="5f85d-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="5f85d-103">HasBlockedImages</span></span>

<span data-ttu-id="5f85d-104">**HasBlockedImages**要素は、アイテムの画像がブロックされているかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f85d-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="5f85d-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="5f85d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f85d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5f85d-106">Attributes and elements</span></span>

<span data-ttu-id="5f85d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f85d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f85d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f85d-108">Attributes</span></span>

<span data-ttu-id="5f85d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5f85d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f85d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5f85d-110">Child elements</span></span>

<span data-ttu-id="5f85d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5f85d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f85d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5f85d-112">Parent elements</span></span>

|<span data-ttu-id="5f85d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f85d-113">**Element**</span></span>|<span data-ttu-id="5f85d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f85d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f85d-115">Item</span><span class="sxs-lookup"><span data-stu-id="5f85d-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="5f85d-116">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="5f85d-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f85d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5f85d-117">Text value</span></span>

<span data-ttu-id="5f85d-118">の**場合は true** 、 **HasBlockedImages**要素のテキスト値は、アイテムの画像がブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="5f85d-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="5f85d-119">**False**の値は、項目がすべてブロックされている画像を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="5f85d-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5f85d-120">備考</span><span class="sxs-lookup"><span data-stu-id="5f85d-120">Remarks</span></span>

<span data-ttu-id="5f85d-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5f85d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5f85d-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5f85d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f85d-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="5f85d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f85d-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="5f85d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f85d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f85d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5f85d-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="5f85d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="5f85d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f85d-127">Validation File</span></span>  <br/> |<span data-ttu-id="5f85d-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="5f85d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f85d-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5f85d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5f85d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f85d-130">See also</span></span>



- [<span data-ttu-id="5f85d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f85d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

