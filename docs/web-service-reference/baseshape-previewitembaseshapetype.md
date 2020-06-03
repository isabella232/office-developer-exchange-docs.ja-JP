---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: BaseShape 要素は、返されたすべてのプロパティを持つ既定のプレビューを指定します。または、コンパクトプレビューで返されるプロパティの数が少なくなります。
ms.openlocfilehash: 29f008840d649f97dfb299fee8e7bf5aaa573404
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527419"
---
# <a name="baseshape-previewitembaseshapetype"></a><span data-ttu-id="d65da-103">BaseShape (PreviewItemBaseShapeType)</span><span class="sxs-lookup"><span data-stu-id="d65da-103">BaseShape (PreviewItemBaseShapeType)</span></span>

<span data-ttu-id="d65da-104">**Baseshape**要素は、返されたすべてのプロパティを持つ既定のプレビューを指定します。または、コンパクトプレビューで返されるプロパティの数が少なくなります。</span><span class="sxs-lookup"><span data-stu-id="d65da-104">The **BaseShape** element specifies either the default preview with all properties returned or a compact preview with fewer properties returned.</span></span> 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 <span data-ttu-id="d65da-105">**PreviewItemBaseShapeType**</span><span class="sxs-lookup"><span data-stu-id="d65da-105">**PreviewItemBaseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d65da-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d65da-106">Attributes and elements</span></span>

<span data-ttu-id="d65da-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d65da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d65da-108">属性</span><span class="sxs-lookup"><span data-stu-id="d65da-108">Attributes</span></span>

<span data-ttu-id="d65da-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d65da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d65da-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d65da-110">Child elements</span></span>

<span data-ttu-id="d65da-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d65da-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d65da-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d65da-112">Parent elements</span></span>

|<span data-ttu-id="d65da-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d65da-113">**Element**</span></span>|<span data-ttu-id="d65da-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d65da-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d65da-115">プレビュー Itemresponseshape</span><span class="sxs-lookup"><span data-stu-id="d65da-115">PreviewItemResponseShape</span></span>](previewitemresponseshape.md) <br/> |<span data-ttu-id="d65da-116">応答の図形を含みます。</span><span class="sxs-lookup"><span data-stu-id="d65da-116">Contains the shape of the response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d65da-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d65da-117">Text value</span></span>

<span data-ttu-id="d65da-118">**BaseShape 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="d65da-118">**BaseShape element text values**</span></span>

|<span data-ttu-id="d65da-119">**値**</span><span class="sxs-lookup"><span data-stu-id="d65da-119">**Value**</span></span>|<span data-ttu-id="d65da-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="d65da-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d65da-121">既定値</span><span class="sxs-lookup"><span data-stu-id="d65da-121">Default</span></span>  <br/> |<span data-ttu-id="d65da-122">すべてのプロパティが表示されることを示します。</span><span class="sxs-lookup"><span data-stu-id="d65da-122">Indicates that all properties are shown.</span></span>  <br/> |
|<span data-ttu-id="d65da-123">コンパクト</span><span class="sxs-lookup"><span data-stu-id="d65da-123">Compact</span></span>  <br/> |<span data-ttu-id="d65da-124">選択されているプロパティのみが表示されることを示します。</span><span class="sxs-lookup"><span data-stu-id="d65da-124">Indicates that only selected properties are shown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d65da-125">注釈</span><span class="sxs-lookup"><span data-stu-id="d65da-125">Remarks</span></span>

<span data-ttu-id="d65da-126">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d65da-126">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d65da-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d65da-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d65da-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d65da-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d65da-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d65da-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d65da-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d65da-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d65da-131">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="d65da-131">Type schema</span></span>  <br/> |
|<span data-ttu-id="d65da-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d65da-132">Validation File</span></span>  <br/> |<span data-ttu-id="d65da-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d65da-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d65da-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d65da-134">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d65da-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="d65da-135">See also</span></span>



- [<span data-ttu-id="d65da-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d65da-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

