---
title: ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: bbbc56e4-8cc1-43ae-b70a-9a8d6bb0f399
description: ExportItems 要素は、メールボックスからアイテムをエクスポートする要求を表します。
ms.openlocfilehash: 6e4996f62ea5051e6dc235ee7255057f16b3855b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457271"
---
# <a name="exportitems"></a><span data-ttu-id="51a89-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="51a89-103">ExportItems</span></span>

<span data-ttu-id="51a89-104">**ExportItems**要素は、メールボックスからアイテムをエクスポートする要求を表します。</span><span class="sxs-lookup"><span data-stu-id="51a89-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="51a89-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="51a89-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="51a89-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="51a89-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51a89-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51a89-107">Attributes and elements</span></span>

<span data-ttu-id="51a89-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51a89-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51a89-109">属性</span><span class="sxs-lookup"><span data-stu-id="51a89-109">Attributes</span></span>

<span data-ttu-id="51a89-110">なし。</span><span class="sxs-lookup"><span data-stu-id="51a89-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51a89-111">子要素</span><span class="sxs-lookup"><span data-stu-id="51a89-111">Child elements</span></span>

|<span data-ttu-id="51a89-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="51a89-112">**Element**</span></span>|<span data-ttu-id="51a89-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="51a89-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51a89-114">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="51a89-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="51a89-115">メールボックスからエクスポートするアイテムを識別するアイテム識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="51a89-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51a89-116">親要素</span><span class="sxs-lookup"><span data-stu-id="51a89-116">Parent elements</span></span>

<span data-ttu-id="51a89-117">なし。</span><span class="sxs-lookup"><span data-stu-id="51a89-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="51a89-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="51a89-118">Text value</span></span>

<span data-ttu-id="51a89-119">なし。</span><span class="sxs-lookup"><span data-stu-id="51a89-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51a89-120">注釈</span><span class="sxs-lookup"><span data-stu-id="51a89-120">Remarks</span></span>

<span data-ttu-id="51a89-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="51a89-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51a89-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51a89-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51a89-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="51a89-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="51a89-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51a89-124">Schema Name</span></span>  <br/> |<span data-ttu-id="51a89-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="51a89-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="51a89-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51a89-126">Validation File</span></span>  <br/> |<span data-ttu-id="51a89-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="51a89-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51a89-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51a89-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="51a89-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="51a89-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51a89-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="51a89-130">See also</span></span>



[<span data-ttu-id="51a89-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="51a89-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="51a89-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="51a89-132">UploadItems operation</span></span>](uploaditems-operation.md)

