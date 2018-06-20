---
title: GlobalMessageCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalMessageCount
api_type:
- schema
ms.assetid: e2ac4677-9645-4a1e-911c-17a5a08e2b21
description: GlobalMessageCount 要素には、メールボックス内の会話のアイテムの合計数が含まれています。
ms.openlocfilehash: 2dd871c1614bd537aeb7e7bf362b56adae7e4b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831741"
---
# <a name="globalmessagecount"></a><span data-ttu-id="92515-103">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="92515-103">GlobalMessageCount</span></span>

<span data-ttu-id="92515-104">**GlobalMessageCount**要素には、メールボックス内の会話のアイテムの合計数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92515-104">The **GlobalMessageCount** element contains the total number of conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="92515-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="92515-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="92515-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="92515-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="92515-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="92515-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="92515-108">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="92515-108">GlobalMessageCount</span></span>](globalmessagecount.md)
  
```XML
<GlobalMessageCount/>
```

 <span data-ttu-id="92515-109">**xs:int**</span><span class="sxs-lookup"><span data-stu-id="92515-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92515-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="92515-110">Attributes and elements</span></span>

<span data-ttu-id="92515-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92515-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92515-112">属性</span><span class="sxs-lookup"><span data-stu-id="92515-112">Attributes</span></span>

<span data-ttu-id="92515-113">なし。</span><span class="sxs-lookup"><span data-stu-id="92515-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92515-114">子要素</span><span class="sxs-lookup"><span data-stu-id="92515-114">Child elements</span></span>

<span data-ttu-id="92515-115">なし。</span><span class="sxs-lookup"><span data-stu-id="92515-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92515-116">親要素</span><span class="sxs-lookup"><span data-stu-id="92515-116">Parent elements</span></span>

|<span data-ttu-id="92515-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="92515-117">**Element**</span></span>|<span data-ttu-id="92515-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="92515-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92515-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="92515-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="92515-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="92515-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92515-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="92515-121">Text value</span></span>

<span data-ttu-id="92515-122">**GlobalMessageCount**要素のテキスト値は、メールボックス内の会話のアイテムの合計数です。</span><span class="sxs-lookup"><span data-stu-id="92515-122">The text value of the **GlobalMessageCount** element is the total number of conversation items in a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="92515-123">備考</span><span class="sxs-lookup"><span data-stu-id="92515-123">Remarks</span></span>

<span data-ttu-id="92515-124">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="92515-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92515-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="92515-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92515-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="92515-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92515-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92515-127">Schema name</span></span>  <br/> |<span data-ttu-id="92515-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="92515-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="92515-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92515-129">Validation file</span></span>  <br/> |<span data-ttu-id="92515-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92515-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92515-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="92515-131">Can be empty</span></span>  <br/> |<span data-ttu-id="92515-132">False</span><span class="sxs-lookup"><span data-stu-id="92515-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92515-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="92515-133">See also</span></span>



<span data-ttu-id="92515-134">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="92515-134">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="92515-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="92515-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="92515-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="92515-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

