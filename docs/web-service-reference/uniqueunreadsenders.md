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
description: UniqueUnreadSenders 要素には現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。 この要素は、読み取り専用です。
ms.openlocfilehash: d1f5593f6b86745aa27d86e9d25487f5855cb0cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839799"
---
# <a name="uniqueunreadsenders"></a><span data-ttu-id="772d2-104">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="772d2-104">UniqueUnreadSenders</span></span>

<span data-ttu-id="772d2-105">**UniqueUnreadSenders**要素には現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="772d2-105">The **UniqueUnreadSenders** element contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="772d2-106">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="772d2-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="772d2-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="772d2-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="772d2-108">スレッド</span><span class="sxs-lookup"><span data-stu-id="772d2-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="772d2-109">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="772d2-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="772d2-110">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="772d2-110">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md)
  
```XML
<UniqueUnreadSenders>
   <String/>
</UniqueUnreadSenders>
```

 <span data-ttu-id="772d2-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="772d2-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="772d2-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="772d2-112">Attributes and elements</span></span>

<span data-ttu-id="772d2-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="772d2-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="772d2-114">属性</span><span class="sxs-lookup"><span data-stu-id="772d2-114">Attributes</span></span>

<span data-ttu-id="772d2-115">なし。</span><span class="sxs-lookup"><span data-stu-id="772d2-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="772d2-116">子要素</span><span class="sxs-lookup"><span data-stu-id="772d2-116">Child elements</span></span>

|<span data-ttu-id="772d2-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="772d2-117">**Element**</span></span>|<span data-ttu-id="772d2-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="772d2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="772d2-119">String</span><span class="sxs-lookup"><span data-stu-id="772d2-119">String</span></span>](string.md) <br/> |<span data-ttu-id="772d2-120">1 つの会話の送信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="772d2-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="772d2-121">親要素</span><span class="sxs-lookup"><span data-stu-id="772d2-121">Parent elements</span></span>

|<span data-ttu-id="772d2-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="772d2-122">**Element**</span></span>|<span data-ttu-id="772d2-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="772d2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="772d2-124">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="772d2-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="772d2-125">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="772d2-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="772d2-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="772d2-126">Text value</span></span>

<span data-ttu-id="772d2-127">なし。</span><span class="sxs-lookup"><span data-stu-id="772d2-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="772d2-128">備考</span><span class="sxs-lookup"><span data-stu-id="772d2-128">Remarks</span></span>

<span data-ttu-id="772d2-129">この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="772d2-129">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="772d2-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="772d2-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="772d2-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="772d2-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="772d2-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="772d2-132">Schema name</span></span>  <br/> |<span data-ttu-id="772d2-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="772d2-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="772d2-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="772d2-134">Validation file</span></span>  <br/> |<span data-ttu-id="772d2-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="772d2-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="772d2-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="772d2-136">Can be empty</span></span>  <br/> |<span data-ttu-id="772d2-137">False</span><span class="sxs-lookup"><span data-stu-id="772d2-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="772d2-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="772d2-138">See also</span></span>



<span data-ttu-id="772d2-139">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="772d2-139">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="772d2-140">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="772d2-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="772d2-141">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="772d2-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

