---
title: ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: ExtendedProperties 要素は、追加のプロパティの配列を指定します。
ms.openlocfilehash: b92108ecde63d4a3ac3cc80861c204c4d1950cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760412"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="dae3b-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="dae3b-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="dae3b-104">**ExtendedProperties**要素は、追加のプロパティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="dae3b-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="dae3b-105">**NonEmptyArrayOfExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="dae3b-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dae3b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dae3b-106">Attributes and elements</span></span>

<span data-ttu-id="dae3b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dae3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dae3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="dae3b-108">Attributes</span></span>

<span data-ttu-id="dae3b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dae3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dae3b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dae3b-110">Child elements</span></span>

|<span data-ttu-id="dae3b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dae3b-111">**Element**</span></span>|<span data-ttu-id="dae3b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae3b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae3b-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="dae3b-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="dae3b-114">フォルダーおよびアイテムの拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="dae3b-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dae3b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dae3b-115">Parent elements</span></span>

|<span data-ttu-id="dae3b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dae3b-116">**Element**</span></span>|<span data-ttu-id="dae3b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae3b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae3b-118">ImGroup</span><span class="sxs-lookup"><span data-stu-id="dae3b-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="dae3b-119">インスタント メッセージングのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="dae3b-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="dae3b-120">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="dae3b-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="dae3b-121">アイテムを開かずにプレビューを表示するメールボックスのアイテムの最初の 256 文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="dae3b-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dae3b-122">備考</span><span class="sxs-lookup"><span data-stu-id="dae3b-122">Remarks</span></span>

<span data-ttu-id="dae3b-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dae3b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dae3b-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dae3b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dae3b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="dae3b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dae3b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="dae3b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dae3b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dae3b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="dae3b-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="dae3b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="dae3b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dae3b-129">Validation File</span></span>  <br/> |<span data-ttu-id="dae3b-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="dae3b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dae3b-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dae3b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dae3b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="dae3b-132">See also</span></span>



- [<span data-ttu-id="dae3b-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dae3b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

