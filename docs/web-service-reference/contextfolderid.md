---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: ContextFolderId 要素は、フォルダーを使用する操作を対象とするフォルダーを示します。 この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。
ms.openlocfilehash: 60f1eaf3b45eee83632c7da6f453a1d09f54d9fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529260"
---
# <a name="contextfolderid"></a><span data-ttu-id="f1ae3-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="f1ae3-104">ContextFolderId</span></span>

<span data-ttu-id="f1ae3-105">**ContextFolderId**要素は、フォルダーを使用する操作を対象とするフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="f1ae3-106">この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="f1ae3-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f1ae3-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="f1ae3-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f1ae3-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="f1ae3-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f1ae3-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="f1ae3-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="f1ae3-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


<span data-ttu-id="f1ae3-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="f1ae3-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f1ae3-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f1ae3-112">Attributes and elements</span></span>

<span data-ttu-id="f1ae3-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1ae3-114">属性</span><span class="sxs-lookup"><span data-stu-id="f1ae3-114">Attributes</span></span>

<span data-ttu-id="f1ae3-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1ae3-116">子要素</span><span class="sxs-lookup"><span data-stu-id="f1ae3-116">Child elements</span></span>

|<span data-ttu-id="f1ae3-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="f1ae3-117">**Element**</span></span>|<span data-ttu-id="f1ae3-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1ae3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1ae3-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="f1ae3-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="f1ae3-120">コンテキストフォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="f1ae3-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="f1ae3-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="f1ae3-122">名前で参照できるフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1ae3-123">親要素</span><span class="sxs-lookup"><span data-stu-id="f1ae3-123">Parent elements</span></span>

|<span data-ttu-id="f1ae3-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="f1ae3-124">**Element**</span></span>|<span data-ttu-id="f1ae3-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1ae3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1ae3-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f1ae3-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f1ae3-127">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1ae3-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f1ae3-128">Text value</span></span>

<span data-ttu-id="f1ae3-129">なし。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1ae3-130">注釈</span><span class="sxs-lookup"><span data-stu-id="f1ae3-130">Remarks</span></span>

<span data-ttu-id="f1ae3-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f1ae3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1ae3-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f1ae3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1ae3-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1ae3-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1ae3-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f1ae3-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f1ae3-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f1ae3-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1ae3-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f1ae3-136">Validation File</span></span>  <br/> |<span data-ttu-id="f1ae3-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f1ae3-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1ae3-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f1ae3-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1ae3-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="f1ae3-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1ae3-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="f1ae3-140">See also</span></span>

- [<span data-ttu-id="f1ae3-141">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="f1ae3-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

