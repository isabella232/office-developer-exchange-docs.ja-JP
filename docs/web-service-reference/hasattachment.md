---
title: 添付ファイルあり
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: 添付ファイルあり要素では、アイテムが添付ファイルがあるかどうかを示すブール値を指定します。
ms.openlocfilehash: dfe163e0850e835784a43984a34c89f14bfbc59b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831798"
---
# <a name="hasattachment"></a><span data-ttu-id="886f1-103">添付ファイルあり</span><span class="sxs-lookup"><span data-stu-id="886f1-103">HasAttachment</span></span>

<span data-ttu-id="886f1-104">**添付ファイルあり**要素では、アイテムが添付ファイルがあるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="886f1-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="886f1-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="886f1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="886f1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="886f1-106">Attributes and elements</span></span>

<span data-ttu-id="886f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="886f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="886f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="886f1-108">Attributes</span></span>

<span data-ttu-id="886f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="886f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="886f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="886f1-110">Child elements</span></span>

<span data-ttu-id="886f1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="886f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="886f1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="886f1-112">Parent elements</span></span>

|<span data-ttu-id="886f1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="886f1-113">**Element**</span></span>|<span data-ttu-id="886f1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="886f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="886f1-115">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="886f1-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="886f1-116">アイテムを開かずにプレビューを表示するメールボックスのアイテムの最初の 256 文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="886f1-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="886f1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="886f1-117">Text value</span></span>

<span data-ttu-id="886f1-118">の**場合は true** **添付ファイルあり**要素のテキスト値は、アイテムに添付ファイルがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="886f1-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="886f1-119">**False**の値は、アイテムが添付ファイルを持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="886f1-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="886f1-120">備考</span><span class="sxs-lookup"><span data-stu-id="886f1-120">Remarks</span></span>

<span data-ttu-id="886f1-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="886f1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="886f1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="886f1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="886f1-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="886f1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="886f1-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="886f1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="886f1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="886f1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="886f1-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="886f1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="886f1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="886f1-127">Validation File</span></span>  <br/> |<span data-ttu-id="886f1-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="886f1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="886f1-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="886f1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="886f1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="886f1-130">See also</span></span>



- [<span data-ttu-id="886f1-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="886f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

