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
description: GlobalImportance 度要素には、メールボックス内のすべての会話アイテムの集約された重要度が含まれています。
ms.openlocfilehash: c760168afa3edac20ca0ae7bc677610d8456d178
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459448"
---
# <a name="globalimportance"></a><span data-ttu-id="912bb-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="912bb-103">GlobalImportance</span></span>

<span data-ttu-id="912bb-104">**Globalimportance 度**要素には、メールボックス内のすべての会話アイテムの集約された重要度が含まれています。</span><span class="sxs-lookup"><span data-stu-id="912bb-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="912bb-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="912bb-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="912bb-106">会話</span><span class="sxs-lookup"><span data-stu-id="912bb-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="912bb-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="912bb-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="912bb-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="912bb-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="912bb-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="912bb-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="912bb-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="912bb-110">Attributes and elements</span></span>

<span data-ttu-id="912bb-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="912bb-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="912bb-112">属性</span><span class="sxs-lookup"><span data-stu-id="912bb-112">Attributes</span></span>

<span data-ttu-id="912bb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="912bb-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="912bb-114">子要素</span><span class="sxs-lookup"><span data-stu-id="912bb-114">Child elements</span></span>

<span data-ttu-id="912bb-115">なし。</span><span class="sxs-lookup"><span data-stu-id="912bb-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="912bb-116">親要素</span><span class="sxs-lookup"><span data-stu-id="912bb-116">Parent elements</span></span>

|<span data-ttu-id="912bb-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="912bb-117">**Element**</span></span>|<span data-ttu-id="912bb-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="912bb-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="912bb-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="912bb-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="912bb-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="912bb-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="912bb-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="912bb-121">Text value</span></span>

<span data-ttu-id="912bb-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="912bb-122">A text value is required.</span></span> <span data-ttu-id="912bb-123">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="912bb-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="912bb-124">低</span><span class="sxs-lookup"><span data-stu-id="912bb-124">Low</span></span>
    
- <span data-ttu-id="912bb-125">標準</span><span class="sxs-lookup"><span data-stu-id="912bb-125">Normal</span></span>
    
- <span data-ttu-id="912bb-126">高</span><span class="sxs-lookup"><span data-stu-id="912bb-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="912bb-127">注釈</span><span class="sxs-lookup"><span data-stu-id="912bb-127">Remarks</span></span>

<span data-ttu-id="912bb-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="912bb-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="912bb-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="912bb-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="912bb-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="912bb-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="912bb-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="912bb-131">Schema name</span></span>  <br/> |<span data-ttu-id="912bb-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="912bb-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="912bb-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="912bb-133">Validation file</span></span>  <br/> |<span data-ttu-id="912bb-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="912bb-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="912bb-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="912bb-135">Can be empty</span></span>  <br/> |<span data-ttu-id="912bb-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="912bb-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="912bb-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="912bb-137">See also</span></span>



[<span data-ttu-id="912bb-138">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="912bb-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="912bb-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="912bb-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="912bb-140">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="912bb-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

