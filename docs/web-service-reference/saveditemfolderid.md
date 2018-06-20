---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: SavedItemFolderId 要素は、更新、送信、およびメールボックス内のアイテムを作成する操作のターゲット フォルダーを識別します。
ms.openlocfilehash: c57a7fb4abc2f7ee7b599f56f016811d6ff2c21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833277"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="6d9bb-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="6d9bb-103">SavedItemFolderId</span></span>

<span data-ttu-id="6d9bb-104">**SavedItemFolderId**要素は、更新、送信、およびメールボックス内のアイテムを作成する操作のターゲット フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

 <span data-ttu-id="6d9bb-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6d9bb-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d9bb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6d9bb-106">Attributes and elements</span></span>

<span data-ttu-id="6d9bb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d9bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d9bb-108">Attributes</span></span>

<span data-ttu-id="6d9bb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d9bb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d9bb-110">Child elements</span></span>

|<span data-ttu-id="6d9bb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d9bb-111">**Element**</span></span>|<span data-ttu-id="6d9bb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d9bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d9bb-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="6d9bb-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6d9bb-114">更新、送信、および Exchange ストア内の項目を作成する操作の対象となるフォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d9bb-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6d9bb-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6d9bb-116">更新、送信、および Exchange ストア内の項目を作成する操作の名前付きの識別子では、対象となるフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d9bb-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6d9bb-117">Parent elements</span></span>

|<span data-ttu-id="6d9bb-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d9bb-118">**Element**</span></span>|<span data-ttu-id="6d9bb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d9bb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d9bb-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="6d9bb-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="6d9bb-121">Exchange ストア内のアイテムを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="6d9bb-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="6d9bb-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="6d9bb-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="6d9bb-124">Exchange ストア内の項目を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="6d9bb-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="6d9bb-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="6d9bb-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="6d9bb-127">Exchange ストア内のアイテムを送信する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="6d9bb-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d9bb-129">備考</span><span class="sxs-lookup"><span data-stu-id="6d9bb-129">Remarks</span></span>

<span data-ttu-id="6d9bb-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6d9bb-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d9bb-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="6d9bb-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d9bb-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="6d9bb-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d9bb-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d9bb-133">Schema Name</span></span>  <br/> |<span data-ttu-id="6d9bb-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d9bb-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6d9bb-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d9bb-135">Validation File</span></span>  <br/> |<span data-ttu-id="6d9bb-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d9bb-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d9bb-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d9bb-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d9bb-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="6d9bb-138">False</span></span>  <br/> |
   

