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
ms.openlocfilehash: bd863d0395b9b9d7b437833acfb656fec4580985
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759742"
---
# <a name="contextfolderid"></a><span data-ttu-id="f2ece-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="f2ece-104">ContextFolderId</span></span>

<span data-ttu-id="f2ece-105">**ContextFolderId**要素では、フォルダーを使用する操作を対象としているフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="f2ece-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="f2ece-106">この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2ece-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
[<span data-ttu-id="f2ece-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f2ece-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="f2ece-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f2ece-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="f2ece-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f2ece-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="f2ece-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="f2ece-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

 <span data-ttu-id="f2ece-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="f2ece-111">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2ece-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2ece-112">Attributes and elements</span></span>

<span data-ttu-id="f2ece-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2ece-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2ece-114">属性</span><span class="sxs-lookup"><span data-stu-id="f2ece-114">Attributes</span></span>

<span data-ttu-id="f2ece-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f2ece-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2ece-116">子要素</span><span class="sxs-lookup"><span data-stu-id="f2ece-116">Child elements</span></span>

|<span data-ttu-id="f2ece-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2ece-117">**Element**</span></span>|<span data-ttu-id="f2ece-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2ece-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2ece-119">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="f2ece-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="f2ece-120">コンテキスト フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2ece-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="f2ece-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="f2ece-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="f2ece-122">名前で参照可能なフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2ece-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2ece-123">親要素</span><span class="sxs-lookup"><span data-stu-id="f2ece-123">Parent elements</span></span>

|<span data-ttu-id="f2ece-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2ece-124">**Element**</span></span>|<span data-ttu-id="f2ece-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2ece-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2ece-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f2ece-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f2ece-127">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2ece-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2ece-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2ece-128">Text value</span></span>

<span data-ttu-id="f2ece-129">なし。</span><span class="sxs-lookup"><span data-stu-id="f2ece-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2ece-130">備考</span><span class="sxs-lookup"><span data-stu-id="f2ece-130">Remarks</span></span>

<span data-ttu-id="f2ece-131">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f2ece-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2ece-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2ece-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2ece-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2ece-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2ece-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2ece-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f2ece-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f2ece-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2ece-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2ece-136">Validation File</span></span>  <br/> |<span data-ttu-id="f2ece-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2ece-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2ece-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2ece-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2ece-139">False</span><span class="sxs-lookup"><span data-stu-id="f2ece-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2ece-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2ece-140">See also</span></span>



[<span data-ttu-id="f2ece-141">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="f2ece-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

