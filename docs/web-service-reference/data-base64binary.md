---
title: データ (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: データ要素には、エクスポートされたアイテムを 1 つまたはメールボックスにアップロードするアイテムのデータが含まれています。
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759902"
---
# <a name="data-base64binary"></a><span data-ttu-id="25643-103">データ (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="25643-103">Data (base64Binary)</span></span>

<span data-ttu-id="25643-104">**データ**要素には、エクスポートされたアイテムを 1 つまたはメールボックスにアップロードするアイテムのデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="25643-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="25643-105">**xs:base64Binary**</span><span class="sxs-lookup"><span data-stu-id="25643-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="25643-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="25643-106">Attributes and elements</span></span>

<span data-ttu-id="25643-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="25643-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25643-108">属性</span><span class="sxs-lookup"><span data-stu-id="25643-108">Attributes</span></span>

<span data-ttu-id="25643-109">なし。</span><span class="sxs-lookup"><span data-stu-id="25643-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25643-110">子要素</span><span class="sxs-lookup"><span data-stu-id="25643-110">Child elements</span></span>

<span data-ttu-id="25643-111">なし。</span><span class="sxs-lookup"><span data-stu-id="25643-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25643-112">親要素</span><span class="sxs-lookup"><span data-stu-id="25643-112">Parent elements</span></span>

|<span data-ttu-id="25643-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="25643-113">**Element**</span></span>|<span data-ttu-id="25643-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="25643-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25643-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="25643-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="25643-116">状態および 1 つのメールボックス アイテムをエクスポートするのには要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="25643-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="25643-117">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="25643-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="25643-118">メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="25643-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25643-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="25643-119">Text value</span></span>

<span data-ttu-id="25643-120">**データ**要素には、プロパティ名とメールボックスにアップロードするには、エクスポートされたアイテムの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="25643-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="25643-121">備考</span><span class="sxs-lookup"><span data-stu-id="25643-121">Remarks</span></span>

<span data-ttu-id="25643-122">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="25643-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25643-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="25643-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25643-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="25643-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="25643-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="25643-125">Schema Name</span></span>  <br/> |<span data-ttu-id="25643-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="25643-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="25643-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="25643-127">Validation File</span></span>  <br/> |<span data-ttu-id="25643-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="25643-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="25643-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="25643-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="25643-130">False</span><span class="sxs-lookup"><span data-stu-id="25643-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25643-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="25643-131">See also</span></span>

- [<span data-ttu-id="25643-132">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="25643-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="25643-133">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="25643-133">UploadItems operation</span></span>](uploaditems-operation.md)

