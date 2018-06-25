---
title: ItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: ItemClasses 要素は、適用する条件または例外の順序で受信したメッセージにスタンプする必要がある項目クラスを表します。
ms.openlocfilehash: 70a4823f9017ba8c6f894394d5907f1adeb80167
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832148"
---
# <a name="itemclasses"></a><span data-ttu-id="b4f77-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="b4f77-103">ItemClasses</span></span>

<span data-ttu-id="b4f77-104">**ItemClasses**要素は、適用する条件または例外の順序で受信したメッセージにスタンプする必要がある項目クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="b4f77-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="b4f77-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b4f77-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4f77-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b4f77-106">Attributes and elements</span></span>

<span data-ttu-id="b4f77-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b4f77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4f77-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4f77-108">Attributes</span></span>

<span data-ttu-id="b4f77-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b4f77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4f77-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b4f77-110">Child elements</span></span>

|<span data-ttu-id="b4f77-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4f77-111">**Element**</span></span>|<span data-ttu-id="b4f77-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4f77-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4f77-113">String</span><span class="sxs-lookup"><span data-stu-id="b4f77-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b4f77-114">アイテムを 1 つのクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="b4f77-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4f77-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b4f77-115">Parent elements</span></span>

|<span data-ttu-id="b4f77-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4f77-116">**Element**</span></span>|<span data-ttu-id="b4f77-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4f77-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4f77-118">条件</span><span class="sxs-lookup"><span data-stu-id="b4f77-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b4f77-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="b4f77-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b4f77-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b4f77-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b4f77-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="b4f77-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b4f77-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b4f77-122">Text value</span></span>

<span data-ttu-id="b4f77-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b4f77-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b4f77-124">備考</span><span class="sxs-lookup"><span data-stu-id="b4f77-124">Remarks</span></span>

<span data-ttu-id="b4f77-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b4f77-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4f77-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b4f77-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4f77-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b4f77-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4f77-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b4f77-128">Schema name</span></span>  <br/> |<span data-ttu-id="b4f77-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b4f77-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4f77-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b4f77-130">Validation file</span></span>  <br/> |<span data-ttu-id="b4f77-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b4f77-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4f77-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b4f77-132">Can be empty</span></span>  <br/> |<span data-ttu-id="b4f77-133">False</span><span class="sxs-lookup"><span data-stu-id="b4f77-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4f77-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b4f77-134">See also</span></span>



- [<span data-ttu-id="b4f77-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b4f77-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

