---
title: ID (ItemIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9909ed2-fdc5-4b1f-b7db-1f517add8eb3
description: Id 要素は、項目の識別子を指定します。
ms.openlocfilehash: a0abd81de0fc30bc5168543fc75f44d470eef100
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831849"
---
# <a name="id-itemidtype"></a><span data-ttu-id="9c33c-103">ID (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="9c33c-103">ID (ItemIdType)</span></span>

<span data-ttu-id="9c33c-104">**Id**要素は、項目の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c33c-104">The **Id** element specifies the identifier of an item.</span></span> 
  
```XML
<Id Id="" ChangeKey=""/>
```

 <span data-ttu-id="9c33c-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="9c33c-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c33c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9c33c-106">Attributes and elements</span></span>

<span data-ttu-id="9c33c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c33c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c33c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c33c-108">Attributes</span></span>

|<span data-ttu-id="9c33c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9c33c-109">**Attribute**</span></span>|<span data-ttu-id="9c33c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c33c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c33c-111">ID</span><span class="sxs-lookup"><span data-stu-id="9c33c-111">Id</span></span>  <br/> |<span data-ttu-id="9c33c-112">**Id**属性のテキスト値は、項目の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9c33c-112">The text value of the **Id** attribute is the identifier of the item.</span></span>  <br/> |
|<span data-ttu-id="9c33c-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="9c33c-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="9c33c-114">**変更キー**属性のテキスト値は、項目のキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="9c33c-114">The text value of the **ChangeKey** attribute is the change key of the item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9c33c-115">子要素</span><span class="sxs-lookup"><span data-stu-id="9c33c-115">Child elements</span></span>

<span data-ttu-id="9c33c-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9c33c-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c33c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="9c33c-117">Parent elements</span></span>

[<span data-ttu-id="9c33c-118">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="9c33c-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="9c33c-119">備考</span><span class="sxs-lookup"><span data-stu-id="9c33c-119">Remarks</span></span>

<span data-ttu-id="9c33c-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9c33c-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9c33c-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9c33c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c33c-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9c33c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c33c-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9c33c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c33c-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c33c-124">Schema name</span></span>  <br/> |<span data-ttu-id="9c33c-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9c33c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c33c-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c33c-126">Validation file</span></span>  <br/> |<span data-ttu-id="9c33c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c33c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c33c-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9c33c-128">Can be empty</span></span>  <br/> ||
   

