---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: BaseShape の要素は、返される少数のプロパティで返されるすべてのプロパティの既定のプレビューまたはコンパクトなプレビューのいずれかを指定します。
ms.openlocfilehash: 1f060ae9adf52cc2916a634e3d954e3fc0903941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759491"
---
# <a name="baseshape-previewitembaseshapetype"></a><span data-ttu-id="70f08-103">BaseShape (PreviewItemBaseShapeType)</span><span class="sxs-lookup"><span data-stu-id="70f08-103">BaseShape (PreviewItemBaseShapeType)</span></span>

<span data-ttu-id="70f08-104">**BaseShape**の要素は、返される少数のプロパティで返されるすべてのプロパティの既定のプレビューまたはコンパクトなプレビューのいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="70f08-104">The **BaseShape** element specifies either the default preview with all properties returned or a compact preview with fewer properties returned.</span></span> 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 <span data-ttu-id="70f08-105">**PreviewItemBaseShapeType**</span><span class="sxs-lookup"><span data-stu-id="70f08-105">**PreviewItemBaseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70f08-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="70f08-106">Attributes and elements</span></span>

<span data-ttu-id="70f08-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70f08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70f08-108">属性</span><span class="sxs-lookup"><span data-stu-id="70f08-108">Attributes</span></span>

<span data-ttu-id="70f08-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70f08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70f08-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70f08-110">Child elements</span></span>

<span data-ttu-id="70f08-111">なし。</span><span class="sxs-lookup"><span data-stu-id="70f08-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70f08-112">親要素</span><span class="sxs-lookup"><span data-stu-id="70f08-112">Parent elements</span></span>

|<span data-ttu-id="70f08-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="70f08-113">**Element**</span></span>|<span data-ttu-id="70f08-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="70f08-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70f08-115">PreviewItemResponseShape</span><span class="sxs-lookup"><span data-stu-id="70f08-115">PreviewItemResponseShape</span></span>](previewitemresponseshape.md) <br/> |<span data-ttu-id="70f08-116">応答の図形が含まれています。</span><span class="sxs-lookup"><span data-stu-id="70f08-116">Contains the shape of the response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70f08-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70f08-117">Text value</span></span>

<span data-ttu-id="70f08-118">**BaseShape の要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="70f08-118">**BaseShape element text values**</span></span>

|<span data-ttu-id="70f08-119">**値**</span><span class="sxs-lookup"><span data-stu-id="70f08-119">**Value**</span></span>|<span data-ttu-id="70f08-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="70f08-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70f08-121">Default</span><span class="sxs-lookup"><span data-stu-id="70f08-121">Default</span></span>  <br/> |<span data-ttu-id="70f08-122">すべてのプロパティが表示されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="70f08-122">Indicates that all properties are shown.</span></span>  <br/> |
|<span data-ttu-id="70f08-123">コンパクト</span><span class="sxs-lookup"><span data-stu-id="70f08-123">Compact</span></span>  <br/> |<span data-ttu-id="70f08-124">選択したプロパティのみが表示されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="70f08-124">Indicates that only selected properties are shown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70f08-125">備考</span><span class="sxs-lookup"><span data-stu-id="70f08-125">Remarks</span></span>

<span data-ttu-id="70f08-126">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="70f08-126">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="70f08-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="70f08-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70f08-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="70f08-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70f08-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="70f08-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70f08-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70f08-130">Schema Name</span></span>  <br/> |<span data-ttu-id="70f08-131">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="70f08-131">Type schema</span></span>  <br/> |
|<span data-ttu-id="70f08-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70f08-132">Validation File</span></span>  <br/> |<span data-ttu-id="70f08-133">types.xsd</span><span class="sxs-lookup"><span data-stu-id="70f08-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="70f08-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70f08-134">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="70f08-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="70f08-135">See also</span></span>



- [<span data-ttu-id="70f08-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="70f08-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

