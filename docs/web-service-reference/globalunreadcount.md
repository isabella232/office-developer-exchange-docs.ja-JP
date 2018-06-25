---
title: GlobalUnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUnreadCount
api_type:
- schema
ms.assetid: 5e5ccf3e-2f95-4bf9-b915-8b7e59e807a5
description: GlobalUnreadCount 要素には、メールボックス内のすべての未読の会話項目の数が含まれています。
ms.openlocfilehash: fe001b70633198c0c1351e3c11c9542ed556a938
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831743"
---
# <a name="globalunreadcount"></a><span data-ttu-id="b9c5a-103">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="b9c5a-103">GlobalUnreadCount</span></span>

<span data-ttu-id="b9c5a-104">**GlobalUnreadCount**要素には、メールボックス内のすべての未読の会話項目の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-104">The **GlobalUnreadCount** element contains a count of all the unread conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="b9c5a-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b9c5a-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="b9c5a-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="b9c5a-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="b9c5a-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b9c5a-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="b9c5a-108">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="b9c5a-108">GlobalUnreadCount</span></span>](globalunreadcount.md)
  
```XML
<GlobalUnreadCount/>
```

 <span data-ttu-id="b9c5a-109">**xs:int**</span><span class="sxs-lookup"><span data-stu-id="b9c5a-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9c5a-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b9c5a-110">Attributes and elements</span></span>

<span data-ttu-id="b9c5a-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9c5a-112">属性</span><span class="sxs-lookup"><span data-stu-id="b9c5a-112">Attributes</span></span>

<span data-ttu-id="b9c5a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9c5a-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b9c5a-114">Child elements</span></span>

<span data-ttu-id="b9c5a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9c5a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b9c5a-116">Parent elements</span></span>

|<span data-ttu-id="b9c5a-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9c5a-117">**Element**</span></span>|<span data-ttu-id="b9c5a-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9c5a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9c5a-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b9c5a-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b9c5a-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9c5a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9c5a-121">Text value</span></span>

<span data-ttu-id="b9c5a-122">**GlobalUnreadCount**要素のテキスト値は、メールボックス内のすべての未読の会話項目の数を表す整数値です。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-122">The text value of the **GlobalUnreadCount** element is an integer value that represents a count of all the unread conversation items in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b9c5a-123">備考</span><span class="sxs-lookup"><span data-stu-id="b9c5a-123">Remarks</span></span>

<span data-ttu-id="b9c5a-124">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9c5a-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="b9c5a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9c5a-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="b9c5a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9c5a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9c5a-127">Schema name</span></span>  <br/> |<span data-ttu-id="b9c5a-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b9c5a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9c5a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9c5a-129">Validation file</span></span>  <br/> |<span data-ttu-id="b9c5a-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b9c5a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9c5a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-131">Can be empty</span></span>  <br/> |<span data-ttu-id="b9c5a-132">False</span><span class="sxs-lookup"><span data-stu-id="b9c5a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9c5a-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9c5a-133">See also</span></span>



<span data-ttu-id="b9c5a-134">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="b9c5a-134">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="b9c5a-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="b9c5a-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="b9c5a-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="b9c5a-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

