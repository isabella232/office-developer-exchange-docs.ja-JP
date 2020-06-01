---
title: GlobalSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalSize
api_type:
- schema
ms.assetid: 23c24437-8dab-4c86-888d-471d23af675a
description: GlobalSize 要素には、メールボックス内のすべての会話アイテムのサイズによって計算された会話のサイズが含まれています。
ms.openlocfilehash: d23ab080dadb006cd5eff9d712d081fe7d94a2a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462452"
---
# <a name="globalsize"></a><span data-ttu-id="d50c5-103">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="d50c5-103">GlobalSize</span></span>

<span data-ttu-id="d50c5-104">**Globalsize**要素には、メールボックス内のすべての会話アイテムのサイズによって計算された会話のサイズが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d50c5-104">The **GlobalSize** element contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="d50c5-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d50c5-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d50c5-106">会話</span><span class="sxs-lookup"><span data-stu-id="d50c5-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="d50c5-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d50c5-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="d50c5-108">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="d50c5-108">GlobalSize</span></span>](globalsize.md)
  
```XML
<GlobalSize/>
```

 <span data-ttu-id="d50c5-109">**xs: int**</span><span class="sxs-lookup"><span data-stu-id="d50c5-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d50c5-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d50c5-110">Attributes and elements</span></span>

<span data-ttu-id="d50c5-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d50c5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d50c5-112">属性</span><span class="sxs-lookup"><span data-stu-id="d50c5-112">Attributes</span></span>

<span data-ttu-id="d50c5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d50c5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d50c5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d50c5-114">Child elements</span></span>

<span data-ttu-id="d50c5-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d50c5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d50c5-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d50c5-116">Parent elements</span></span>

|<span data-ttu-id="d50c5-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d50c5-117">**Element**</span></span>|<span data-ttu-id="d50c5-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d50c5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d50c5-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d50c5-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d50c5-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="d50c5-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d50c5-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d50c5-121">Text value</span></span>

<span data-ttu-id="d50c5-122">**Globalsize**要素のテキスト値は、メールボックス内のすべての会話アイテムのサイズから計算された会話のサイズです。</span><span class="sxs-lookup"><span data-stu-id="d50c5-122">The text value of the **GlobalSize** element is the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d50c5-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d50c5-123">Remarks</span></span>

<span data-ttu-id="d50c5-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d50c5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d50c5-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d50c5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d50c5-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d50c5-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d50c5-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d50c5-127">Schema name</span></span>  <br/> |<span data-ttu-id="d50c5-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d50c5-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d50c5-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d50c5-129">Validation file</span></span>  <br/> |<span data-ttu-id="d50c5-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d50c5-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d50c5-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d50c5-131">Can be empty</span></span>  <br/> |<span data-ttu-id="d50c5-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="d50c5-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d50c5-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d50c5-133">See also</span></span>



[<span data-ttu-id="d50c5-134">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="d50c5-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="d50c5-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="d50c5-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="d50c5-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="d50c5-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

