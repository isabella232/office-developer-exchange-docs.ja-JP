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
description: ItemClasses 要素は、条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスを表します。
ms.openlocfilehash: 56b99cad2abef0a9953e1793e5b633acca83a9eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460114"
---
# <a name="itemclasses"></a><span data-ttu-id="f1894-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="f1894-103">ItemClasses</span></span>

<span data-ttu-id="f1894-104">**Itemclasses**要素は、条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="f1894-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="f1894-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="f1894-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1894-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f1894-106">Attributes and elements</span></span>

<span data-ttu-id="f1894-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f1894-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1894-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1894-108">Attributes</span></span>

<span data-ttu-id="f1894-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f1894-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1894-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f1894-110">Child elements</span></span>

|<span data-ttu-id="f1894-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f1894-111">**Element**</span></span>|<span data-ttu-id="f1894-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1894-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1894-113">String</span><span class="sxs-lookup"><span data-stu-id="f1894-113">String</span></span>](string.md) <br/> |<span data-ttu-id="f1894-114">1つのアイテムクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="f1894-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1894-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f1894-115">Parent elements</span></span>

|<span data-ttu-id="f1894-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f1894-116">**Element**</span></span>|<span data-ttu-id="f1894-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1894-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1894-118">条件</span><span class="sxs-lookup"><span data-stu-id="f1894-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="f1894-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="f1894-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="f1894-120">例外</span><span class="sxs-lookup"><span data-stu-id="f1894-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="f1894-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="f1894-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1894-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f1894-122">Text value</span></span>

<span data-ttu-id="f1894-123">なし。</span><span class="sxs-lookup"><span data-stu-id="f1894-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1894-124">注釈</span><span class="sxs-lookup"><span data-stu-id="f1894-124">Remarks</span></span>

<span data-ttu-id="f1894-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f1894-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1894-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f1894-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1894-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1894-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1894-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f1894-128">Schema name</span></span>  <br/> |<span data-ttu-id="f1894-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f1894-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1894-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f1894-130">Validation file</span></span>  <br/> |<span data-ttu-id="f1894-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f1894-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1894-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f1894-132">Can be empty</span></span>  <br/> |<span data-ttu-id="f1894-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="f1894-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1894-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="f1894-134">See also</span></span>



- [<span data-ttu-id="f1894-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f1894-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

