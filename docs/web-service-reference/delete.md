---
title: Delete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: Delete 要素は、クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。
ms.openlocfilehash: 5460f9e49b126ca6b039c6f11aaa3c6eb4a40544
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457355"
---
# <a name="delete"></a><span data-ttu-id="c0453-103">削除</span><span class="sxs-lookup"><span data-stu-id="c0453-103">Delete</span></span>

<span data-ttu-id="c0453-104">**Delete**要素は、クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0453-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="c0453-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="c0453-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c0453-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c0453-106">Attributes and elements</span></span>

<span data-ttu-id="c0453-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0453-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0453-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0453-108">Attributes</span></span>

<span data-ttu-id="c0453-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c0453-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0453-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c0453-110">Child elements</span></span>

<span data-ttu-id="c0453-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c0453-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0453-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c0453-112">Parent elements</span></span>

|<span data-ttu-id="c0453-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0453-113">**Element**</span></span>|<span data-ttu-id="c0453-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0453-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0453-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c0453-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c0453-116">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0453-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="c0453-117">Actions</span><span class="sxs-lookup"><span data-stu-id="c0453-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c0453-118">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c0453-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0453-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c0453-119">Text value</span></span>

<span data-ttu-id="c0453-120">テキスト値が**true の場合**は、クライアントがアイテムまたはフォルダーを削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="c0453-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="c0453-121">値が**false**の場合は、クライアントがアイテムまたはフォルダーを削除できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c0453-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c0453-122">注釈</span><span class="sxs-lookup"><span data-stu-id="c0453-122">Remarks</span></span>

<span data-ttu-id="c0453-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c0453-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0453-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c0453-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0453-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0453-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0453-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0453-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c0453-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c0453-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0453-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0453-128">Validation File</span></span>  <br/> |<span data-ttu-id="c0453-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c0453-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0453-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c0453-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0453-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="c0453-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0453-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0453-132">See also</span></span>

- [<span data-ttu-id="c0453-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c0453-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c0453-134">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="c0453-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

