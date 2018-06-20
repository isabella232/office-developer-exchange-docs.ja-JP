---
title: GlobalUniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueRecipients
api_type:
- schema
ms.assetid: 67379c1c-85d9-4b11-8f17-ad9d24904788
description: GlobalUniqueRecipients 要素には、メールボックス間で集計する対話の受信者のリストが含まれています。
ms.openlocfilehash: 5eb6e60d3ece8d8369f4603e36ffaaf72a3e459d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831742"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="6b1ab-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="6b1ab-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="6b1ab-104">**GlobalUniqueRecipients**要素には、メールボックス間で集計する対話の受信者のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="6b1ab-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="6b1ab-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="6b1ab-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="6b1ab-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="6b1ab-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6b1ab-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="6b1ab-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="6b1ab-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="6b1ab-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="6b1ab-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b1ab-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b1ab-110">Attributes and elements</span></span>

<span data-ttu-id="6b1ab-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b1ab-112">属性</span><span class="sxs-lookup"><span data-stu-id="6b1ab-112">Attributes</span></span>

<span data-ttu-id="6b1ab-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b1ab-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6b1ab-114">Child elements</span></span>

|<span data-ttu-id="6b1ab-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b1ab-115">**Element**</span></span>|<span data-ttu-id="6b1ab-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b1ab-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b1ab-117">String</span><span class="sxs-lookup"><span data-stu-id="6b1ab-117">String</span></span>](string.md) <br/> |<span data-ttu-id="6b1ab-118">会話の 1 つの受信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b1ab-119">親要素</span><span class="sxs-lookup"><span data-stu-id="6b1ab-119">Parent elements</span></span>

|<span data-ttu-id="6b1ab-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b1ab-120">**Element**</span></span>|<span data-ttu-id="6b1ab-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b1ab-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b1ab-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6b1ab-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6b1ab-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b1ab-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b1ab-124">Text value</span></span>

<span data-ttu-id="6b1ab-125">なし。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b1ab-126">備考</span><span class="sxs-lookup"><span data-stu-id="6b1ab-126">Remarks</span></span>

<span data-ttu-id="6b1ab-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b1ab-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="6b1ab-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b1ab-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="6b1ab-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b1ab-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b1ab-130">Schema name</span></span>  <br/> |<span data-ttu-id="6b1ab-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b1ab-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b1ab-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b1ab-132">Validation file</span></span>  <br/> |<span data-ttu-id="6b1ab-133">types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b1ab-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b1ab-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6b1ab-134">Can be empty</span></span>  <br/> |<span data-ttu-id="6b1ab-135">False</span><span class="sxs-lookup"><span data-stu-id="6b1ab-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b1ab-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b1ab-136">See also</span></span>



<span data-ttu-id="6b1ab-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="6b1ab-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="6b1ab-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="6b1ab-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="6b1ab-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="6b1ab-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

