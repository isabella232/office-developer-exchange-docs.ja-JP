---
title: ItemClasses (ArrayOfItemClassType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 971784d1-6860-4833-bb26-0e930fa11c21
description: ItemClasses 要素には、会話の項目の現在のフォルダーのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。
ms.openlocfilehash: 62ea5b624025b3f012249afd1763e2b393ef5caa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832150"
---
# <a name="itemclasses-arrayofitemclasstype"></a><span data-ttu-id="85ec2-103">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="85ec2-103">ItemClasses (ArrayOfItemClassType)</span></span>

<span data-ttu-id="85ec2-104">**ItemClasses**要素には、会話の項目の現在のフォルダーのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="85ec2-104">The **ItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="85ec2-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="85ec2-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="85ec2-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="85ec2-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="85ec2-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="85ec2-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="85ec2-108">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="85ec2-108">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="85ec2-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="85ec2-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85ec2-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="85ec2-110">Attributes and elements</span></span>

<span data-ttu-id="85ec2-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="85ec2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85ec2-112">属性</span><span class="sxs-lookup"><span data-stu-id="85ec2-112">Attributes</span></span>

<span data-ttu-id="85ec2-113">なし。</span><span class="sxs-lookup"><span data-stu-id="85ec2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85ec2-114">子要素</span><span class="sxs-lookup"><span data-stu-id="85ec2-114">Child elements</span></span>

|<span data-ttu-id="85ec2-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="85ec2-115">**Element**</span></span>|<span data-ttu-id="85ec2-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="85ec2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ec2-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="85ec2-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="85ec2-118">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="85ec2-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85ec2-119">親要素</span><span class="sxs-lookup"><span data-stu-id="85ec2-119">Parent elements</span></span>

|<span data-ttu-id="85ec2-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="85ec2-120">**Element**</span></span>|<span data-ttu-id="85ec2-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="85ec2-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ec2-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="85ec2-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="85ec2-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="85ec2-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85ec2-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="85ec2-124">Text value</span></span>

<span data-ttu-id="85ec2-125">なし。</span><span class="sxs-lookup"><span data-stu-id="85ec2-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85ec2-126">備考</span><span class="sxs-lookup"><span data-stu-id="85ec2-126">Remarks</span></span>

<span data-ttu-id="85ec2-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="85ec2-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85ec2-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="85ec2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85ec2-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="85ec2-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85ec2-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="85ec2-130">Schema name</span></span>  <br/> |<span data-ttu-id="85ec2-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="85ec2-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="85ec2-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="85ec2-132">Validation file</span></span>  <br/> |<span data-ttu-id="85ec2-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85ec2-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85ec2-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="85ec2-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="85ec2-135">False</span><span class="sxs-lookup"><span data-stu-id="85ec2-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85ec2-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="85ec2-136">See also</span></span>



<span data-ttu-id="85ec2-137">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="85ec2-137">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="85ec2-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="85ec2-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="85ec2-139">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="85ec2-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

