---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: GlobalImportance 要素には、メールボックス内のすべての会話項目の集計の重要性が含まれています。
ms.openlocfilehash: c9cdcf20fd3e6eca9ab501cbc747544a4d7b7ded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831731"
---
# <a name="globalimportance"></a><span data-ttu-id="2ee75-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="2ee75-103">GlobalImportance</span></span>

<span data-ttu-id="2ee75-104">**GlobalImportance**要素には、メールボックス内のすべての会話項目の集計の重要性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ee75-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="2ee75-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="2ee75-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="2ee75-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="2ee75-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="2ee75-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2ee75-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="2ee75-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="2ee75-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="2ee75-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="2ee75-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ee75-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2ee75-110">Attributes and elements</span></span>

<span data-ttu-id="2ee75-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ee75-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ee75-112">属性</span><span class="sxs-lookup"><span data-stu-id="2ee75-112">Attributes</span></span>

<span data-ttu-id="2ee75-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2ee75-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ee75-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2ee75-114">Child elements</span></span>

<span data-ttu-id="2ee75-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2ee75-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ee75-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2ee75-116">Parent elements</span></span>

|<span data-ttu-id="2ee75-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="2ee75-117">**Element**</span></span>|<span data-ttu-id="2ee75-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2ee75-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ee75-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2ee75-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="2ee75-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="2ee75-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ee75-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2ee75-121">Text value</span></span>

<span data-ttu-id="2ee75-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="2ee75-122">A text value is required.</span></span> <span data-ttu-id="2ee75-123">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="2ee75-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="2ee75-124">低</span><span class="sxs-lookup"><span data-stu-id="2ee75-124">Low</span></span>
    
- <span data-ttu-id="2ee75-125">Normal</span><span class="sxs-lookup"><span data-stu-id="2ee75-125">Normal</span></span>
    
- <span data-ttu-id="2ee75-126">高</span><span class="sxs-lookup"><span data-stu-id="2ee75-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2ee75-127">備考</span><span class="sxs-lookup"><span data-stu-id="2ee75-127">Remarks</span></span>

<span data-ttu-id="2ee75-128">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2ee75-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ee75-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="2ee75-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ee75-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="2ee75-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ee75-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ee75-131">Schema name</span></span>  <br/> |<span data-ttu-id="2ee75-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2ee75-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ee75-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ee75-133">Validation file</span></span>  <br/> |<span data-ttu-id="2ee75-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ee75-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ee75-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ee75-135">Can be empty</span></span>  <br/> |<span data-ttu-id="2ee75-136">False</span><span class="sxs-lookup"><span data-stu-id="2ee75-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ee75-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ee75-137">See also</span></span>



<span data-ttu-id="2ee75-138">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="2ee75-138">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="2ee75-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="2ee75-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="2ee75-140">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="2ee75-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

