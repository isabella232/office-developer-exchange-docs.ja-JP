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
description: GetItem 要素は、Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。
ms.openlocfilehash: a02403ee84195a41387d5dbe1785ae6d12b47da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458699"
---
# <a name="getitem"></a><span data-ttu-id="60c8d-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="60c8d-103">GetItem</span></span>

<span data-ttu-id="60c8d-104">**GetItem**要素は、Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="60c8d-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="60c8d-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="60c8d-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60c8d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="60c8d-106">Attributes and elements</span></span>

<span data-ttu-id="60c8d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60c8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60c8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="60c8d-108">Attributes</span></span>

<span data-ttu-id="60c8d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="60c8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60c8d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="60c8d-110">Child elements</span></span>

|<span data-ttu-id="60c8d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="60c8d-111">**Element**</span></span>|<span data-ttu-id="60c8d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="60c8d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60c8d-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="60c8d-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="60c8d-114">**GetItem**応答に含めるアイテムのプロパティとコンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="60c8d-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="60c8d-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="60c8d-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="60c8d-116">Exchange ストアからアイテムを取得するために使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60c8d-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="60c8d-117">これらのアイテムは、メールボックス内の連絡先、タスク、メッセージ、予定表アイテム、会議出席依頼、およびその他の有効なアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="60c8d-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60c8d-118">親要素</span><span class="sxs-lookup"><span data-stu-id="60c8d-118">Parent elements</span></span>

<span data-ttu-id="60c8d-119">なし。</span><span class="sxs-lookup"><span data-stu-id="60c8d-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60c8d-120">注釈</span><span class="sxs-lookup"><span data-stu-id="60c8d-120">Remarks</span></span>

<span data-ttu-id="60c8d-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="60c8d-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60c8d-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="60c8d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60c8d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="60c8d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60c8d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60c8d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="60c8d-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="60c8d-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="60c8d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60c8d-126">Validation File</span></span>  <br/> |<span data-ttu-id="60c8d-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="60c8d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60c8d-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="60c8d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="60c8d-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="60c8d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60c8d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="60c8d-130">See also</span></span>



[<span data-ttu-id="60c8d-131">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="60c8d-131">GetItem operation</span></span>](getitem-operation.md)

