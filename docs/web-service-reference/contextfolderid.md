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
description: ContextFolderId 要素では、フォルダーを使用する操作を対象としているフォルダーを示します。 この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。
ms.openlocfilehash: 94428a079be6da8873c777556771579a7110fb62
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354282"
---
# <a name="contextfolderid"></a><span data-ttu-id="496b0-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="496b0-104">ContextFolderId</span></span>

<span data-ttu-id="496b0-105">**ContextFolderId**要素では、フォルダーを使用する操作を対象としているフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="496b0-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="496b0-106">この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="496b0-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="496b0-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="496b0-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="496b0-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="496b0-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="496b0-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="496b0-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="496b0-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="496b0-110">ContextFolderId</span></span>](contextfolderid.md)
  
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


<span data-ttu-id="496b0-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="496b0-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="496b0-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="496b0-112">Attributes and elements</span></span>

<span data-ttu-id="496b0-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="496b0-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="496b0-114">属性</span><span class="sxs-lookup"><span data-stu-id="496b0-114">Attributes</span></span>

<span data-ttu-id="496b0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="496b0-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="496b0-116">子要素</span><span class="sxs-lookup"><span data-stu-id="496b0-116">Child elements</span></span>

|<span data-ttu-id="496b0-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="496b0-117">**Element**</span></span>|<span data-ttu-id="496b0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="496b0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="496b0-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="496b0-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="496b0-120">コンテキスト フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="496b0-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="496b0-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="496b0-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="496b0-122">名前で参照可能なフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="496b0-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="496b0-123">親要素</span><span class="sxs-lookup"><span data-stu-id="496b0-123">Parent elements</span></span>

|<span data-ttu-id="496b0-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="496b0-124">**Element**</span></span>|<span data-ttu-id="496b0-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="496b0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="496b0-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="496b0-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="496b0-127">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="496b0-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="496b0-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="496b0-128">Text value</span></span>

<span data-ttu-id="496b0-129">なし。</span><span class="sxs-lookup"><span data-stu-id="496b0-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="496b0-130">注釈</span><span class="sxs-lookup"><span data-stu-id="496b0-130">Remarks</span></span>

<span data-ttu-id="496b0-131">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="496b0-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="496b0-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="496b0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="496b0-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="496b0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="496b0-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="496b0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="496b0-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="496b0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="496b0-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="496b0-136">Validation File</span></span>  <br/> |<span data-ttu-id="496b0-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="496b0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="496b0-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="496b0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="496b0-139">False</span><span class="sxs-lookup"><span data-stu-id="496b0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="496b0-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="496b0-140">See also</span></span>

- [<span data-ttu-id="496b0-141">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="496b0-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

