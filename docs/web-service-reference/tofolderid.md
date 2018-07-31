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
description: ToFolderId 要素は、先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353659"
---
# <a name="tofolderid"></a><span data-ttu-id="4e3fc-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="4e3fc-103">ToFolderId</span></span>

<span data-ttu-id="4e3fc-104">**ToFolderId**要素は、先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
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

<span data-ttu-id="4e3fc-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="4e3fc-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4e3fc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e3fc-106">Attributes and elements</span></span>

<span data-ttu-id="4e3fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e3fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e3fc-108">Attributes</span></span>

<span data-ttu-id="4e3fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e3fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4e3fc-110">Child elements</span></span>

|<span data-ttu-id="4e3fc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e3fc-111">**Element**</span></span>|<span data-ttu-id="4e3fc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e3fc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e3fc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="4e3fc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="4e3fc-114">先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="4e3fc-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="4e3fc-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="4e3fc-116">コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e3fc-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4e3fc-117">Parent elements</span></span>

|<span data-ttu-id="4e3fc-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e3fc-118">**Element**</span></span>|<span data-ttu-id="4e3fc-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e3fc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e3fc-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="4e3fc-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="4e3fc-121">Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="4e3fc-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="4e3fc-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="4e3fc-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="4e3fc-124">Exchange ストア内のフォルダーをコピーするのには要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="4e3fc-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="4e3fc-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="4e3fc-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="4e3fc-127">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="4e3fc-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="4e3fc-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="4e3fc-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="4e3fc-130">Exchange ストア内の項目をコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="4e3fc-131">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4e3fc-132">注釈</span><span class="sxs-lookup"><span data-stu-id="4e3fc-132">Remarks</span></span>

<span data-ttu-id="4e3fc-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4e3fc-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e3fc-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="4e3fc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e3fc-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="4e3fc-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e3fc-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e3fc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="4e3fc-137">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4e3fc-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4e3fc-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e3fc-138">Validation File</span></span>  <br/> |<span data-ttu-id="4e3fc-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4e3fc-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e3fc-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4e3fc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e3fc-141">False</span><span class="sxs-lookup"><span data-stu-id="4e3fc-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e3fc-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e3fc-142">See also</span></span>

- [<span data-ttu-id="4e3fc-143">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="4e3fc-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="4e3fc-144">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="4e3fc-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- <span data-ttu-id="4e3fc-145">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4e3fc-145">[MoveItem operation](moveitem-operation.md)</span></span> 
- <span data-ttu-id="4e3fc-146">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4e3fc-146">[CopyItem operation](copyitem-operation.md)</span></span>

