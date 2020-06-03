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
description: GlobalUnreadCount 要素には、メールボックス内のすべての未開封の会話アイテムの数が含まれます。
ms.openlocfilehash: 976067078908523936769b2856712e3e6908f0c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530114"
---
# <a name="globalunreadcount"></a><span data-ttu-id="051dd-103">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="051dd-103">GlobalUnreadCount</span></span>

<span data-ttu-id="051dd-104">**GlobalUnreadCount**要素には、メールボックス内のすべての未開封の会話アイテムの数が含まれます。</span><span class="sxs-lookup"><span data-stu-id="051dd-104">The **GlobalUnreadCount** element contains a count of all the unread conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="051dd-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="051dd-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="051dd-106">会話</span><span class="sxs-lookup"><span data-stu-id="051dd-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="051dd-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="051dd-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="051dd-108">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="051dd-108">GlobalUnreadCount</span></span>](globalunreadcount.md)
  
```XML
<GlobalUnreadCount/>
```

 <span data-ttu-id="051dd-109">**xs: int**</span><span class="sxs-lookup"><span data-stu-id="051dd-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="051dd-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="051dd-110">Attributes and elements</span></span>

<span data-ttu-id="051dd-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="051dd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="051dd-112">属性</span><span class="sxs-lookup"><span data-stu-id="051dd-112">Attributes</span></span>

<span data-ttu-id="051dd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="051dd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="051dd-114">子要素</span><span class="sxs-lookup"><span data-stu-id="051dd-114">Child elements</span></span>

<span data-ttu-id="051dd-115">なし。</span><span class="sxs-lookup"><span data-stu-id="051dd-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="051dd-116">親要素</span><span class="sxs-lookup"><span data-stu-id="051dd-116">Parent elements</span></span>

|<span data-ttu-id="051dd-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="051dd-117">**Element**</span></span>|<span data-ttu-id="051dd-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="051dd-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="051dd-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="051dd-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="051dd-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="051dd-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="051dd-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="051dd-121">Text value</span></span>

<span data-ttu-id="051dd-122">**GlobalUnreadCount**要素のテキスト値は、メールボックス内のすべての未開封の会話アイテムの数を表す整数値です。</span><span class="sxs-lookup"><span data-stu-id="051dd-122">The text value of the **GlobalUnreadCount** element is an integer value that represents a count of all the unread conversation items in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="051dd-123">注釈</span><span class="sxs-lookup"><span data-stu-id="051dd-123">Remarks</span></span>

<span data-ttu-id="051dd-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="051dd-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="051dd-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="051dd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="051dd-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="051dd-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="051dd-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="051dd-127">Schema name</span></span>  <br/> |<span data-ttu-id="051dd-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="051dd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="051dd-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="051dd-129">Validation file</span></span>  <br/> |<span data-ttu-id="051dd-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="051dd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="051dd-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="051dd-131">Can be empty</span></span>  <br/> |<span data-ttu-id="051dd-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="051dd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="051dd-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="051dd-133">See also</span></span>



[<span data-ttu-id="051dd-134">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="051dd-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="051dd-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="051dd-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="051dd-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="051dd-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

