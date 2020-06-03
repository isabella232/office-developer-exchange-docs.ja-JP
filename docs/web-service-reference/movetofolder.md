---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: MoveToFolder 要素は、電子メールアイテムを移動できるフォルダーの識別子を指定します。
ms.openlocfilehash: e323b2ac5390855b3db0b5495af667cdf2da5596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530008"
---
# <a name="movetofolder"></a><span data-ttu-id="0be0c-103">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="0be0c-103">MoveToFolder</span></span>

<span data-ttu-id="0be0c-104">**Movetofolder**要素は、電子メールアイテムを移動できるフォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="0be0c-104">The **MoveToFolder** element specifies the identifier of the folder to which email items can be moved.</span></span> 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 <span data-ttu-id="0be0c-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0be0c-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0be0c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0be0c-106">Attributes and elements</span></span>

<span data-ttu-id="0be0c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0be0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0be0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0be0c-108">Attributes</span></span>

<span data-ttu-id="0be0c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0be0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0be0c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0be0c-110">Child elements</span></span>

|<span data-ttu-id="0be0c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0be0c-111">**Element**</span></span>|<span data-ttu-id="0be0c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0be0c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0be0c-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="0be0c-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0be0c-114">コピーまたは移動したアイテムまたはフォルダーの宛先フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0be0c-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="0be0c-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0be0c-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0be0c-116">コピーまたは移動されたアイテムまたはフォルダーについて、名前付きの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0be0c-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0be0c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0be0c-117">Parent elements</span></span>

|<span data-ttu-id="0be0c-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="0be0c-118">**Element**</span></span>|<span data-ttu-id="0be0c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0be0c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0be0c-120">Actions</span><span class="sxs-lookup"><span data-stu-id="0be0c-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="0be0c-121">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="0be0c-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled..</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0be0c-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0be0c-122">Text value</span></span>

<span data-ttu-id="0be0c-123">なし。</span><span class="sxs-lookup"><span data-stu-id="0be0c-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0be0c-124">注釈</span><span class="sxs-lookup"><span data-stu-id="0be0c-124">Remarks</span></span>

<span data-ttu-id="0be0c-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0be0c-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0be0c-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0be0c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0be0c-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0be0c-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0be0c-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0be0c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0be0c-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0be0c-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0be0c-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0be0c-130">Validation File</span></span>  <br/> |<span data-ttu-id="0be0c-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0be0c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0be0c-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0be0c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0be0c-133">正しい</span><span class="sxs-lookup"><span data-stu-id="0be0c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0be0c-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="0be0c-134">See also</span></span>



[<span data-ttu-id="0be0c-135">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="0be0c-135">CopyToFolder</span></span>](copytofolder.md)


- [<span data-ttu-id="0be0c-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0be0c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

