---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: ViewPrivateItems 要素は、代理人のユーザーまたはクライアントアプリケーションがプリンシパルのメールボックス内のプライベートアイテムを表示するためのアクセス許可を持っているかどうかを示します。
ms.openlocfilehash: 4e1375f7c4a3c660cc5de885deff8d094250ca7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525970"
---
# <a name="viewprivateitems"></a><span data-ttu-id="d2335-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="d2335-103">ViewPrivateItems</span></span>

<span data-ttu-id="d2335-104">**Viewprivateitems**要素は、代理人のユーザーまたはクライアントアプリケーションがプリンシパルのメールボックス内のプライベートアイテムを表示するためのアクセス許可を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2335-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="d2335-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d2335-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2335-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2335-106">Attributes and elements</span></span>

<span data-ttu-id="d2335-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2335-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2335-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2335-108">Attributes</span></span>

<span data-ttu-id="d2335-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2335-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2335-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2335-110">Child elements</span></span>

<span data-ttu-id="d2335-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d2335-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2335-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d2335-112">Parent elements</span></span>

|<span data-ttu-id="d2335-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2335-113">**Element**</span></span>|<span data-ttu-id="d2335-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2335-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2335-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="d2335-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="d2335-116">メールボックスに追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2335-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2335-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="d2335-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="d2335-118">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2335-118">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="d2335-119">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d2335-119">This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2335-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d2335-120">Text value</span></span>

<span data-ttu-id="d2335-121">値が**true の場合**は、代理人またはクライアントがプリンシパルのメールボックス内のプライベートアイテムを表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="d2335-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="d2335-122">値が**false**の場合は、代理人またはクライアントがプライベートアイテムを表示できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d2335-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d2335-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d2335-123">Remarks</span></span>

<span data-ttu-id="d2335-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d2335-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2335-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2335-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2335-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="d2335-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2335-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2335-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d2335-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d2335-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2335-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2335-129">Validation File</span></span>  <br/> |<span data-ttu-id="d2335-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d2335-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2335-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d2335-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2335-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="d2335-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2335-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2335-133">See also</span></span>



[<span data-ttu-id="d2335-134">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="d2335-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="d2335-135">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="d2335-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="d2335-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2335-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d2335-137">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="d2335-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

