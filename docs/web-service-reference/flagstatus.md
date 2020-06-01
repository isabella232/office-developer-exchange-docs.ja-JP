---
title: FlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlagStatus
api_type:
- schema
ms.assetid: d5907ec5-3a60-4d83-bf85-406c54f95eb7
description: FlagStatus 要素には、現在のフォルダー内のスレッドアイテムの集約フラグの状態が含まれています。
ms.openlocfilehash: e65849c4909292c07450f8578fe7a7065c98ab44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466214"
---
# <a name="flagstatus"></a><span data-ttu-id="6bee7-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="6bee7-103">FlagStatus</span></span>

<span data-ttu-id="6bee7-104">**Flagstatus**要素には、現在のフォルダー内のスレッドアイテムの集約フラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6bee7-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="6bee7-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="6bee7-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="6bee7-106">会話</span><span class="sxs-lookup"><span data-stu-id="6bee7-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="6bee7-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6bee7-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="6bee7-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="6bee7-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="6bee7-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="6bee7-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bee7-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6bee7-110">Attributes and elements</span></span>

<span data-ttu-id="6bee7-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bee7-112">属性</span><span class="sxs-lookup"><span data-stu-id="6bee7-112">Attributes</span></span>

<span data-ttu-id="6bee7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6bee7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bee7-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6bee7-114">Child elements</span></span>

<span data-ttu-id="6bee7-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6bee7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bee7-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6bee7-116">Parent elements</span></span>

|<span data-ttu-id="6bee7-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6bee7-117">**Element**</span></span>|<span data-ttu-id="6bee7-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6bee7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bee7-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6bee7-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6bee7-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bee7-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6bee7-121">Text value</span></span>

<span data-ttu-id="6bee7-122">**Flagstatus**要素のテキスト値は、現在のフォルダー内のスレッドアイテムの集計フラグの状態です。</span><span class="sxs-lookup"><span data-stu-id="6bee7-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="6bee7-123">可能なテキスト値を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="6bee7-124">**Notflagged**付き-フラグなしの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="6bee7-125">**フラグ付き**-フラグ付きの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="6bee7-126">**Complete** -完全なフラグの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6bee7-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="6bee7-127">注釈</span><span class="sxs-lookup"><span data-stu-id="6bee7-127">Remarks</span></span>

<span data-ttu-id="6bee7-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6bee7-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bee7-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6bee7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bee7-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6bee7-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6bee7-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6bee7-131">Schema name</span></span>  <br/> |<span data-ttu-id="6bee7-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6bee7-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6bee7-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6bee7-133">Validation file</span></span>  <br/> |<span data-ttu-id="6bee7-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6bee7-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6bee7-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6bee7-135">Can be empty</span></span>  <br/> |<span data-ttu-id="6bee7-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6bee7-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bee7-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6bee7-137">See also</span></span>



[<span data-ttu-id="6bee7-138">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="6bee7-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="6bee7-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="6bee7-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="6bee7-140">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="6bee7-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

