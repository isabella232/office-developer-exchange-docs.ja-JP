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
description: GlobalHasAttachments 要素には、メールボックス内の少なくとも 1 つのテーマのアイテムに添付ファイルがあるかどうかを示す値が含まれています。
ms.openlocfilehash: 85443c45f611a2f4bff392ffecb26029564d7558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831715"
---
# <a name="globalhasattachments"></a><span data-ttu-id="47b27-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="47b27-103">GlobalHasAttachments</span></span>

<span data-ttu-id="47b27-104">**GlobalHasAttachments**要素には、メールボックス内の少なくとも 1 つのテーマのアイテムに添付ファイルがあるかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47b27-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="47b27-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="47b27-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="47b27-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="47b27-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="47b27-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="47b27-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="47b27-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="47b27-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="47b27-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="47b27-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47b27-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="47b27-110">Attributes and elements</span></span>

<span data-ttu-id="47b27-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="47b27-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47b27-112">属性</span><span class="sxs-lookup"><span data-stu-id="47b27-112">Attributes</span></span>

<span data-ttu-id="47b27-113">なし。</span><span class="sxs-lookup"><span data-stu-id="47b27-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47b27-114">子要素</span><span class="sxs-lookup"><span data-stu-id="47b27-114">Child elements</span></span>

<span data-ttu-id="47b27-115">なし。</span><span class="sxs-lookup"><span data-stu-id="47b27-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47b27-116">親要素</span><span class="sxs-lookup"><span data-stu-id="47b27-116">Parent elements</span></span>

|<span data-ttu-id="47b27-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="47b27-117">**Element**</span></span>|<span data-ttu-id="47b27-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="47b27-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47b27-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="47b27-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="47b27-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="47b27-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47b27-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="47b27-121">Text value</span></span>

<span data-ttu-id="47b27-122">**GlobalHasAttachments**要素の値は、メールボックス内の少なくとも 1 つのテーマのアイテムに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47b27-122">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment.</span></span> <span data-ttu-id="47b27-123">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="47b27-123">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="47b27-124">**True**の場合は、会話が表示されている 1 つ以上の添付ファイルを持っているを意味します。</span><span class="sxs-lookup"><span data-stu-id="47b27-124">A value of **true** means that the conversation has at least one visible attachment.</span></span> <span data-ttu-id="47b27-125">**False**の値は、その会話が添付ファイルがないか添付ファイルを非表示にのみを意味します。</span><span class="sxs-lookup"><span data-stu-id="47b27-125">A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="47b27-126">備考</span><span class="sxs-lookup"><span data-stu-id="47b27-126">Remarks</span></span>

<span data-ttu-id="47b27-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="47b27-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47b27-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="47b27-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47b27-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="47b27-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47b27-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="47b27-130">Schema name</span></span>  <br/> |<span data-ttu-id="47b27-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="47b27-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="47b27-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="47b27-132">Validation file</span></span>  <br/> |<span data-ttu-id="47b27-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47b27-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47b27-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="47b27-134">Can be empty</span></span>  <br/> |<span data-ttu-id="47b27-135">False</span><span class="sxs-lookup"><span data-stu-id="47b27-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47b27-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="47b27-136">See also</span></span>



<span data-ttu-id="47b27-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="47b27-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="47b27-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="47b27-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="47b27-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="47b27-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

