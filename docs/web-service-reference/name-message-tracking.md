---
title: Name (メッセージ追跡)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: Name 要素は、メッセージ追跡レポートのプロパティ名を表します。
ms.openlocfilehash: 86f049c0a90dbeb55418a5eee58079adf17e5ded
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466900"
---
# <a name="name-message-tracking"></a><span data-ttu-id="23b15-103">Name (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="23b15-103">Name (Message Tracking)</span></span>

<span data-ttu-id="23b15-104">**Name**要素は、メッセージ追跡レポートのプロパティ名を表します。</span><span class="sxs-lookup"><span data-stu-id="23b15-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="23b15-105">**String**</span><span class="sxs-lookup"><span data-stu-id="23b15-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="23b15-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="23b15-106">Attributes and elements</span></span>

<span data-ttu-id="23b15-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23b15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23b15-108">属性</span><span class="sxs-lookup"><span data-stu-id="23b15-108">Attributes</span></span>

<span data-ttu-id="23b15-109">なし。</span><span class="sxs-lookup"><span data-stu-id="23b15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23b15-110">子要素</span><span class="sxs-lookup"><span data-stu-id="23b15-110">Child elements</span></span>

<span data-ttu-id="23b15-111">なし。</span><span class="sxs-lookup"><span data-stu-id="23b15-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23b15-112">親要素</span><span class="sxs-lookup"><span data-stu-id="23b15-112">Parent elements</span></span>

|<span data-ttu-id="23b15-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="23b15-113">**Element**</span></span>|<span data-ttu-id="23b15-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="23b15-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23b15-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="23b15-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="23b15-116">メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="23b15-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23b15-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="23b15-117">Text value</span></span>

<span data-ttu-id="23b15-118">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="23b15-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23b15-119">注釈</span><span class="sxs-lookup"><span data-stu-id="23b15-119">Remarks</span></span>

<span data-ttu-id="23b15-120">この要素は、 [TrackingPropertyType](trackingpropertytype.md)要素で最大で1回発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="23b15-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="23b15-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="23b15-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23b15-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="23b15-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23b15-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="23b15-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23b15-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23b15-124">Schema Name</span></span>  <br/> |<span data-ttu-id="23b15-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="23b15-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="23b15-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23b15-126">Validation File</span></span>  <br/> |<span data-ttu-id="23b15-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="23b15-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23b15-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="23b15-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="23b15-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="23b15-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23b15-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="23b15-130">See also</span></span>

- [<span data-ttu-id="23b15-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="23b15-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

