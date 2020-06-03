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
ms.openlocfilehash: 36011e0252ed391daefab190d4da679fb3a3f856
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463098"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="d6cfe-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="d6cfe-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="d6cfe-104">**Extendedproperties**要素は、追加のプロパティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="d6cfe-105">**NonEmptyArrayOfExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="d6cfe-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6cfe-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d6cfe-106">Attributes and elements</span></span>

<span data-ttu-id="d6cfe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6cfe-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6cfe-108">Attributes</span></span>

<span data-ttu-id="d6cfe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6cfe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d6cfe-110">Child elements</span></span>

|<span data-ttu-id="d6cfe-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d6cfe-111">**Element**</span></span>|<span data-ttu-id="d6cfe-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6cfe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6cfe-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d6cfe-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="d6cfe-114">フォルダーとアイテムの拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6cfe-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d6cfe-115">Parent elements</span></span>

|<span data-ttu-id="d6cfe-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6cfe-116">**Element**</span></span>|<span data-ttu-id="d6cfe-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6cfe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6cfe-118">ImGroup</span><span class="sxs-lookup"><span data-stu-id="d6cfe-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="d6cfe-119">インスタントメッセージンググループを表します。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="d6cfe-120">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="d6cfe-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="d6cfe-121">アイテムを開かずに、プレビューのメールボックスアイテムの最初の256文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6cfe-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d6cfe-122">Remarks</span></span>

<span data-ttu-id="d6cfe-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d6cfe-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6cfe-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d6cfe-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6cfe-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6cfe-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6cfe-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6cfe-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d6cfe-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="d6cfe-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="d6cfe-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6cfe-129">Validation File</span></span>  <br/> |<span data-ttu-id="d6cfe-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d6cfe-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6cfe-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d6cfe-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d6cfe-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6cfe-132">See also</span></span>



- [<span data-ttu-id="d6cfe-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6cfe-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

