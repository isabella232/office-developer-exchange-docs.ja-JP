---
title: OldFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: OldFolderId 要素には、移動またはコピーするフォルダーの元の識別子が含まれています。
ms.openlocfilehash: ef73cad73213a1e8b5341907cd22177d8e1ba628
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832645"
---
# <a name="oldfolderid"></a><span data-ttu-id="b0d1b-103">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="b0d1b-103">OldFolderId</span></span>

<span data-ttu-id="b0d1b-104">**OldFolderId**要素には、移動またはコピーするフォルダーの元の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="b0d1b-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0d1b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b0d1b-106">Attributes and elements</span></span>

<span data-ttu-id="b0d1b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0d1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0d1b-108">Attributes</span></span>

|<span data-ttu-id="b0d1b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-109">**Attribute**</span></span>|<span data-ttu-id="b0d1b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0d1b-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-111">**Id**</span></span> <br/> |<span data-ttu-id="b0d1b-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="b0d1b-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b0d1b-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="b0d1b-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="b0d1b-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-116">This attribute is optional.</span></span> <span data-ttu-id="b0d1b-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b0d1b-118">子要素</span><span class="sxs-lookup"><span data-stu-id="b0d1b-118">Child elements</span></span>

<span data-ttu-id="b0d1b-119">なし。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0d1b-120">親要素</span><span class="sxs-lookup"><span data-stu-id="b0d1b-120">Parent elements</span></span>

|<span data-ttu-id="b0d1b-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-121">**Element**</span></span>|<span data-ttu-id="b0d1b-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0d1b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0d1b-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="b0d1b-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="b0d1b-124">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="b0d1b-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="b0d1b-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="b0d1b-126">アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0d1b-127">備考</span><span class="sxs-lookup"><span data-stu-id="b0d1b-127">Remarks</span></span>

<span data-ttu-id="b0d1b-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b0d1b-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0d1b-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="b0d1b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0d1b-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="b0d1b-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0d1b-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0d1b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b0d1b-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b0d1b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0d1b-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0d1b-133">Validation File</span></span>  <br/> |<span data-ttu-id="b0d1b-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0d1b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0d1b-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0d1b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0d1b-136">False</span><span class="sxs-lookup"><span data-stu-id="b0d1b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0d1b-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0d1b-137">See also</span></span>



[<span data-ttu-id="b0d1b-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="b0d1b-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="b0d1b-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="b0d1b-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="b0d1b-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="b0d1b-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="b0d1b-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0d1b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

