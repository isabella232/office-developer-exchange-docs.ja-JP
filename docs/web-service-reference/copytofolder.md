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
description: CopyToFolder 要素に項目をコピーすることができます、電子メール フォルダーの識別子を指定します。
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759786"
---
# <a name="copytofolder"></a><span data-ttu-id="b9bcb-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="b9bcb-103">CopyToFolder</span></span>

<span data-ttu-id="b9bcb-104">**CopyToFolder**要素に項目をコピーすることができます、電子メール フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="b9bcb-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="b9bcb-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9bcb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b9bcb-106">Attributes and elements</span></span>

<span data-ttu-id="b9bcb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9bcb-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9bcb-108">Attributes</span></span>

<span data-ttu-id="b9bcb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9bcb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b9bcb-110">Child elements</span></span>

|<span data-ttu-id="b9bcb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9bcb-111">**Element**</span></span>|<span data-ttu-id="b9bcb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9bcb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9bcb-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="b9bcb-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="b9bcb-114">先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="b9bcb-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="b9bcb-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="b9bcb-116">コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9bcb-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b9bcb-117">Parent elements</span></span>

|<span data-ttu-id="b9bcb-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9bcb-118">**Element**</span></span>|<span data-ttu-id="b9bcb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9bcb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9bcb-120">アクション</span><span class="sxs-lookup"><span data-stu-id="b9bcb-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="b9bcb-121">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9bcb-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9bcb-122">Text value</span></span>

<span data-ttu-id="b9bcb-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9bcb-124">備考</span><span class="sxs-lookup"><span data-stu-id="b9bcb-124">Remarks</span></span>

<span data-ttu-id="b9bcb-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b9bcb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9bcb-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b9bcb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9bcb-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b9bcb-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9bcb-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9bcb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9bcb-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9bcb-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9bcb-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9bcb-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9bcb-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9bcb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9bcb-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b9bcb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9bcb-133">True</span><span class="sxs-lookup"><span data-stu-id="b9bcb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9bcb-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9bcb-134">See also</span></span>



[<span data-ttu-id="b9bcb-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="b9bcb-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="b9bcb-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b9bcb-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

