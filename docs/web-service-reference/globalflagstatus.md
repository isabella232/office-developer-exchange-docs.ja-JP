---
title: GlobalFlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalFlagStatus
api_type:
- schema
ms.assetid: 3ba300f3-3355-4cab-9e77-0dcc2902e712
description: GlobalFlagStatus 要素には、メールボックス内のすべての会話アイテムの集約フラグの状態が含まれています。
ms.openlocfilehash: f9984a1bb7e8205a98dd3ef91f841b48a7ab9389
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459505"
---
# <a name="globalflagstatus"></a><span data-ttu-id="6e2ab-103">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="6e2ab-103">GlobalFlagStatus</span></span>

<span data-ttu-id="6e2ab-104">**Globalflagstatus**要素には、メールボックス内のすべての会話アイテムの集約フラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="6e2ab-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="6e2ab-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="6e2ab-106">会話</span><span class="sxs-lookup"><span data-stu-id="6e2ab-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="6e2ab-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6e2ab-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="6e2ab-108">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="6e2ab-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="6e2ab-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="6e2ab-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e2ab-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6e2ab-110">Attributes and elements</span></span>

<span data-ttu-id="6e2ab-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e2ab-112">属性</span><span class="sxs-lookup"><span data-stu-id="6e2ab-112">Attributes</span></span>

<span data-ttu-id="6e2ab-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e2ab-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6e2ab-114">Child elements</span></span>

<span data-ttu-id="6e2ab-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e2ab-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6e2ab-116">Parent elements</span></span>

|<span data-ttu-id="6e2ab-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e2ab-117">**Element**</span></span>|<span data-ttu-id="6e2ab-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e2ab-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e2ab-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6e2ab-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6e2ab-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e2ab-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6e2ab-121">Text value</span></span>

<span data-ttu-id="6e2ab-122">**Globalflagstatus**要素のテキスト値は、現在のフォルダー内のスレッドアイテムの集計フラグの状態です。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="6e2ab-123">可能なテキスト値を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="6e2ab-124">**Notflagged**付き-フラグなしの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="6e2ab-125">**フラグ付き**-フラグ付きの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="6e2ab-126">**Complete** -完全なフラグの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="6e2ab-127">注釈</span><span class="sxs-lookup"><span data-stu-id="6e2ab-127">Remarks</span></span>

<span data-ttu-id="6e2ab-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e2ab-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6e2ab-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e2ab-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e2ab-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e2ab-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e2ab-131">Schema name</span></span>  <br/> |<span data-ttu-id="6e2ab-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6e2ab-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e2ab-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e2ab-133">Validation file</span></span>  <br/> |<span data-ttu-id="6e2ab-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6e2ab-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e2ab-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6e2ab-135">Can be empty</span></span>  <br/> |<span data-ttu-id="6e2ab-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6e2ab-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e2ab-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e2ab-137">See also</span></span>



[<span data-ttu-id="6e2ab-138">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="6e2ab-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="6e2ab-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="6e2ab-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="6e2ab-140">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="6e2ab-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

