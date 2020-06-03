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
description: SavedItemFolderId 要素は、メールボックス内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーを指定します。
ms.openlocfilehash: 8e18b8863a54aa4e9d6e65f7a54e20904f5a9599
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465276"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="7b6dc-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="7b6dc-103">SavedItemFolderId</span></span>

<span data-ttu-id="7b6dc-104">**SavedItemFolderId**要素は、メールボックス内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

<span data-ttu-id="7b6dc-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="7b6dc-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7b6dc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7b6dc-106">Attributes and elements</span></span>

<span data-ttu-id="7b6dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b6dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b6dc-108">Attributes</span></span>

<span data-ttu-id="7b6dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b6dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7b6dc-110">Child elements</span></span>

|<span data-ttu-id="7b6dc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7b6dc-111">**Element**</span></span>|<span data-ttu-id="7b6dc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b6dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b6dc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="7b6dc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7b6dc-114">Exchange ストア内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーの識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7b6dc-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7b6dc-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="7b6dc-116">Exchange ストア内のアイテムを更新、送信、および作成する操作について、ターゲットフォルダーを名前付き識別子で識別します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b6dc-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7b6dc-117">Parent elements</span></span>

|<span data-ttu-id="7b6dc-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b6dc-118">**Element**</span></span>|<span data-ttu-id="7b6dc-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b6dc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b6dc-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="7b6dc-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="7b6dc-121">Exchange ストア内のアイテムを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="7b6dc-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="7b6dc-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7b6dc-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="7b6dc-124">Exchange ストア内のアイテムを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="7b6dc-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="7b6dc-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="7b6dc-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="7b6dc-127">Exchange ストア内のアイテムを送信するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="7b6dc-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b6dc-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7b6dc-129">Remarks</span></span>

<span data-ttu-id="7b6dc-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7b6dc-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b6dc-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7b6dc-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b6dc-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="7b6dc-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7b6dc-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b6dc-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7b6dc-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7b6dc-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7b6dc-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b6dc-135">Validation File</span></span>  <br/> |<span data-ttu-id="7b6dc-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7b6dc-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b6dc-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7b6dc-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b6dc-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="7b6dc-138">False</span></span>  <br/> |
   

