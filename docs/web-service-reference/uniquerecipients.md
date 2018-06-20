---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: UniqueRecipients 要素には、特定のフォルダー内の会話の受信者のリストが含まれています。 この要素は、読み取り専用です。
ms.openlocfilehash: 710559e599c6cec1db371165f01187f8960024f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839806"
---
# <a name="uniquerecipients"></a><span data-ttu-id="e2b39-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e2b39-104">UniqueRecipients</span></span>

<span data-ttu-id="e2b39-105">**UniqueRecipients**要素には、特定のフォルダー内の会話の受信者のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2b39-105">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder.</span></span> <span data-ttu-id="e2b39-106">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e2b39-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="e2b39-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="e2b39-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="e2b39-108">スレッド</span><span class="sxs-lookup"><span data-stu-id="e2b39-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="e2b39-109">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e2b39-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="e2b39-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e2b39-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="e2b39-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e2b39-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2b39-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e2b39-112">Attributes and elements</span></span>

<span data-ttu-id="e2b39-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e2b39-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2b39-114">属性</span><span class="sxs-lookup"><span data-stu-id="e2b39-114">Attributes</span></span>

<span data-ttu-id="e2b39-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e2b39-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2b39-116">子要素</span><span class="sxs-lookup"><span data-stu-id="e2b39-116">Child elements</span></span>

|<span data-ttu-id="e2b39-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e2b39-117">**Element**</span></span>|<span data-ttu-id="e2b39-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2b39-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2b39-119">String</span><span class="sxs-lookup"><span data-stu-id="e2b39-119">String</span></span>](string.md) <br/> |<span data-ttu-id="e2b39-120">スレッドの一意の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="e2b39-120">Represents a unique recipient of a conversation.</span></span> <span data-ttu-id="e2b39-121">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e2b39-121">This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2b39-122">親要素</span><span class="sxs-lookup"><span data-stu-id="e2b39-122">Parent elements</span></span>

|<span data-ttu-id="e2b39-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="e2b39-123">**Element**</span></span>|<span data-ttu-id="e2b39-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2b39-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2b39-125">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e2b39-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e2b39-126">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="e2b39-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2b39-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e2b39-127">Text value</span></span>

<span data-ttu-id="e2b39-128">なし。</span><span class="sxs-lookup"><span data-stu-id="e2b39-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2b39-129">備考</span><span class="sxs-lookup"><span data-stu-id="e2b39-129">Remarks</span></span>

<span data-ttu-id="e2b39-130">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e2b39-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2b39-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="e2b39-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2b39-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="e2b39-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2b39-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e2b39-133">Schema name</span></span>  <br/> |<span data-ttu-id="e2b39-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e2b39-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2b39-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e2b39-135">Validation file</span></span>  <br/> |<span data-ttu-id="e2b39-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2b39-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2b39-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e2b39-137">Can be empty</span></span>  <br/> |<span data-ttu-id="e2b39-138">False</span><span class="sxs-lookup"><span data-stu-id="e2b39-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2b39-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="e2b39-139">See also</span></span>



<span data-ttu-id="e2b39-140">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e2b39-140">[FindConversation operation](findconversation-operation.md)</span></span>


[<span data-ttu-id="e2b39-141">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="e2b39-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

