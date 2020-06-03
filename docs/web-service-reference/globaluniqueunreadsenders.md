---
title: GlobalUniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueUnreadSenders
api_type:
- schema
ms.assetid: 490abe30-7608-407a-923b-a4b3ddbca610
description: GlobalUniqueUnreadSenders 要素は、メールボックス内のすべてのフォルダーにわたって、この会話で現在未読のメッセージを送信したすべてのユーザーのリストを指定します。
ms.openlocfilehash: 5a26053158a262d65993dba4be90888ee97f2112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530819"
---
# <a name="globaluniqueunreadsenders"></a><span data-ttu-id="ac136-103">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ac136-103">GlobalUniqueUnreadSenders</span></span>

<span data-ttu-id="ac136-104">**GlobalUniqueUnreadSenders**要素は、メールボックス内のすべてのフォルダーにわたって、この会話で現在未読のメッセージを送信したすべてのユーザーのリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac136-104">The **GlobalUniqueUnreadSenders** element specifies a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="ac136-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="ac136-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="ac136-106">会話</span><span class="sxs-lookup"><span data-stu-id="ac136-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="ac136-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ac136-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="ac136-108">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ac136-108">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md)
  
```XML
<GlobalUniqueUnreadSenders>
   <String/>
</GlobalUniqueUnreadSenders>
```

 <span data-ttu-id="ac136-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="ac136-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac136-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ac136-110">Attributes and elements</span></span>

<span data-ttu-id="ac136-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac136-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac136-112">属性</span><span class="sxs-lookup"><span data-stu-id="ac136-112">Attributes</span></span>

<span data-ttu-id="ac136-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ac136-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac136-114">子要素</span><span class="sxs-lookup"><span data-stu-id="ac136-114">Child elements</span></span>

|<span data-ttu-id="ac136-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="ac136-115">**Element**</span></span>|<span data-ttu-id="ac136-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac136-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac136-117">String</span><span class="sxs-lookup"><span data-stu-id="ac136-117">String</span></span>](string.md) <br/> |<span data-ttu-id="ac136-118">1つの会話の送信者を含みます。</span><span class="sxs-lookup"><span data-stu-id="ac136-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac136-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ac136-119">Parent elements</span></span>

|<span data-ttu-id="ac136-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac136-120">**Element**</span></span>|<span data-ttu-id="ac136-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac136-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac136-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ac136-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ac136-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="ac136-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac136-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ac136-124">Text value</span></span>

<span data-ttu-id="ac136-125">なし。</span><span class="sxs-lookup"><span data-stu-id="ac136-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac136-126">注釈</span><span class="sxs-lookup"><span data-stu-id="ac136-126">Remarks</span></span>

<span data-ttu-id="ac136-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ac136-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac136-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ac136-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac136-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac136-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac136-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac136-130">Schema name</span></span>  <br/> |<span data-ttu-id="ac136-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ac136-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac136-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac136-132">Validation file</span></span>  <br/> |<span data-ttu-id="ac136-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ac136-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac136-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ac136-134">Can be empty</span></span>  <br/> |<span data-ttu-id="ac136-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="ac136-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac136-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac136-136">See also</span></span>



[<span data-ttu-id="ac136-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="ac136-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="ac136-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="ac136-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="ac136-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="ac136-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

