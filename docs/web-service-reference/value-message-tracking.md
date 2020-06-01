---
title: 値 (メッセージ追跡)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: Value 要素は、メッセージ追跡レポートのプロパティ値を表します。
ms.openlocfilehash: 4f6b5cb9d82a35bbe010b36e409cdc9f3a70173d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465009"
---
# <a name="value-message-tracking"></a><span data-ttu-id="ae3a5-103">値 (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="ae3a5-103">Value (Message Tracking)</span></span>

<span data-ttu-id="ae3a5-104">**Value**要素は、メッセージ追跡レポートのプロパティ値を表します。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="ae3a5-105">**String**</span><span class="sxs-lookup"><span data-stu-id="ae3a5-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ae3a5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ae3a5-106">Attributes and elements</span></span>

<span data-ttu-id="ae3a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae3a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae3a5-108">Attributes</span></span>

<span data-ttu-id="ae3a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae3a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ae3a5-110">Child elements</span></span>

<span data-ttu-id="ae3a5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae3a5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ae3a5-112">Parent elements</span></span>

|<span data-ttu-id="ae3a5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae3a5-113">**Element**</span></span>|<span data-ttu-id="ae3a5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae3a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae3a5-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="ae3a5-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="ae3a5-116">メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae3a5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ae3a5-117">Text value</span></span>

<span data-ttu-id="ae3a5-118">テキスト値はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae3a5-119">注釈</span><span class="sxs-lookup"><span data-stu-id="ae3a5-119">Remarks</span></span>

<span data-ttu-id="ae3a5-120">この要素は、 [TrackingPropertyType](trackingpropertytype.md)要素で最大で1回発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="ae3a5-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ae3a5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae3a5-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ae3a5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae3a5-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae3a5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae3a5-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae3a5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ae3a5-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ae3a5-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae3a5-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae3a5-126">Validation File</span></span>  <br/> |<span data-ttu-id="ae3a5-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ae3a5-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae3a5-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ae3a5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae3a5-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="ae3a5-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae3a5-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae3a5-130">See also</span></span>

- [<span data-ttu-id="ae3a5-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae3a5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

