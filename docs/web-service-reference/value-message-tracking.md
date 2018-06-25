---
title: 値 (メッセージの追跡)
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
description: 値要素は、メッセージ ・ トラッキング ・ レポートのプロパティ値を表します。
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839972"
---
# <a name="value-message-tracking"></a><span data-ttu-id="4c9bc-103">値 (メッセージの追跡)</span><span class="sxs-lookup"><span data-stu-id="4c9bc-103">Value (Message Tracking)</span></span>

<span data-ttu-id="4c9bc-104">**値**要素は、メッセージ ・ トラッキング ・ レポートのプロパティ値を表します。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="4c9bc-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="4c9bc-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4c9bc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4c9bc-106">Attributes and elements</span></span>

<span data-ttu-id="4c9bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c9bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c9bc-108">Attributes</span></span>

<span data-ttu-id="4c9bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c9bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4c9bc-110">Child elements</span></span>

<span data-ttu-id="4c9bc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c9bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4c9bc-112">Parent elements</span></span>

|<span data-ttu-id="4c9bc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4c9bc-113">**Element**</span></span>|<span data-ttu-id="4c9bc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c9bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c9bc-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="4c9bc-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="4c9bc-116">名前と値文字列のペアを使用してレポートを追跡するメッセージのプロパティを作成するを表します。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c9bc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4c9bc-117">Text value</span></span>

<span data-ttu-id="4c9bc-118">テキスト値は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c9bc-119">備考</span><span class="sxs-lookup"><span data-stu-id="4c9bc-119">Remarks</span></span>

<span data-ttu-id="4c9bc-120">この要素に最大で 1 回、 [TrackingPropertyType](trackingpropertytype.md)の要素で発生します。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="4c9bc-121">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4c9bc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c9bc-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="4c9bc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c9bc-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="4c9bc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c9bc-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4c9bc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4c9bc-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4c9bc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c9bc-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4c9bc-126">Validation File</span></span>  <br/> |<span data-ttu-id="4c9bc-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c9bc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c9bc-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4c9bc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c9bc-129">False</span><span class="sxs-lookup"><span data-stu-id="4c9bc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c9bc-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4c9bc-130">See also</span></span>

- [<span data-ttu-id="4c9bc-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4c9bc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

