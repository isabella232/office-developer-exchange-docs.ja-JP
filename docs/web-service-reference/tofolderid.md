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
ms.openlocfilehash: a48309f0b7f5c9bf667fc2eb653a0502832bc996
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839710"
---
# <a name="tofolderid"></a><span data-ttu-id="f2451-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="f2451-103">ToFolderId</span></span>

<span data-ttu-id="f2451-104">**ToFolderId**要素は、先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f2451-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

 <span data-ttu-id="f2451-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="f2451-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2451-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2451-106">Attributes and elements</span></span>

<span data-ttu-id="f2451-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2451-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2451-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2451-108">Attributes</span></span>

<span data-ttu-id="f2451-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2451-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2451-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2451-110">Child elements</span></span>

|<span data-ttu-id="f2451-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2451-111">**Element**</span></span>|<span data-ttu-id="f2451-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2451-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2451-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="f2451-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="f2451-114">先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2451-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="f2451-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="f2451-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="f2451-116">コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2451-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2451-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f2451-117">Parent elements</span></span>

|<span data-ttu-id="f2451-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2451-118">**Element**</span></span>|<span data-ttu-id="f2451-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2451-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2451-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="f2451-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="f2451-121">Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2451-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="f2451-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f2451-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="f2451-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="f2451-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="f2451-124">Exchange ストア内のフォルダーをコピーするのには要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2451-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="f2451-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f2451-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="f2451-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="f2451-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="f2451-127">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2451-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="f2451-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f2451-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="f2451-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="f2451-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="f2451-130">Exchange ストア内の項目をコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2451-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="f2451-131">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f2451-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2451-132">備考</span><span class="sxs-lookup"><span data-stu-id="f2451-132">Remarks</span></span>

<span data-ttu-id="f2451-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f2451-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2451-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2451-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2451-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2451-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2451-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2451-136">Schema Name</span></span>  <br/> |<span data-ttu-id="f2451-137">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f2451-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f2451-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2451-138">Validation File</span></span>  <br/> |<span data-ttu-id="f2451-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f2451-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2451-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2451-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2451-141">False</span><span class="sxs-lookup"><span data-stu-id="f2451-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2451-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2451-142">See also</span></span>



[<span data-ttu-id="f2451-143">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="f2451-143">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="f2451-144">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="f2451-144">CopyFolder operation</span></span>](copyfolder-operation.md)
  
<span data-ttu-id="f2451-145">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="f2451-145">[MoveItem operation](moveitem-operation.md)</span></span>
  
<span data-ttu-id="f2451-146">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="f2451-146">[CopyItem operation](copyitem-operation.md)</span></span>

