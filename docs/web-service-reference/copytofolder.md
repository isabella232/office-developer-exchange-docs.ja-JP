---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: CopyToFolder 要素は、電子メールアイテムをコピーできるフォルダーの識別子を指定します。
ms.openlocfilehash: 7cdda0f9769f909255c9b76f78ac7094a8dfc8f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463175"
---
# <a name="copytofolder"></a><span data-ttu-id="ed5c9-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="ed5c9-103">CopyToFolder</span></span>

<span data-ttu-id="ed5c9-104">**Copytofolder**要素は、電子メールアイテムをコピーできるフォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="ed5c9-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="ed5c9-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed5c9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ed5c9-106">Attributes and elements</span></span>

<span data-ttu-id="ed5c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed5c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed5c9-108">Attributes</span></span>

<span data-ttu-id="ed5c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed5c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed5c9-110">Child elements</span></span>

|<span data-ttu-id="ed5c9-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ed5c9-111">**Element**</span></span>|<span data-ttu-id="ed5c9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed5c9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed5c9-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ed5c9-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ed5c9-114">コピーまたは移動したアイテムまたはフォルダーの宛先フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ed5c9-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ed5c9-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="ed5c9-116">コピーまたは移動されたアイテムまたはフォルダーについて、名前付きの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed5c9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ed5c9-117">Parent elements</span></span>

|<span data-ttu-id="ed5c9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed5c9-118">**Element**</span></span>|<span data-ttu-id="ed5c9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed5c9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed5c9-120">Actions</span><span class="sxs-lookup"><span data-stu-id="ed5c9-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ed5c9-121">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed5c9-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed5c9-122">Text value</span></span>

<span data-ttu-id="ed5c9-123">なし。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed5c9-124">注釈</span><span class="sxs-lookup"><span data-stu-id="ed5c9-124">Remarks</span></span>

<span data-ttu-id="ed5c9-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ed5c9-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed5c9-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ed5c9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed5c9-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed5c9-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed5c9-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed5c9-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ed5c9-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ed5c9-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ed5c9-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed5c9-130">Validation File</span></span>  <br/> |<span data-ttu-id="ed5c9-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ed5c9-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed5c9-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed5c9-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed5c9-133">正しい</span><span class="sxs-lookup"><span data-stu-id="ed5c9-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed5c9-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed5c9-134">See also</span></span>



[<span data-ttu-id="ed5c9-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="ed5c9-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="ed5c9-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ed5c9-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

