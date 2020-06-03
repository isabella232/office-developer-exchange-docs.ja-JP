---
title: GlobalCategories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalCategories
api_type:
- schema
ms.assetid: 7a1d3f04-4ada-4a31-845e-f1f1ff6e136f
description: GlobalCategories 要素には、メールボックス内のすべての会話アイテムのカテゴリリストが含まれています。
ms.openlocfilehash: d608328f8adae56e140affdb36b38605d6f89486
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530121"
---
# <a name="globalcategories"></a><span data-ttu-id="b8244-103">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="b8244-103">GlobalCategories</span></span>

<span data-ttu-id="b8244-104">**Globalcategories**要素には、メールボックス内のすべての会話アイテムのカテゴリリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b8244-104">The **GlobalCategories** element contains the category list for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="b8244-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b8244-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="b8244-106">会話</span><span class="sxs-lookup"><span data-stu-id="b8244-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="b8244-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b8244-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="b8244-108">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="b8244-108">GlobalCategories</span></span>](globalcategories.md)
  
```XML
<GlobalCategories>
   <String/>
</GlobalCategories>
```

 <span data-ttu-id="b8244-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b8244-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8244-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8244-110">Attributes and elements</span></span>

<span data-ttu-id="b8244-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8244-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8244-112">属性</span><span class="sxs-lookup"><span data-stu-id="b8244-112">Attributes</span></span>

<span data-ttu-id="b8244-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b8244-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8244-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b8244-114">Child elements</span></span>

|<span data-ttu-id="b8244-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="b8244-115">**Element**</span></span>|<span data-ttu-id="b8244-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8244-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8244-117">String</span><span class="sxs-lookup"><span data-stu-id="b8244-117">String</span></span>](string.md) <br/> |<span data-ttu-id="b8244-118">1つのカテゴリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b8244-118">Contains a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8244-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b8244-119">Parent elements</span></span>

|<span data-ttu-id="b8244-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8244-120">**Element**</span></span>|<span data-ttu-id="b8244-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8244-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8244-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b8244-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b8244-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="b8244-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8244-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8244-124">Text value</span></span>

<span data-ttu-id="b8244-125">なし。</span><span class="sxs-lookup"><span data-stu-id="b8244-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8244-126">注釈</span><span class="sxs-lookup"><span data-stu-id="b8244-126">Remarks</span></span>

<span data-ttu-id="b8244-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b8244-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8244-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8244-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8244-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8244-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8244-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8244-130">Schema name</span></span>  <br/> |<span data-ttu-id="b8244-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b8244-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8244-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8244-132">Validation file</span></span>  <br/> |<span data-ttu-id="b8244-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b8244-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8244-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8244-134">Can be empty</span></span>  <br/> |<span data-ttu-id="b8244-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="b8244-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8244-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8244-136">See also</span></span>



[<span data-ttu-id="b8244-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="b8244-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="b8244-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="b8244-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="b8244-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="b8244-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

