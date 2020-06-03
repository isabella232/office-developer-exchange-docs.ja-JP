---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: DeleteType 要素は、スレッド内のアイテムが削除される方法を示します。
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442634"
---
# <a name="deletetype"></a><span data-ttu-id="922c9-103">DeleteType</span><span class="sxs-lookup"><span data-stu-id="922c9-103">DeleteType</span></span>

<span data-ttu-id="922c9-104">**Deletetype**要素は、スレッド内のアイテムが削除される方法を示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="922c9-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="922c9-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="922c9-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="922c9-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="922c9-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="922c9-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="922c9-108">DeleteType</span><span class="sxs-lookup"><span data-stu-id="922c9-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="922c9-109">**DisposalType**</span><span class="sxs-lookup"><span data-stu-id="922c9-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="922c9-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="922c9-110">Attributes and elements</span></span>

<span data-ttu-id="922c9-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="922c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="922c9-112">属性</span><span class="sxs-lookup"><span data-stu-id="922c9-112">Attributes</span></span>

<span data-ttu-id="922c9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="922c9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="922c9-114">子要素</span><span class="sxs-lookup"><span data-stu-id="922c9-114">Child elements</span></span>

<span data-ttu-id="922c9-115">なし。</span><span class="sxs-lookup"><span data-stu-id="922c9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="922c9-116">親要素</span><span class="sxs-lookup"><span data-stu-id="922c9-116">Parent elements</span></span>

|<span data-ttu-id="922c9-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="922c9-117">**Element**</span></span>|<span data-ttu-id="922c9-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="922c9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="922c9-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="922c9-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="922c9-120">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="922c9-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="922c9-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="922c9-121">Text value</span></span>

<span data-ttu-id="922c9-122">**Deletetype**要素のテキスト値は、スレッド内のアイテムが削除される方法を示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="922c9-123">可能なテキスト値を次に示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="922c9-124">ハード削除-会話内のアイテムがメールボックスデータベースから完全に削除されることを示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="922c9-125">MoveToDeleteItems-スレッド内のアイテムが [削除済みアイテム] フォルダーに移動されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="922c9-126">SoftDelete-メッセージの収集が有効になっている場合に、スレッド内のアイテムが収集に移動されることを示します。</span><span class="sxs-lookup"><span data-stu-id="922c9-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="922c9-127">注釈</span><span class="sxs-lookup"><span data-stu-id="922c9-127">Remarks</span></span>

<span data-ttu-id="922c9-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="922c9-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="922c9-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="922c9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="922c9-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="922c9-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="922c9-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="922c9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="922c9-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="922c9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="922c9-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="922c9-133">Validation File</span></span>  <br/> |<span data-ttu-id="922c9-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="922c9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="922c9-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="922c9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="922c9-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="922c9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="922c9-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="922c9-137">See also</span></span>

- [<span data-ttu-id="922c9-138">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="922c9-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="922c9-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="922c9-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

