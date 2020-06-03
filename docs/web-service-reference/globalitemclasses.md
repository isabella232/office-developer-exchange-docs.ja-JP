---
title: GlobalItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemClasses
api_type:
- schema
ms.assetid: 72634700-6d75-44c0-80b7-8c31743c04d6
description: GlobalItemClasses 要素には、メールボックス内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれています。
ms.openlocfilehash: e4cb8a8886f8262e8cb4a550b054e81ea18a5e11
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459434"
---
# <a name="globalitemclasses"></a><span data-ttu-id="72ba3-103">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="72ba3-103">GlobalItemClasses</span></span>

<span data-ttu-id="72ba3-104">**Globalitemclasses**要素には、メールボックス内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="72ba3-104">The **GlobalItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="72ba3-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="72ba3-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="72ba3-106">会話</span><span class="sxs-lookup"><span data-stu-id="72ba3-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="72ba3-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="72ba3-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="72ba3-108">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="72ba3-108">GlobalItemClasses</span></span>](globalitemclasses.md)
  
```XML
<GlobalItemClasses>
    <String/>
</GlobalItemClasses>
```

 <span data-ttu-id="72ba3-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="72ba3-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72ba3-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="72ba3-110">Attributes and elements</span></span>

<span data-ttu-id="72ba3-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72ba3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72ba3-112">属性</span><span class="sxs-lookup"><span data-stu-id="72ba3-112">Attributes</span></span>

<span data-ttu-id="72ba3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="72ba3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72ba3-114">子要素</span><span class="sxs-lookup"><span data-stu-id="72ba3-114">Child elements</span></span>

|<span data-ttu-id="72ba3-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="72ba3-115">**Element**</span></span>|<span data-ttu-id="72ba3-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="72ba3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72ba3-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="72ba3-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="72ba3-118">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="72ba3-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72ba3-119">親要素</span><span class="sxs-lookup"><span data-stu-id="72ba3-119">Parent elements</span></span>

|<span data-ttu-id="72ba3-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="72ba3-120">**Element**</span></span>|<span data-ttu-id="72ba3-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="72ba3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72ba3-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="72ba3-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="72ba3-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="72ba3-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72ba3-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="72ba3-124">Text value</span></span>

<span data-ttu-id="72ba3-125">なし。</span><span class="sxs-lookup"><span data-stu-id="72ba3-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72ba3-126">注釈</span><span class="sxs-lookup"><span data-stu-id="72ba3-126">Remarks</span></span>

<span data-ttu-id="72ba3-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="72ba3-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72ba3-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="72ba3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72ba3-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="72ba3-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72ba3-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72ba3-130">Schema name</span></span>  <br/> |<span data-ttu-id="72ba3-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="72ba3-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="72ba3-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72ba3-132">Validation file</span></span>  <br/> |<span data-ttu-id="72ba3-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="72ba3-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72ba3-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="72ba3-134">Can be empty</span></span>  <br/> |<span data-ttu-id="72ba3-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="72ba3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72ba3-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="72ba3-136">See also</span></span>



[<span data-ttu-id="72ba3-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="72ba3-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="72ba3-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="72ba3-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="72ba3-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="72ba3-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

