---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: DestinationFolderId 要素は、コピー先のフォルダーを指定し、アクションを移動します。
ms.openlocfilehash: 5fb6cae7db9cdb09e23b3627e26e695ecf6418f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760022"
---
# <a name="destinationfolderid"></a><span data-ttu-id="fd30e-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="fd30e-103">DestinationFolderId</span></span>

<span data-ttu-id="fd30e-104">**DestinationFolderId**要素は、コピー先のフォルダーを指定し、アクションを移動します。</span><span class="sxs-lookup"><span data-stu-id="fd30e-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="fd30e-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="fd30e-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="fd30e-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="fd30e-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="fd30e-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="fd30e-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="fd30e-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="fd30e-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

 <span data-ttu-id="fd30e-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="fd30e-109">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd30e-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fd30e-110">Attributes and elements</span></span>

<span data-ttu-id="fd30e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd30e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd30e-112">属性</span><span class="sxs-lookup"><span data-stu-id="fd30e-112">Attributes</span></span>

<span data-ttu-id="fd30e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fd30e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd30e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="fd30e-114">Child elements</span></span>

|<span data-ttu-id="fd30e-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd30e-115">**Element**</span></span>|<span data-ttu-id="fd30e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd30e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd30e-117">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="fd30e-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="fd30e-118">コピー先のフォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd30e-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="fd30e-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="fd30e-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="fd30e-120">名前で参照可能なフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="fd30e-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd30e-121">親要素</span><span class="sxs-lookup"><span data-stu-id="fd30e-121">Parent elements</span></span>

|<span data-ttu-id="fd30e-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd30e-122">**Element**</span></span>|<span data-ttu-id="fd30e-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd30e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd30e-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="fd30e-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="fd30e-125">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd30e-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd30e-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fd30e-126">Text value</span></span>

<span data-ttu-id="fd30e-127">なし。</span><span class="sxs-lookup"><span data-stu-id="fd30e-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fd30e-128">備考</span><span class="sxs-lookup"><span data-stu-id="fd30e-128">Remarks</span></span>

<span data-ttu-id="fd30e-129">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fd30e-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd30e-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="fd30e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd30e-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="fd30e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd30e-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd30e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="fd30e-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fd30e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd30e-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd30e-134">Validation File</span></span>  <br/> |<span data-ttu-id="fd30e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd30e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd30e-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd30e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd30e-137">False</span><span class="sxs-lookup"><span data-stu-id="fd30e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd30e-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd30e-138">See also</span></span>

- [<span data-ttu-id="fd30e-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="fd30e-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

