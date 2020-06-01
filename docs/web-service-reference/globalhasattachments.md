---
title: GlobalHasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalHasAttachments
api_type:
- schema
ms.assetid: 3d075e93-14bc-479d-957f-9b7873d1db39
description: GlobalHasAttachments 要素には、メールボックス内の少なくとも1つの会話アイテムに添付ファイルがあるかどうかを示す値が含まれています。
ms.openlocfilehash: e314e8e5c06ca7d7820b910c05b381765e88911f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459477"
---
# <a name="globalhasattachments"></a><span data-ttu-id="e4ca4-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="e4ca4-103">GlobalHasAttachments</span></span>

<span data-ttu-id="e4ca4-104">**Globalhasattachments**要素には、メールボックス内の少なくとも1つの会話アイテムに添付ファイルがあるかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="e4ca4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="e4ca4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="e4ca4-106">会話</span><span class="sxs-lookup"><span data-stu-id="e4ca4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="e4ca4-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e4ca4-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="e4ca4-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="e4ca4-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="e4ca4-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e4ca4-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4ca4-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e4ca4-110">Attributes and elements</span></span>

<span data-ttu-id="e4ca4-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4ca4-112">属性</span><span class="sxs-lookup"><span data-stu-id="e4ca4-112">Attributes</span></span>

<span data-ttu-id="e4ca4-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4ca4-114">子要素</span><span class="sxs-lookup"><span data-stu-id="e4ca4-114">Child elements</span></span>

<span data-ttu-id="e4ca4-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4ca4-116">親要素</span><span class="sxs-lookup"><span data-stu-id="e4ca4-116">Parent elements</span></span>

|<span data-ttu-id="e4ca4-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e4ca4-117">**Element**</span></span>|<span data-ttu-id="e4ca4-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4ca4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4ca4-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e4ca4-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e4ca4-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4ca4-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e4ca4-121">Text value</span></span>

<span data-ttu-id="e4ca4-122">**Globalhasattachments**要素の値は、メールボックス内の少なくとも1つの会話アイテムに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-122">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment.</span></span> <span data-ttu-id="e4ca4-123">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-123">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="e4ca4-124">値が**true**の場合は、スレッドに少なくとも1つの添付ファイルがあることを意味します。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-124">A value of **true** means that the conversation has at least one visible attachment.</span></span> <span data-ttu-id="e4ca4-125">値が**false**の場合、会話に添付ファイルがないか、または添付ファイルのみが含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-125">A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e4ca4-126">注釈</span><span class="sxs-lookup"><span data-stu-id="e4ca4-126">Remarks</span></span>

<span data-ttu-id="e4ca4-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4ca4-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e4ca4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4ca4-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4ca4-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4ca4-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4ca4-130">Schema name</span></span>  <br/> |<span data-ttu-id="e4ca4-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e4ca4-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4ca4-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4ca4-132">Validation file</span></span>  <br/> |<span data-ttu-id="e4ca4-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e4ca4-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4ca4-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e4ca4-134">Can be empty</span></span>  <br/> |<span data-ttu-id="e4ca4-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="e4ca4-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4ca4-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4ca4-136">See also</span></span>



[<span data-ttu-id="e4ca4-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="e4ca4-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="e4ca4-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="e4ca4-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="e4ca4-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="e4ca4-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

