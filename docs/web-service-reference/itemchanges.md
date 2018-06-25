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
description: ItemChanges 要素には、アイテムと、アイテムに適用する更新プログラムを識別する ItemChange 要素の配列が含まれています。
ms.openlocfilehash: 38fe112441a8773a2d6b494ed57c63341cab2b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832141"
---
# <a name="itemchanges"></a><span data-ttu-id="31106-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="31106-103">ItemChanges</span></span>

<span data-ttu-id="31106-104">**ItemChanges**要素には、アイテムと、アイテムに適用する更新プログラムを識別する[ItemChange](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="31106-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="31106-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="31106-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="31106-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="31106-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="31106-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="31106-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31106-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31106-108">Attributes and elements</span></span>

<span data-ttu-id="31106-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31106-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31106-110">属性</span><span class="sxs-lookup"><span data-stu-id="31106-110">Attributes</span></span>

<span data-ttu-id="31106-111">なし。</span><span class="sxs-lookup"><span data-stu-id="31106-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31106-112">子要素</span><span class="sxs-lookup"><span data-stu-id="31106-112">Child elements</span></span>

|<span data-ttu-id="31106-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="31106-113">**Element**</span></span>|<span data-ttu-id="31106-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="31106-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31106-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="31106-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="31106-116">アイテム識別子と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="31106-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31106-117">親要素</span><span class="sxs-lookup"><span data-stu-id="31106-117">Parent elements</span></span>

|<span data-ttu-id="31106-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="31106-118">**Element**</span></span>|<span data-ttu-id="31106-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="31106-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31106-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="31106-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="31106-121">メールボックス内のアイテムを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="31106-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="31106-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="31106-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31106-123">備考</span><span class="sxs-lookup"><span data-stu-id="31106-123">Remarks</span></span>

<span data-ttu-id="31106-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="31106-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31106-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="31106-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31106-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="31106-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31106-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31106-127">Schema Name</span></span>  <br/> |<span data-ttu-id="31106-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="31106-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="31106-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31106-129">Validation File</span></span>  <br/> |<span data-ttu-id="31106-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31106-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31106-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="31106-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="31106-132">False</span><span class="sxs-lookup"><span data-stu-id="31106-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31106-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="31106-133">See also</span></span>



<span data-ttu-id="31106-134">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="31106-134">[UpdateItem operation](updateitem-operation.md)</span></span>

