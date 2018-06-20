---
title: 削除の種類
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: 削除の種類の要素では、会話内の項目を削除する方法を示します。
ms.openlocfilehash: abaa0c3d8b7001b2f42a38d1c82475edba32d2c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759988"
---
# <a name="deletetype"></a><span data-ttu-id="fe002-103">削除の種類</span><span class="sxs-lookup"><span data-stu-id="fe002-103">DeleteType</span></span>

<span data-ttu-id="fe002-104">**削除の種類**の要素では、会話内の項目を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fe002-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="fe002-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="fe002-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="fe002-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="fe002-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="fe002-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="fe002-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="fe002-108">削除の種類</span><span class="sxs-lookup"><span data-stu-id="fe002-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="fe002-109">**DisposalType**</span><span class="sxs-lookup"><span data-stu-id="fe002-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe002-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fe002-110">Attributes and elements</span></span>

<span data-ttu-id="fe002-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe002-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe002-112">属性</span><span class="sxs-lookup"><span data-stu-id="fe002-112">Attributes</span></span>

<span data-ttu-id="fe002-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fe002-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe002-114">子要素</span><span class="sxs-lookup"><span data-stu-id="fe002-114">Child elements</span></span>

<span data-ttu-id="fe002-115">なし。</span><span class="sxs-lookup"><span data-stu-id="fe002-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe002-116">親要素</span><span class="sxs-lookup"><span data-stu-id="fe002-116">Parent elements</span></span>

|<span data-ttu-id="fe002-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="fe002-117">**Element**</span></span>|<span data-ttu-id="fe002-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe002-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe002-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="fe002-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="fe002-120">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe002-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe002-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fe002-121">Text value</span></span>

<span data-ttu-id="fe002-122">**削除の種類**の要素のテキスト値では、会話内の項目を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fe002-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="fe002-123">可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="fe002-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="fe002-124">HardDelete - では、会話内のアイテムがメールボックス データベースから完全に削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="fe002-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="fe002-125">MoveToDeleteItems では、会話内のアイテムが削除済みアイテム フォルダーに移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="fe002-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="fe002-126">SoftDelete では、会話内のアイテムに移動したことを示します、ごみ箱をあさる場合、収集を有効にします。</span><span class="sxs-lookup"><span data-stu-id="fe002-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fe002-127">備考</span><span class="sxs-lookup"><span data-stu-id="fe002-127">Remarks</span></span>

<span data-ttu-id="fe002-128">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fe002-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe002-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="fe002-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe002-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="fe002-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe002-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fe002-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fe002-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fe002-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe002-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fe002-133">Validation File</span></span>  <br/> |<span data-ttu-id="fe002-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fe002-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe002-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fe002-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe002-136">False</span><span class="sxs-lookup"><span data-stu-id="fe002-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe002-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="fe002-137">See also</span></span>

- [<span data-ttu-id="fe002-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="fe002-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="fe002-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fe002-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

