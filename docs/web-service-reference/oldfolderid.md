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
description: OldFolderId 要素には、移動またはコピーされたフォルダーの元の識別子が含まれています。
ms.openlocfilehash: a6713b9e0c47d68480724c3902086da6a8647dd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458062"
---
# <a name="oldfolderid"></a><span data-ttu-id="5f95e-103">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="5f95e-103">OldFolderId</span></span>

<span data-ttu-id="5f95e-104">**OldFolderId**要素には、移動またはコピーされたフォルダーの元の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5f95e-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="5f95e-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="5f95e-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f95e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5f95e-106">Attributes and elements</span></span>

<span data-ttu-id="5f95e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f95e-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f95e-108">Attributes</span></span>

|<span data-ttu-id="5f95e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="5f95e-109">**Attribute**</span></span>|<span data-ttu-id="5f95e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f95e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5f95e-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="5f95e-111">**Id**</span></span> <br/> |<span data-ttu-id="5f95e-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="5f95e-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="5f95e-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="5f95e-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="5f95e-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="5f95e-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="5f95e-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5f95e-116">This attribute is optional.</span></span> <span data-ttu-id="5f95e-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5f95e-118">子要素</span><span class="sxs-lookup"><span data-stu-id="5f95e-118">Child elements</span></span>

<span data-ttu-id="5f95e-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5f95e-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f95e-120">親要素</span><span class="sxs-lookup"><span data-stu-id="5f95e-120">Parent elements</span></span>

|<span data-ttu-id="5f95e-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f95e-121">**Element**</span></span>|<span data-ttu-id="5f95e-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f95e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f95e-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="5f95e-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="5f95e-124">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="5f95e-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="5f95e-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="5f95e-126">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="5f95e-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5f95e-127">注釈</span><span class="sxs-lookup"><span data-stu-id="5f95e-127">Remarks</span></span>

<span data-ttu-id="5f95e-128">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5f95e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f95e-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5f95e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f95e-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f95e-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f95e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f95e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5f95e-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5f95e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f95e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f95e-133">Validation File</span></span>  <br/> |<span data-ttu-id="5f95e-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5f95e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f95e-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5f95e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f95e-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="5f95e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f95e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f95e-137">See also</span></span>



[<span data-ttu-id="5f95e-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="5f95e-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5f95e-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="5f95e-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5f95e-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="5f95e-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="5f95e-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f95e-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

