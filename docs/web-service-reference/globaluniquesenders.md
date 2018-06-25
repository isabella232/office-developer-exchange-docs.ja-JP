---
title: GlobalUniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueSenders
api_type:
- schema
ms.assetid: 6bd9e9cb-19c8-45af-b211-dfb8a6003b1b
description: GlobalUniqueSender 要素には、メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。
ms.openlocfilehash: 72dec056880c41ac9e79235dddb3c82102580a31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831751"
---
# <a name="globaluniquesenders"></a><span data-ttu-id="89e0c-103">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="89e0c-103">GlobalUniqueSenders</span></span>

<span data-ttu-id="89e0c-104">**GlobalUniqueSender**要素には、メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="89e0c-104">The **GlobalUniqueSender** element contains a list of all the senders of conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="89e0c-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="89e0c-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="89e0c-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="89e0c-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="89e0c-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="89e0c-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="89e0c-108">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="89e0c-108">GlobalUniqueSenders</span></span>](globaluniquesenders.md)
  
```XML
<GlobalUniqueSender>
   <String/>
</GlobalUniqueSender>
```

 <span data-ttu-id="89e0c-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="89e0c-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89e0c-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="89e0c-110">Attributes and elements</span></span>

<span data-ttu-id="89e0c-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89e0c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89e0c-112">属性</span><span class="sxs-lookup"><span data-stu-id="89e0c-112">Attributes</span></span>

<span data-ttu-id="89e0c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="89e0c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89e0c-114">子要素</span><span class="sxs-lookup"><span data-stu-id="89e0c-114">Child elements</span></span>

|<span data-ttu-id="89e0c-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="89e0c-115">**Element**</span></span>|<span data-ttu-id="89e0c-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="89e0c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89e0c-117">String</span><span class="sxs-lookup"><span data-stu-id="89e0c-117">String</span></span>](string.md) <br/> |<span data-ttu-id="89e0c-118">1 つの会話の送信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="89e0c-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89e0c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="89e0c-119">Parent elements</span></span>

|<span data-ttu-id="89e0c-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="89e0c-120">**Element**</span></span>|<span data-ttu-id="89e0c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="89e0c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89e0c-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="89e0c-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="89e0c-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="89e0c-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89e0c-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="89e0c-124">Text value</span></span>

<span data-ttu-id="89e0c-125">なし。</span><span class="sxs-lookup"><span data-stu-id="89e0c-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89e0c-126">備考</span><span class="sxs-lookup"><span data-stu-id="89e0c-126">Remarks</span></span>

<span data-ttu-id="89e0c-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="89e0c-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89e0c-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="89e0c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89e0c-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="89e0c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89e0c-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89e0c-130">Schema name</span></span>  <br/> |<span data-ttu-id="89e0c-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="89e0c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="89e0c-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89e0c-132">Validation file</span></span>  <br/> |<span data-ttu-id="89e0c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89e0c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89e0c-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="89e0c-134">Can be empty</span></span>  <br/> |<span data-ttu-id="89e0c-135">False</span><span class="sxs-lookup"><span data-stu-id="89e0c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89e0c-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="89e0c-136">See also</span></span>



<span data-ttu-id="89e0c-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="89e0c-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="89e0c-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="89e0c-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="89e0c-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="89e0c-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

