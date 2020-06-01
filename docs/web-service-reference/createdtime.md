---
title: CreatedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7055c86f-c364-42d3-87b4-c741ccb15c57
description: Created Time 要素は、アイテムが作成された時刻を指定します。
ms.openlocfilehash: 709e6021e48a9f2b4857b9283750306d5e513c72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44445315"
---
# <a name="createdtime"></a><span data-ttu-id="55388-103">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="55388-103">CreatedTime</span></span>

<span data-ttu-id="55388-104">Created **time**要素は、アイテムが作成された時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="55388-104">The **CreatedTime** element specifies the time at which the item was created.</span></span> 
  
```xml
<CreatedTime></CreatedTime>
```

 <span data-ttu-id="55388-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="55388-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55388-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="55388-106">Attributes and elements</span></span>

<span data-ttu-id="55388-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55388-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55388-108">属性</span><span class="sxs-lookup"><span data-stu-id="55388-108">Attributes</span></span>

<span data-ttu-id="55388-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55388-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55388-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55388-110">Child elements</span></span>

<span data-ttu-id="55388-111">なし。</span><span class="sxs-lookup"><span data-stu-id="55388-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55388-112">親要素</span><span class="sxs-lookup"><span data-stu-id="55388-112">Parent elements</span></span>

|<span data-ttu-id="55388-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="55388-113">**Element**</span></span>|<span data-ttu-id="55388-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="55388-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55388-115">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="55388-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="55388-116">アイテムを開かずに、プレビューのメールボックスアイテムの最初の256文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="55388-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55388-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55388-117">Text value</span></span>

<span data-ttu-id="55388-118">指定した time 要素のテキスト値は、アイテムが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="55388-118">The text value of the CreatedTime element is the time at which the item was created.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55388-119">注釈</span><span class="sxs-lookup"><span data-stu-id="55388-119">Remarks</span></span>

<span data-ttu-id="55388-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="55388-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55388-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="55388-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55388-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="55388-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55388-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="55388-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55388-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55388-124">Schema Name</span></span>  <br/> |<span data-ttu-id="55388-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="55388-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="55388-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55388-126">Validation File</span></span>  <br/> |<span data-ttu-id="55388-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="55388-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="55388-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="55388-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="55388-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="55388-129">See also</span></span>



- [<span data-ttu-id="55388-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="55388-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

