---
title: Data (base64Binary)
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
description: Data 要素には、1つのエクスポートされたアイテムまたはメールボックスにアップロードするアイテムのデータが含まれています。
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526971"
---
# <a name="data-base64binary"></a><span data-ttu-id="ed535-103">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="ed535-103">Data (base64Binary)</span></span>

<span data-ttu-id="ed535-104">**Data**要素には、1つのエクスポートされたアイテムまたはメールボックスにアップロードするアイテムのデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed535-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="ed535-105">**xs: base64Binary**</span><span class="sxs-lookup"><span data-stu-id="ed535-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ed535-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ed535-106">Attributes and elements</span></span>

<span data-ttu-id="ed535-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed535-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed535-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed535-108">Attributes</span></span>

<span data-ttu-id="ed535-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed535-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed535-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed535-110">Child elements</span></span>

<span data-ttu-id="ed535-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ed535-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed535-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ed535-112">Parent elements</span></span>

|<span data-ttu-id="ed535-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed535-113">**Element**</span></span>|<span data-ttu-id="ed535-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed535-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed535-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ed535-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="ed535-116">1つのメールボックスアイテムをエクスポートする要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="ed535-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="ed535-117">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="ed535-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="ed535-118">メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ed535-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed535-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed535-119">Text value</span></span>

<span data-ttu-id="ed535-120">**Data**要素には、エクスポートされたアイテムまたはメールボックスにアップロードされるアイテムのプロパティ名と値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed535-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ed535-121">注釈</span><span class="sxs-lookup"><span data-stu-id="ed535-121">Remarks</span></span>

<span data-ttu-id="ed535-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ed535-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed535-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ed535-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed535-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed535-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed535-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed535-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ed535-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ed535-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="ed535-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed535-127">Validation File</span></span>  <br/> |<span data-ttu-id="ed535-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ed535-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed535-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed535-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed535-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="ed535-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed535-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed535-131">See also</span></span>

- [<span data-ttu-id="ed535-132">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="ed535-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="ed535-133">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="ed535-133">UploadItems operation</span></span>](uploaditems-operation.md)

