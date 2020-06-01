---
title: UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: fd2b9545-7213-4427-95ae-71a155b75971
description: UploadItems 要素は、メールボックスにアイテムをアップロードする要求を表します。
ms.openlocfilehash: 8fdb7253926e030085374b650e792349e598ee4a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468825"
---
# <a name="uploaditems"></a><span data-ttu-id="c9e72-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="c9e72-103">UploadItems</span></span>

<span data-ttu-id="c9e72-104">**UploadItems**要素は、メールボックスにアイテムをアップロードする要求を表します。</span><span class="sxs-lookup"><span data-stu-id="c9e72-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="c9e72-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="c9e72-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="c9e72-106">**UploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="c9e72-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9e72-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c9e72-107">Attributes and elements</span></span>

<span data-ttu-id="c9e72-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9e72-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9e72-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9e72-109">Attributes</span></span>

<span data-ttu-id="c9e72-110">なし。</span><span class="sxs-lookup"><span data-stu-id="c9e72-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9e72-111">子要素</span><span class="sxs-lookup"><span data-stu-id="c9e72-111">Child elements</span></span>

|<span data-ttu-id="c9e72-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="c9e72-112">**Element**</span></span>|<span data-ttu-id="c9e72-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9e72-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9e72-114">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="c9e72-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="c9e72-115">メールボックスにアップロードする項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="c9e72-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9e72-116">親要素</span><span class="sxs-lookup"><span data-stu-id="c9e72-116">Parent elements</span></span>

<span data-ttu-id="c9e72-117">なし。</span><span class="sxs-lookup"><span data-stu-id="c9e72-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c9e72-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c9e72-118">Text value</span></span>

<span data-ttu-id="c9e72-119">なし。</span><span class="sxs-lookup"><span data-stu-id="c9e72-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9e72-120">注釈</span><span class="sxs-lookup"><span data-stu-id="c9e72-120">Remarks</span></span>

<span data-ttu-id="c9e72-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c9e72-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9e72-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c9e72-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9e72-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9e72-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9e72-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9e72-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c9e72-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9e72-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="c9e72-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9e72-126">Validation File</span></span>  <br/> |<span data-ttu-id="c9e72-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c9e72-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9e72-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c9e72-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9e72-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="c9e72-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9e72-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9e72-130">See also</span></span>



[<span data-ttu-id="c9e72-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="c9e72-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="c9e72-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="c9e72-132">UploadItems operation</span></span>](uploaditems-operation.md)

