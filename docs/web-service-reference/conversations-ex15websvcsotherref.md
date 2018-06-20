---
title: スレッド
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversations
api_type:
- schema
ms.assetid: 1d18f98c-6457-45e9-a934-32da20885ac6
description: 会話の要素には、FindConversation の応答で返される会話の配列が含まれています。
ms.openlocfilehash: cd36364bd975d1464af9a1114c64c29543b4ec47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759769"
---
# <a name="conversations"></a><span data-ttu-id="fb874-103">スレッド</span><span class="sxs-lookup"><span data-stu-id="fb874-103">Conversations</span></span>

<span data-ttu-id="fb874-104">**会話**の要素には、 **FindConversation**の応答で返される会話の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb874-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="fb874-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="fb874-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="fb874-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="fb874-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="fb874-107">**ArrayOfConversationsType**</span><span class="sxs-lookup"><span data-stu-id="fb874-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb874-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb874-108">Attributes and elements</span></span>

<span data-ttu-id="fb874-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb874-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb874-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb874-110">Attributes</span></span>

<span data-ttu-id="fb874-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fb874-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb874-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fb874-112">Child elements</span></span>

|<span data-ttu-id="fb874-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb874-113">**Element**</span></span>|<span data-ttu-id="fb874-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb874-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb874-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="fb874-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="fb874-116">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="fb874-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb874-117">親要素</span><span class="sxs-lookup"><span data-stu-id="fb874-117">Parent elements</span></span>

|<span data-ttu-id="fb874-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb874-118">**Element**</span></span>|<span data-ttu-id="fb874-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb874-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb874-120">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="fb874-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="fb874-121">**FindConversation**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="fb874-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb874-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fb874-122">Text value</span></span>

<span data-ttu-id="fb874-123">なし。</span><span class="sxs-lookup"><span data-stu-id="fb874-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb874-124">備考</span><span class="sxs-lookup"><span data-stu-id="fb874-124">Remarks</span></span>

<span data-ttu-id="fb874-125">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fb874-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb874-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb874-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb874-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb874-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb874-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb874-128">Schema name</span></span>  <br/> |<span data-ttu-id="fb874-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb874-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb874-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb874-130">Validation file</span></span>  <br/> |<span data-ttu-id="fb874-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb874-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb874-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb874-132">Can be empty</span></span>  <br/> |<span data-ttu-id="fb874-133">False</span><span class="sxs-lookup"><span data-stu-id="fb874-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb874-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb874-134">See also</span></span>



<span data-ttu-id="fb874-135">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="fb874-135">[FindConversation operation](findconversation-operation.md)</span></span>


[<span data-ttu-id="fb874-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="fb874-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

