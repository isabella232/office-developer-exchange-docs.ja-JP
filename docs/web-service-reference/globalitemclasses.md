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
description: GlobalItemClasses 要素には、メールボックス内の会話項目のすべてのアイテム クラスを表す項目のクラスのリストが含まれています。
ms.openlocfilehash: a8f947d37c1335f1eaba5550a2b3a0aece0246ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831735"
---
# <a name="globalitemclasses"></a><span data-ttu-id="88dc0-103">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="88dc0-103">GlobalItemClasses</span></span>

<span data-ttu-id="88dc0-104">**GlobalItemClasses**要素には、メールボックス内の会話項目のすべてのアイテム クラスを表す項目のクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="88dc0-104">The **GlobalItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="88dc0-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="88dc0-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="88dc0-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="88dc0-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="88dc0-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88dc0-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="88dc0-108">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="88dc0-108">GlobalItemClasses</span></span>](globalitemclasses.md)
  
```XML
<GlobalItemClasses>
    <String/>
</GlobalItemClasses>
```

 <span data-ttu-id="88dc0-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="88dc0-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88dc0-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="88dc0-110">Attributes and elements</span></span>

<span data-ttu-id="88dc0-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="88dc0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88dc0-112">属性</span><span class="sxs-lookup"><span data-stu-id="88dc0-112">Attributes</span></span>

<span data-ttu-id="88dc0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="88dc0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88dc0-114">子要素</span><span class="sxs-lookup"><span data-stu-id="88dc0-114">Child elements</span></span>

|<span data-ttu-id="88dc0-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="88dc0-115">**Element**</span></span>|<span data-ttu-id="88dc0-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="88dc0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88dc0-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="88dc0-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="88dc0-118">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="88dc0-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88dc0-119">親要素</span><span class="sxs-lookup"><span data-stu-id="88dc0-119">Parent elements</span></span>

|<span data-ttu-id="88dc0-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="88dc0-120">**Element**</span></span>|<span data-ttu-id="88dc0-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="88dc0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88dc0-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88dc0-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="88dc0-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="88dc0-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88dc0-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="88dc0-124">Text value</span></span>

<span data-ttu-id="88dc0-125">なし。</span><span class="sxs-lookup"><span data-stu-id="88dc0-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88dc0-126">備考</span><span class="sxs-lookup"><span data-stu-id="88dc0-126">Remarks</span></span>

<span data-ttu-id="88dc0-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="88dc0-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88dc0-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="88dc0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88dc0-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="88dc0-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88dc0-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="88dc0-130">Schema name</span></span>  <br/> |<span data-ttu-id="88dc0-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="88dc0-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="88dc0-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="88dc0-132">Validation file</span></span>  <br/> |<span data-ttu-id="88dc0-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88dc0-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88dc0-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="88dc0-134">Can be empty</span></span>  <br/> |<span data-ttu-id="88dc0-135">False</span><span class="sxs-lookup"><span data-stu-id="88dc0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88dc0-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="88dc0-136">See also</span></span>



<span data-ttu-id="88dc0-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="88dc0-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="88dc0-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="88dc0-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="88dc0-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="88dc0-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

