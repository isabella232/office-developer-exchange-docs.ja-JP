---
title: UniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueUnreadSenders
api_type:
- schema
ms.assetid: eb7d1274-ce2e-4ef8-b47f-e911174aab0c
description: UniqueUnreadSenders 要素には、現在のフォルダーでこのスレッドで現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。 この要素は値の取得のみ可能です。
ms.openlocfilehash: 0e45362e88be4930b8bc2f641c1fb00cc63c0605
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458853"
---
# <a name="uniqueunreadsenders"></a><span data-ttu-id="c24db-104">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="c24db-104">UniqueUnreadSenders</span></span>

<span data-ttu-id="c24db-105">**UniqueUnreadSenders**要素には、現在のフォルダーでこのスレッドで現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c24db-105">The **UniqueUnreadSenders** element contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="c24db-106">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c24db-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="c24db-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="c24db-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="c24db-108">会話</span><span class="sxs-lookup"><span data-stu-id="c24db-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="c24db-109">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="c24db-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="c24db-110">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="c24db-110">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md)
  
```XML
<UniqueUnreadSenders>
   <String/>
</UniqueUnreadSenders>
```

 <span data-ttu-id="c24db-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c24db-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c24db-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c24db-112">Attributes and elements</span></span>

<span data-ttu-id="c24db-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c24db-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c24db-114">属性</span><span class="sxs-lookup"><span data-stu-id="c24db-114">Attributes</span></span>

<span data-ttu-id="c24db-115">なし。</span><span class="sxs-lookup"><span data-stu-id="c24db-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c24db-116">子要素</span><span class="sxs-lookup"><span data-stu-id="c24db-116">Child elements</span></span>

|<span data-ttu-id="c24db-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="c24db-117">**Element**</span></span>|<span data-ttu-id="c24db-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="c24db-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c24db-119">String</span><span class="sxs-lookup"><span data-stu-id="c24db-119">String</span></span>](string.md) <br/> |<span data-ttu-id="c24db-120">1つの会話の送信者を含みます。</span><span class="sxs-lookup"><span data-stu-id="c24db-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c24db-121">親要素</span><span class="sxs-lookup"><span data-stu-id="c24db-121">Parent elements</span></span>

|<span data-ttu-id="c24db-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="c24db-122">**Element**</span></span>|<span data-ttu-id="c24db-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="c24db-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c24db-124">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="c24db-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="c24db-125">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="c24db-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c24db-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c24db-126">Text value</span></span>

<span data-ttu-id="c24db-127">なし。</span><span class="sxs-lookup"><span data-stu-id="c24db-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c24db-128">注釈</span><span class="sxs-lookup"><span data-stu-id="c24db-128">Remarks</span></span>

<span data-ttu-id="c24db-129">この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c24db-129">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c24db-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c24db-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c24db-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="c24db-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c24db-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c24db-132">Schema name</span></span>  <br/> |<span data-ttu-id="c24db-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c24db-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c24db-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c24db-134">Validation file</span></span>  <br/> |<span data-ttu-id="c24db-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c24db-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c24db-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c24db-136">Can be empty</span></span>  <br/> |<span data-ttu-id="c24db-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="c24db-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c24db-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c24db-138">See also</span></span>



[<span data-ttu-id="c24db-139">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="c24db-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="c24db-140">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="c24db-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="c24db-141">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="c24db-141">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

