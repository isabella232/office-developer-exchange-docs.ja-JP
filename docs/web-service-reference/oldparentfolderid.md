---
title: OldParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: OldParentFolderId 要素には、アイテムまたはフォルダーをコピーまたは移動の親フォルダーの識別子が含まれています。
ms.openlocfilehash: 1c4a51755c4194939dd797efa31cf5410b02bf85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832644"
---
# <a name="oldparentfolderid"></a><span data-ttu-id="6c600-103">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6c600-103">OldParentFolderId</span></span>

<span data-ttu-id="6c600-104">**OldParentFolderId**要素には、アイテムまたはフォルダーをコピーまたは移動の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c600-104">The **OldParentFolderId** element contains the identifier of the parent folder of an item or folder that was copied or moved.</span></span> 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="6c600-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6c600-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c600-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6c600-106">Attributes and elements</span></span>

<span data-ttu-id="6c600-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c600-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c600-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c600-108">Attributes</span></span>

|<span data-ttu-id="6c600-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6c600-109">**Attribute**</span></span>|<span data-ttu-id="6c600-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c600-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c600-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="6c600-111">**Id**</span></span> <br/> |<span data-ttu-id="6c600-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c600-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="6c600-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c600-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6c600-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="6c600-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="6c600-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c600-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="6c600-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6c600-116">This attribute is optional.</span></span> <span data-ttu-id="6c600-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="6c600-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6c600-118">子要素</span><span class="sxs-lookup"><span data-stu-id="6c600-118">Child elements</span></span>

<span data-ttu-id="6c600-119">なし。</span><span class="sxs-lookup"><span data-stu-id="6c600-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c600-120">親要素</span><span class="sxs-lookup"><span data-stu-id="6c600-120">Parent elements</span></span>

|<span data-ttu-id="6c600-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c600-121">**Element**</span></span>|<span data-ttu-id="6c600-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c600-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c600-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="6c600-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="6c600-124">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="6c600-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="6c600-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="6c600-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="6c600-126">アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="6c600-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c600-127">備考</span><span class="sxs-lookup"><span data-stu-id="6c600-127">Remarks</span></span>

<span data-ttu-id="6c600-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6c600-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c600-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="6c600-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c600-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="6c600-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c600-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c600-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6c600-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c600-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c600-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c600-133">Validation File</span></span>  <br/> |<span data-ttu-id="6c600-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6c600-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c600-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c600-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c600-136">False</span><span class="sxs-lookup"><span data-stu-id="6c600-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c600-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c600-137">See also</span></span>



[<span data-ttu-id="6c600-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6c600-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="6c600-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="6c600-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="6c600-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="6c600-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="6c600-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c600-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

