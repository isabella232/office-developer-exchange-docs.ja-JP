---
title: 会話
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
description: 会話要素には、FindConversation 応答で返されるスレッドの配列が含まれています。
ms.openlocfilehash: 8af1023db51dd955c544422520ec5565f09f5372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463798"
---
# <a name="conversations"></a><span data-ttu-id="872cb-103">会話</span><span class="sxs-lookup"><span data-stu-id="872cb-103">Conversations</span></span>

<span data-ttu-id="872cb-104">**会話**要素には、 **findconversation**応答で返されるスレッドの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="872cb-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="872cb-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="872cb-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="872cb-106">会話</span><span class="sxs-lookup"><span data-stu-id="872cb-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="872cb-107">**ArrayOfConversationsType**</span><span class="sxs-lookup"><span data-stu-id="872cb-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="872cb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="872cb-108">Attributes and elements</span></span>

<span data-ttu-id="872cb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="872cb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="872cb-110">属性</span><span class="sxs-lookup"><span data-stu-id="872cb-110">Attributes</span></span>

<span data-ttu-id="872cb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="872cb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="872cb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="872cb-112">Child elements</span></span>

|<span data-ttu-id="872cb-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="872cb-113">**Element**</span></span>|<span data-ttu-id="872cb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="872cb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="872cb-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="872cb-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="872cb-116">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="872cb-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="872cb-117">親要素</span><span class="sxs-lookup"><span data-stu-id="872cb-117">Parent elements</span></span>

|<span data-ttu-id="872cb-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="872cb-118">**Element**</span></span>|<span data-ttu-id="872cb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="872cb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="872cb-120">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="872cb-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="872cb-121">**Findconversation**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="872cb-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="872cb-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="872cb-122">Text value</span></span>

<span data-ttu-id="872cb-123">なし。</span><span class="sxs-lookup"><span data-stu-id="872cb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="872cb-124">注釈</span><span class="sxs-lookup"><span data-stu-id="872cb-124">Remarks</span></span>

<span data-ttu-id="872cb-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="872cb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="872cb-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="872cb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="872cb-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="872cb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="872cb-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="872cb-128">Schema name</span></span>  <br/> |<span data-ttu-id="872cb-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="872cb-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="872cb-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="872cb-130">Validation file</span></span>  <br/> |<span data-ttu-id="872cb-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="872cb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="872cb-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="872cb-132">Can be empty</span></span>  <br/> |<span data-ttu-id="872cb-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="872cb-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="872cb-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="872cb-134">See also</span></span>



[<span data-ttu-id="872cb-135">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="872cb-135">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="872cb-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="872cb-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

