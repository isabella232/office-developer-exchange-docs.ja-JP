---
title: Enablealways Delete
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
description: Enablealways Delete 要素は、スレッド内のすべての新しいアイテムの削除を有効にするフラグを指定します。
ms.openlocfilehash: 14784d3a6ba52c76b64b81e15c0522d66d125cbf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526208"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="b6355-103">Enablealways Delete</span><span class="sxs-lookup"><span data-stu-id="b6355-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="b6355-104">**Enablealways delete**要素は、スレッド内のすべての新しいアイテムの削除を有効にするフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6355-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="b6355-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="b6355-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="b6355-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="b6355-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="b6355-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="b6355-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="b6355-108">Enablealways Delete</span><span class="sxs-lookup"><span data-stu-id="b6355-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="b6355-109">**xs: boolean**</span><span class="sxs-lookup"><span data-stu-id="b6355-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6355-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6355-110">Attributes and elements</span></span>

<span data-ttu-id="b6355-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6355-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6355-112">属性</span><span class="sxs-lookup"><span data-stu-id="b6355-112">Attributes</span></span>

<span data-ttu-id="b6355-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b6355-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6355-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b6355-114">Child elements</span></span>

<span data-ttu-id="b6355-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b6355-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6355-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b6355-116">Parent elements</span></span>

|<span data-ttu-id="b6355-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6355-117">**Element**</span></span>|<span data-ttu-id="b6355-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6355-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6355-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="b6355-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="b6355-120">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b6355-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b6355-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b6355-121">Text value</span></span>

<span data-ttu-id="b6355-122">**Enablealways delete**要素のテキスト値は、スレッド内のすべてのアイテムの削除を有効にする**場合は true**です。それ以外の場合は**false**。</span><span class="sxs-lookup"><span data-stu-id="b6355-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6355-123">注釈</span><span class="sxs-lookup"><span data-stu-id="b6355-123">Remarks</span></span>

<span data-ttu-id="b6355-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6355-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6355-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6355-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6355-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6355-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6355-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6355-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b6355-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6355-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6355-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6355-129">Validation File</span></span>  <br/> |<span data-ttu-id="b6355-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b6355-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6355-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b6355-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6355-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="b6355-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6355-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6355-133">See also</span></span>



[<span data-ttu-id="b6355-134">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="b6355-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

