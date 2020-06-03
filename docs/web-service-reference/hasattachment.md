---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: HasAttachment 要素は、アイテムに添付ファイルがあるかどうかを示すブール値を指定します。
ms.openlocfilehash: c6bc0932a08a1bbec215bb8a974ed746d2961123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530262"
---
# <a name="hasattachment"></a><span data-ttu-id="6b288-103">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="6b288-103">HasAttachment</span></span>

<span data-ttu-id="6b288-104">**Hasattachment**要素は、アイテムに添付ファイルがあるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b288-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="6b288-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6b288-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b288-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6b288-106">Attributes and elements</span></span>

<span data-ttu-id="6b288-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b288-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b288-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b288-108">Attributes</span></span>

<span data-ttu-id="6b288-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b288-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b288-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b288-110">Child elements</span></span>

<span data-ttu-id="6b288-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6b288-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b288-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6b288-112">Parent elements</span></span>

|<span data-ttu-id="6b288-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b288-113">**Element**</span></span>|<span data-ttu-id="6b288-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b288-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b288-115">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="6b288-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="6b288-116">アイテムを開かずに、プレビューのメールボックスアイテムの最初の256文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b288-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b288-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b288-117">Text value</span></span>

<span data-ttu-id="6b288-118">**Hasattachment**要素のテキスト値が**true の場合**は、アイテムに添付ファイルがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="6b288-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="6b288-119">値が**false**の場合は、アイテムに添付ファイルがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6b288-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6b288-120">注釈</span><span class="sxs-lookup"><span data-stu-id="6b288-120">Remarks</span></span>

<span data-ttu-id="6b288-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6b288-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b288-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b288-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b288-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6b288-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b288-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b288-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b288-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b288-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6b288-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="6b288-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6b288-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b288-127">Validation File</span></span>  <br/> |<span data-ttu-id="6b288-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6b288-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b288-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6b288-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6b288-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b288-130">See also</span></span>



- [<span data-ttu-id="6b288-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b288-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

