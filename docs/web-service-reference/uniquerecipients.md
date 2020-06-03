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
description: UniqueRecipients 要素には、特定のフォルダー内のスレッドの受信者の一覧が含まれています。 この要素は値の取得のみ可能です。
ms.openlocfilehash: d7f6b0aa01aceb6a251fb0c46d89b34cad260acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530727"
---
# <a name="uniquerecipients"></a><span data-ttu-id="f4715-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="f4715-104">UniqueRecipients</span></span>

<span data-ttu-id="f4715-105">**UniqueRecipients**要素には、特定のフォルダー内のスレッドの受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4715-105">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder.</span></span> <span data-ttu-id="f4715-106">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f4715-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="f4715-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="f4715-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f4715-108">会話</span><span class="sxs-lookup"><span data-stu-id="f4715-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f4715-109">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f4715-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="f4715-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="f4715-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="f4715-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="f4715-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4715-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f4715-112">Attributes and elements</span></span>

<span data-ttu-id="f4715-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4715-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4715-114">属性</span><span class="sxs-lookup"><span data-stu-id="f4715-114">Attributes</span></span>

<span data-ttu-id="f4715-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f4715-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4715-116">子要素</span><span class="sxs-lookup"><span data-stu-id="f4715-116">Child elements</span></span>

|<span data-ttu-id="f4715-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="f4715-117">**Element**</span></span>|<span data-ttu-id="f4715-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4715-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4715-119">String</span><span class="sxs-lookup"><span data-stu-id="f4715-119">String</span></span>](string.md) <br/> |<span data-ttu-id="f4715-120">会話の一意の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="f4715-120">Represents a unique recipient of a conversation.</span></span> <span data-ttu-id="f4715-121">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f4715-121">This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4715-122">親要素</span><span class="sxs-lookup"><span data-stu-id="f4715-122">Parent elements</span></span>

|<span data-ttu-id="f4715-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4715-123">**Element**</span></span>|<span data-ttu-id="f4715-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4715-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4715-125">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f4715-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f4715-126">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="f4715-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4715-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f4715-127">Text value</span></span>

<span data-ttu-id="f4715-128">なし。</span><span class="sxs-lookup"><span data-stu-id="f4715-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4715-129">注釈</span><span class="sxs-lookup"><span data-stu-id="f4715-129">Remarks</span></span>

<span data-ttu-id="f4715-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f4715-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4715-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f4715-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4715-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4715-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4715-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4715-133">Schema name</span></span>  <br/> |<span data-ttu-id="f4715-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f4715-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4715-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4715-135">Validation file</span></span>  <br/> |<span data-ttu-id="f4715-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f4715-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4715-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f4715-137">Can be empty</span></span>  <br/> |<span data-ttu-id="f4715-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="f4715-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4715-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4715-139">See also</span></span>



[<span data-ttu-id="f4715-140">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="f4715-140">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="f4715-141">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="f4715-141">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

