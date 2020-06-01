---
title: ItemClasses (ArrayOfItemClassType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 971784d1-6860-4833-bb26-0e930fa11c21
description: ItemClasses 要素には、現在のフォルダー内の会話アイテムのすべてのアイテムクラスを表す item クラスのリストが含まれています。
ms.openlocfilehash: 39118bf845429bb198874ae4e6b424c6339b1964
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467299"
---
# <a name="itemclasses-arrayofitemclasstype"></a><span data-ttu-id="a4592-103">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="a4592-103">ItemClasses (ArrayOfItemClassType)</span></span>

<span data-ttu-id="a4592-104">**Itemclasses**要素には、現在のフォルダー内の会話アイテムのすべてのアイテムクラスを表す item クラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4592-104">The **ItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="a4592-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="a4592-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="a4592-106">会話</span><span class="sxs-lookup"><span data-stu-id="a4592-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="a4592-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a4592-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="a4592-108">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="a4592-108">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="a4592-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="a4592-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4592-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a4592-110">Attributes and elements</span></span>

<span data-ttu-id="a4592-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4592-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4592-112">属性</span><span class="sxs-lookup"><span data-stu-id="a4592-112">Attributes</span></span>

<span data-ttu-id="a4592-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a4592-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4592-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a4592-114">Child elements</span></span>

|<span data-ttu-id="a4592-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="a4592-115">**Element**</span></span>|<span data-ttu-id="a4592-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4592-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4592-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="a4592-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="a4592-118">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="a4592-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4592-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a4592-119">Parent elements</span></span>

|<span data-ttu-id="a4592-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4592-120">**Element**</span></span>|<span data-ttu-id="a4592-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4592-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4592-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a4592-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="a4592-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="a4592-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4592-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4592-124">Text value</span></span>

<span data-ttu-id="a4592-125">なし。</span><span class="sxs-lookup"><span data-stu-id="a4592-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a4592-126">注釈</span><span class="sxs-lookup"><span data-stu-id="a4592-126">Remarks</span></span>

<span data-ttu-id="a4592-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a4592-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4592-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a4592-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4592-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a4592-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4592-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4592-130">Schema name</span></span>  <br/> |<span data-ttu-id="a4592-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a4592-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4592-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4592-132">Validation file</span></span>  <br/> |<span data-ttu-id="a4592-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a4592-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4592-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4592-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4592-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="a4592-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4592-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4592-136">See also</span></span>



[<span data-ttu-id="a4592-137">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="a4592-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="a4592-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="a4592-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="a4592-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="a4592-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

