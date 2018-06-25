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
description: GlobalFlagStatus 要素には、メールボックス内のすべての会話項目の集計のフラグの状態が含まれています。
ms.openlocfilehash: 0c560c065463b8b619f96ecef73d1120b216ca35
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831713"
---
# <a name="globalflagstatus"></a><span data-ttu-id="af52f-103">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="af52f-103">GlobalFlagStatus</span></span>

<span data-ttu-id="af52f-104">**GlobalFlagStatus**要素には、メールボックス内のすべての会話項目の集計のフラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af52f-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="af52f-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="af52f-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="af52f-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="af52f-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="af52f-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="af52f-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="af52f-108">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="af52f-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="af52f-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="af52f-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af52f-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af52f-110">Attributes and elements</span></span>

<span data-ttu-id="af52f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af52f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af52f-112">属性</span><span class="sxs-lookup"><span data-stu-id="af52f-112">Attributes</span></span>

<span data-ttu-id="af52f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="af52f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af52f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="af52f-114">Child elements</span></span>

<span data-ttu-id="af52f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="af52f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af52f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="af52f-116">Parent elements</span></span>

|<span data-ttu-id="af52f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="af52f-117">**Element**</span></span>|<span data-ttu-id="af52f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="af52f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af52f-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="af52f-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="af52f-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="af52f-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af52f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="af52f-121">Text value</span></span>

<span data-ttu-id="af52f-122">**GlobalFlagStatus**要素のテキスト値は、現在のフォルダー内の会話の項目の集計のフラグの状態です。</span><span class="sxs-lookup"><span data-stu-id="af52f-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="af52f-123">可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="af52f-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="af52f-124">**NotFlagged** - は、not のフラグが設定された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="af52f-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="af52f-125">**フラグ付き**では、フラグが設定された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="af52f-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="af52f-126">**完了**には、完了のフラグの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="af52f-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="af52f-127">備考</span><span class="sxs-lookup"><span data-stu-id="af52f-127">Remarks</span></span>

<span data-ttu-id="af52f-128">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="af52f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af52f-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="af52f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af52f-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="af52f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af52f-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af52f-131">Schema name</span></span>  <br/> |<span data-ttu-id="af52f-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="af52f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="af52f-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af52f-133">Validation file</span></span>  <br/> |<span data-ttu-id="af52f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af52f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af52f-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="af52f-135">Can be empty</span></span>  <br/> |<span data-ttu-id="af52f-136">False</span><span class="sxs-lookup"><span data-stu-id="af52f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af52f-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="af52f-137">See also</span></span>



<span data-ttu-id="af52f-138">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="af52f-138">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="af52f-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="af52f-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="af52f-140">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="af52f-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

