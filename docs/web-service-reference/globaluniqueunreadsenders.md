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
description: GlobalUniqueUnreadSenders 要素は現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストを指定します。
ms.openlocfilehash: ae088577f5aac0c7c3ee9c11fde184b70ab12e64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831749"
---
# <a name="globaluniqueunreadsenders"></a><span data-ttu-id="3dd62-103">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="3dd62-103">GlobalUniqueUnreadSenders</span></span>

<span data-ttu-id="3dd62-104">**GlobalUniqueUnreadSenders**要素は現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dd62-104">The **GlobalUniqueUnreadSenders** element specifies a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="3dd62-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="3dd62-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="3dd62-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="3dd62-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="3dd62-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3dd62-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="3dd62-108">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="3dd62-108">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md)
  
```XML
<GlobalUniqueUnreadSenders>
   <String/>
</GlobalUniqueUnreadSenders>
```

 <span data-ttu-id="3dd62-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="3dd62-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dd62-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3dd62-110">Attributes and elements</span></span>

<span data-ttu-id="3dd62-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3dd62-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dd62-112">属性</span><span class="sxs-lookup"><span data-stu-id="3dd62-112">Attributes</span></span>

<span data-ttu-id="3dd62-113">なし。</span><span class="sxs-lookup"><span data-stu-id="3dd62-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dd62-114">子要素</span><span class="sxs-lookup"><span data-stu-id="3dd62-114">Child elements</span></span>

|<span data-ttu-id="3dd62-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="3dd62-115">**Element**</span></span>|<span data-ttu-id="3dd62-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="3dd62-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dd62-117">String</span><span class="sxs-lookup"><span data-stu-id="3dd62-117">String</span></span>](string.md) <br/> |<span data-ttu-id="3dd62-118">1 つの会話の送信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3dd62-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3dd62-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3dd62-119">Parent elements</span></span>

|<span data-ttu-id="3dd62-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="3dd62-120">**Element**</span></span>|<span data-ttu-id="3dd62-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3dd62-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dd62-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3dd62-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3dd62-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="3dd62-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3dd62-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3dd62-124">Text value</span></span>

<span data-ttu-id="3dd62-125">なし。</span><span class="sxs-lookup"><span data-stu-id="3dd62-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3dd62-126">備考</span><span class="sxs-lookup"><span data-stu-id="3dd62-126">Remarks</span></span>

<span data-ttu-id="3dd62-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3dd62-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dd62-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="3dd62-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dd62-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="3dd62-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3dd62-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3dd62-130">Schema name</span></span>  <br/> |<span data-ttu-id="3dd62-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3dd62-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3dd62-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3dd62-132">Validation file</span></span>  <br/> |<span data-ttu-id="3dd62-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3dd62-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3dd62-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3dd62-134">Can be empty</span></span>  <br/> |<span data-ttu-id="3dd62-135">False</span><span class="sxs-lookup"><span data-stu-id="3dd62-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dd62-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="3dd62-136">See also</span></span>



<span data-ttu-id="3dd62-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="3dd62-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="3dd62-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="3dd62-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="3dd62-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="3dd62-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

