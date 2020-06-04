---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: ToFolderId 要素は、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468776"
---
# <a name="tofolderid"></a><span data-ttu-id="171e8-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="171e8-103">ToFolderId</span></span>

<span data-ttu-id="171e8-104">**ToFolderId**要素は、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="171e8-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

<span data-ttu-id="171e8-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="171e8-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="171e8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="171e8-106">Attributes and elements</span></span>

<span data-ttu-id="171e8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="171e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="171e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="171e8-108">Attributes</span></span>

<span data-ttu-id="171e8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="171e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="171e8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="171e8-110">Child elements</span></span>

|<span data-ttu-id="171e8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="171e8-111">**Element**</span></span>|<span data-ttu-id="171e8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="171e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="171e8-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="171e8-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="171e8-114">コピーまたは移動したアイテムまたはフォルダーの宛先フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="171e8-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="171e8-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="171e8-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="171e8-116">コピーまたは移動されたアイテムまたはフォルダーについて、名前付きの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="171e8-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="171e8-117">親要素</span><span class="sxs-lookup"><span data-stu-id="171e8-117">Parent elements</span></span>

|<span data-ttu-id="171e8-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="171e8-118">**Element**</span></span>|<span data-ttu-id="171e8-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="171e8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="171e8-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="171e8-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="171e8-121">Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="171e8-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="171e8-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="171e8-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="171e8-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="171e8-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="171e8-124">Exchange ストア内のフォルダーをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="171e8-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="171e8-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="171e8-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="171e8-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="171e8-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="171e8-127">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="171e8-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="171e8-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="171e8-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="171e8-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="171e8-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="171e8-130">Exchange ストア内のアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="171e8-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="171e8-131">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="171e8-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="171e8-132">注釈</span><span class="sxs-lookup"><span data-stu-id="171e8-132">Remarks</span></span>

<span data-ttu-id="171e8-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="171e8-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="171e8-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="171e8-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="171e8-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="171e8-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="171e8-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="171e8-136">Schema Name</span></span>  <br/> |<span data-ttu-id="171e8-137">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="171e8-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="171e8-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="171e8-138">Validation File</span></span>  <br/> |<span data-ttu-id="171e8-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="171e8-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="171e8-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="171e8-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="171e8-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="171e8-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="171e8-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="171e8-142">See also</span></span>

- [<span data-ttu-id="171e8-143">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="171e8-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="171e8-144">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="171e8-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="171e8-145">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="171e8-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="171e8-146">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="171e8-146">CopyItem operation</span></span>](copyitem-operation.md)

