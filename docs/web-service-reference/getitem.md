---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: GetItem 要素は、Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。
ms.openlocfilehash: 39db141bad62c34bec5ae6a937ba94c2d1288090
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760780"
---
# <a name="getitem"></a><span data-ttu-id="7768a-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="7768a-103">GetItem</span></span>

<span data-ttu-id="7768a-104">**GetItem**要素は、Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7768a-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="7768a-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="7768a-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7768a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7768a-106">Attributes and elements</span></span>

<span data-ttu-id="7768a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7768a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7768a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7768a-108">Attributes</span></span>

<span data-ttu-id="7768a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7768a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7768a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7768a-110">Child elements</span></span>

|<span data-ttu-id="7768a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7768a-111">**Element**</span></span>|<span data-ttu-id="7768a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7768a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7768a-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7768a-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="7768a-114">**GetItem**応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="7768a-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="7768a-115">Itemid</span><span class="sxs-lookup"><span data-stu-id="7768a-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="7768a-116">アイテム、出現アイテム、および Exchange ストアから項目を取得するための定期的なマスター アイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7768a-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="7768a-117">これらの項目は、連絡先、タスク、メッセージ、予定表アイテム、会議出席依頼、およびその他のメールボックス内の有効なアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7768a-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7768a-118">親要素</span><span class="sxs-lookup"><span data-stu-id="7768a-118">Parent elements</span></span>

<span data-ttu-id="7768a-119">なし。</span><span class="sxs-lookup"><span data-stu-id="7768a-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7768a-120">備考</span><span class="sxs-lookup"><span data-stu-id="7768a-120">Remarks</span></span>

<span data-ttu-id="7768a-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7768a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7768a-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="7768a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7768a-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="7768a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7768a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7768a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7768a-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7768a-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="7768a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7768a-126">Validation File</span></span>  <br/> |<span data-ttu-id="7768a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7768a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7768a-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7768a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7768a-129">False</span><span class="sxs-lookup"><span data-stu-id="7768a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7768a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7768a-130">See also</span></span>



<span data-ttu-id="7768a-131">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7768a-131">[GetItem operation](getitem-operation.md)</span></span>

