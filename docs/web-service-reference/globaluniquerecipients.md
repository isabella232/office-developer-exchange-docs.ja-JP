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
description: GlobalUniqueRecipients 要素には、メールボックス全体で集約された会話の受信者の一覧が含まれています。
ms.openlocfilehash: 3481c43b99f75a05a8e7fbe5a288e04708290d83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456039"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="b9435-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="b9435-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="b9435-104">**GlobalUniqueRecipients**要素には、メールボックス全体で集約された会話の受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9435-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="b9435-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b9435-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="b9435-106">会話</span><span class="sxs-lookup"><span data-stu-id="b9435-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="b9435-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b9435-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="b9435-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="b9435-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="b9435-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b9435-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9435-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b9435-110">Attributes and elements</span></span>

<span data-ttu-id="b9435-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9435-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9435-112">属性</span><span class="sxs-lookup"><span data-stu-id="b9435-112">Attributes</span></span>

<span data-ttu-id="b9435-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b9435-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9435-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b9435-114">Child elements</span></span>

|<span data-ttu-id="b9435-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="b9435-115">**Element**</span></span>|<span data-ttu-id="b9435-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9435-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9435-117">String</span><span class="sxs-lookup"><span data-stu-id="b9435-117">String</span></span>](string.md) <br/> |<span data-ttu-id="b9435-118">1つの会話の受信者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b9435-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9435-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b9435-119">Parent elements</span></span>

|<span data-ttu-id="b9435-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9435-120">**Element**</span></span>|<span data-ttu-id="b9435-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9435-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9435-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b9435-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b9435-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="b9435-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9435-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9435-124">Text value</span></span>

<span data-ttu-id="b9435-125">なし。</span><span class="sxs-lookup"><span data-stu-id="b9435-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9435-126">注釈</span><span class="sxs-lookup"><span data-stu-id="b9435-126">Remarks</span></span>

<span data-ttu-id="b9435-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b9435-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9435-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b9435-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9435-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9435-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9435-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9435-130">Schema name</span></span>  <br/> |<span data-ttu-id="b9435-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9435-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9435-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9435-132">Validation file</span></span>  <br/> |<span data-ttu-id="b9435-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b9435-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9435-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9435-134">Can be empty</span></span>  <br/> |<span data-ttu-id="b9435-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="b9435-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9435-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9435-136">See also</span></span>



[<span data-ttu-id="b9435-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="b9435-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="b9435-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="b9435-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="b9435-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="b9435-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

