---
title: 削除
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
description: 削除要素は、クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。
ms.openlocfilehash: 8a00a24ea63fa564ecefb96a5caed3a9199690eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759959"
---
# <a name="delete"></a><span data-ttu-id="19f4b-103">削除</span><span class="sxs-lookup"><span data-stu-id="19f4b-103">Delete</span></span>

<span data-ttu-id="19f4b-104">要素の**削除**では、クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="19f4b-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="19f4b-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="19f4b-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="19f4b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19f4b-106">Attributes and elements</span></span>

<span data-ttu-id="19f4b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19f4b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19f4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="19f4b-108">Attributes</span></span>

<span data-ttu-id="19f4b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19f4b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19f4b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19f4b-110">Child elements</span></span>

<span data-ttu-id="19f4b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19f4b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19f4b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19f4b-112">Parent elements</span></span>

|<span data-ttu-id="19f4b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="19f4b-113">**Element**</span></span>|<span data-ttu-id="19f4b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="19f4b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19f4b-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="19f4b-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="19f4b-116">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19f4b-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="19f4b-117">アクション</span><span class="sxs-lookup"><span data-stu-id="19f4b-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="19f4b-118">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="19f4b-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19f4b-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19f4b-119">Text value</span></span>

<span data-ttu-id="19f4b-120">**True**の場合、テキスト値は、クライアントがアイテムまたはフォルダーを削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="19f4b-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="19f4b-121">**False**の値では、クライアントがアイテムまたはフォルダーを削除できませんすることを示します。</span><span class="sxs-lookup"><span data-stu-id="19f4b-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19f4b-122">備考</span><span class="sxs-lookup"><span data-stu-id="19f4b-122">Remarks</span></span>

<span data-ttu-id="19f4b-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19f4b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19f4b-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="19f4b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19f4b-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="19f4b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19f4b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19f4b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="19f4b-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="19f4b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="19f4b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19f4b-128">Validation File</span></span>  <br/> |<span data-ttu-id="19f4b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19f4b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19f4b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19f4b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="19f4b-131">False</span><span class="sxs-lookup"><span data-stu-id="19f4b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19f4b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="19f4b-132">See also</span></span>

- [<span data-ttu-id="19f4b-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19f4b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="19f4b-134">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="19f4b-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

