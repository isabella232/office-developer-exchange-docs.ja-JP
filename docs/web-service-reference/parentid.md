---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: ParentId 要素では、サーチ プレビューに親アイテムの識別子を指定します。
ms.openlocfilehash: ddc76320b1c482e3518a98fb63fc2296143d163c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832698"
---
# <a name="parentid"></a><span data-ttu-id="4012b-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="4012b-103">ParentId</span></span>

<span data-ttu-id="4012b-104">**ParentId**要素では、サーチ プレビューに親アイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4012b-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="4012b-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="4012b-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4012b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4012b-106">Attributes and elements</span></span>

<span data-ttu-id="4012b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4012b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4012b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4012b-108">Attributes</span></span>

|<span data-ttu-id="4012b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4012b-109">**Attribute**</span></span>|<span data-ttu-id="4012b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4012b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4012b-111">ID</span><span class="sxs-lookup"><span data-stu-id="4012b-111">Id</span></span>  <br/> |<span data-ttu-id="4012b-112">**Id**属性のテキスト値は、親アイテムの識別子です。</span><span class="sxs-lookup"><span data-stu-id="4012b-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="4012b-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="4012b-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="4012b-114">**変更キー**属性のテキスト値は、親アイテムのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="4012b-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4012b-115">子要素</span><span class="sxs-lookup"><span data-stu-id="4012b-115">Child elements</span></span>

<span data-ttu-id="4012b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="4012b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4012b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4012b-117">Parent elements</span></span>

[<span data-ttu-id="4012b-118">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="4012b-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="4012b-119">備考</span><span class="sxs-lookup"><span data-stu-id="4012b-119">Remarks</span></span>

<span data-ttu-id="4012b-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4012b-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4012b-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4012b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4012b-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="4012b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4012b-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="4012b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4012b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4012b-124">Schema name</span></span>  <br/> |<span data-ttu-id="4012b-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4012b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4012b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4012b-126">Validation file</span></span>  <br/> |<span data-ttu-id="4012b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4012b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4012b-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4012b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="4012b-129">true</span><span class="sxs-lookup"><span data-stu-id="4012b-129">true</span></span>  <br/> |
   

