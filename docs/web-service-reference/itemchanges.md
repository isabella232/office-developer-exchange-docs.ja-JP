---
title: ItemChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChanges
api_type:
- schema
ms.assetid: cd307892-2f69-4494-8325-219bdb5c3ad5
description: ItemChanges 要素には、アイテムとアイテムに適用する更新を識別する Itemchanges 要素の配列が含まれています。
ms.openlocfilehash: ea6fb2023b88360f9558057e80c7fe0d855173b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459911"
---
# <a name="itemchanges"></a><span data-ttu-id="14536-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="14536-103">ItemChanges</span></span>

<span data-ttu-id="14536-104">**Itemchanges**要素には、アイテムとアイテムに適用する更新を識別する[itemchanges](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="14536-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="14536-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="14536-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="14536-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="14536-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="14536-107">**非 Emptyarrayofitemchangestん**</span><span class="sxs-lookup"><span data-stu-id="14536-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14536-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="14536-108">Attributes and elements</span></span>

<span data-ttu-id="14536-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="14536-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14536-110">属性</span><span class="sxs-lookup"><span data-stu-id="14536-110">Attributes</span></span>

<span data-ttu-id="14536-111">なし。</span><span class="sxs-lookup"><span data-stu-id="14536-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14536-112">子要素</span><span class="sxs-lookup"><span data-stu-id="14536-112">Child elements</span></span>

|<span data-ttu-id="14536-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="14536-113">**Element**</span></span>|<span data-ttu-id="14536-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="14536-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14536-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="14536-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="14536-116">アイテム識別子と、アイテムに適用する更新を含みます。</span><span class="sxs-lookup"><span data-stu-id="14536-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14536-117">親要素</span><span class="sxs-lookup"><span data-stu-id="14536-117">Parent elements</span></span>

|<span data-ttu-id="14536-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="14536-118">**Element**</span></span>|<span data-ttu-id="14536-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="14536-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14536-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="14536-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="14536-121">メールボックス内のアイテムを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="14536-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="14536-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14536-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="14536-123">注釈</span><span class="sxs-lookup"><span data-stu-id="14536-123">Remarks</span></span>

<span data-ttu-id="14536-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="14536-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14536-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="14536-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14536-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="14536-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14536-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="14536-127">Schema Name</span></span>  <br/> |<span data-ttu-id="14536-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="14536-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="14536-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="14536-129">Validation File</span></span>  <br/> |<span data-ttu-id="14536-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="14536-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14536-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="14536-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="14536-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="14536-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14536-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="14536-133">See also</span></span>



<span data-ttu-id="14536-134">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="14536-134">[UpdateItem operation](updateitem-operation.md)</span></span>

