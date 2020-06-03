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
description: DestinationFolderId 要素は、コピー操作と移動操作の宛先フォルダーを示します。
ms.openlocfilehash: dbfd25084dbd4ea9d5f4ddf98b256d02e71139d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526915"
---
# <a name="destinationfolderid"></a><span data-ttu-id="a5967-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="a5967-103">DestinationFolderId</span></span>

<span data-ttu-id="a5967-104">**DestinationFolderId**要素は、コピー操作と移動操作の宛先フォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="a5967-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="a5967-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="a5967-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="a5967-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="a5967-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="a5967-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="a5967-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="a5967-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="a5967-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

```XML
<DestinationFolderId>
   <DistinguishedFolderId/>
</DestinationFolderId>
```

<span data-ttu-id="a5967-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="a5967-109">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a5967-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a5967-110">Attributes and elements</span></span>

<span data-ttu-id="a5967-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a5967-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5967-112">属性</span><span class="sxs-lookup"><span data-stu-id="a5967-112">Attributes</span></span>

<span data-ttu-id="a5967-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a5967-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5967-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a5967-114">Child elements</span></span>

|<span data-ttu-id="a5967-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="a5967-115">**Element**</span></span>|<span data-ttu-id="a5967-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5967-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5967-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="a5967-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="a5967-118">宛先フォルダーの識別子と変更キーが保存されています。</span><span class="sxs-lookup"><span data-stu-id="a5967-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="a5967-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a5967-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="a5967-120">名前で参照できるフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a5967-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5967-121">親要素</span><span class="sxs-lookup"><span data-stu-id="a5967-121">Parent elements</span></span>

|<span data-ttu-id="a5967-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="a5967-122">**Element**</span></span>|<span data-ttu-id="a5967-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5967-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5967-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="a5967-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="a5967-125">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a5967-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5967-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a5967-126">Text value</span></span>

<span data-ttu-id="a5967-127">なし。</span><span class="sxs-lookup"><span data-stu-id="a5967-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5967-128">注釈</span><span class="sxs-lookup"><span data-stu-id="a5967-128">Remarks</span></span>

<span data-ttu-id="a5967-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a5967-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5967-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a5967-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5967-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5967-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5967-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a5967-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a5967-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a5967-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5967-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a5967-134">Validation File</span></span>  <br/> |<span data-ttu-id="a5967-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a5967-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5967-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a5967-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5967-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="a5967-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5967-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a5967-138">See also</span></span>

- [<span data-ttu-id="a5967-139">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="a5967-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

