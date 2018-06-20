---
title: EnableAlwaysDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EnableAlwaysDelete
api_type:
- schema
ms.assetid: 7753aec5-3f93-4aeb-a28e-8b9b42ca7f9b
description: EnableAlwaysDelete 要素は、会話内のすべての新しいアイテムの削除を有効にするフラグを指定します。
ms.openlocfilehash: f86765c641604afbf13ac962f4b34fbd8de56200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760278"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="e1a38-103">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="e1a38-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="e1a38-104">**EnableAlwaysDelete**要素は、会話内のすべての新しいアイテムの削除を有効にするフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a38-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="e1a38-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e1a38-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="e1a38-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="e1a38-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="e1a38-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="e1a38-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="e1a38-108">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="e1a38-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="e1a38-109">**xs:boolean**</span><span class="sxs-lookup"><span data-stu-id="e1a38-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1a38-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e1a38-110">Attributes and elements</span></span>

<span data-ttu-id="e1a38-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1a38-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1a38-112">属性</span><span class="sxs-lookup"><span data-stu-id="e1a38-112">Attributes</span></span>

<span data-ttu-id="e1a38-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e1a38-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1a38-114">子要素</span><span class="sxs-lookup"><span data-stu-id="e1a38-114">Child elements</span></span>

<span data-ttu-id="e1a38-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e1a38-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1a38-116">親要素</span><span class="sxs-lookup"><span data-stu-id="e1a38-116">Parent elements</span></span>

|<span data-ttu-id="e1a38-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1a38-117">**Element**</span></span>|<span data-ttu-id="e1a38-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1a38-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1a38-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="e1a38-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e1a38-120">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1a38-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1a38-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e1a38-121">Text value</span></span>

<span data-ttu-id="e1a38-122">**EnableAlwaysDelete**要素のテキスト値が**true**の通信でのすべての項目の削除を有効にするにはそれ以外の場合、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="e1a38-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1a38-123">備考</span><span class="sxs-lookup"><span data-stu-id="e1a38-123">Remarks</span></span>

<span data-ttu-id="e1a38-124">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e1a38-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1a38-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="e1a38-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1a38-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="e1a38-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1a38-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1a38-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e1a38-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e1a38-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1a38-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1a38-129">Validation File</span></span>  <br/> |<span data-ttu-id="e1a38-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1a38-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1a38-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e1a38-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1a38-132">False</span><span class="sxs-lookup"><span data-stu-id="e1a38-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1a38-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1a38-133">See also</span></span>



[<span data-ttu-id="e1a38-134">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="e1a38-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

