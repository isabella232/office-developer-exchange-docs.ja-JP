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
description: ViewPrivateItems 要素は、代理人のユーザーまたはクライアント アプリケーションが主体のメールボックスにプライベート アイテムを表示する権限を持つかどうかを示します。
ms.openlocfilehash: c35f24ae79e907424cb5cfb0efeec2307334ca12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839994"
---
# <a name="viewprivateitems"></a><span data-ttu-id="c4317-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="c4317-103">ViewPrivateItems</span></span>

<span data-ttu-id="c4317-104">**ViewPrivateItems**要素は、代理人のユーザーまたはクライアント アプリケーションが主体のメールボックスにプライベート アイテムを表示する権限を持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4317-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="c4317-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c4317-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4317-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c4317-106">Attributes and elements</span></span>

<span data-ttu-id="c4317-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4317-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4317-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4317-108">Attributes</span></span>

<span data-ttu-id="c4317-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c4317-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4317-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c4317-110">Child elements</span></span>

<span data-ttu-id="c4317-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c4317-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4317-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c4317-112">Parent elements</span></span>

|<span data-ttu-id="c4317-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c4317-113">**Element**</span></span>|<span data-ttu-id="c4317-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c4317-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4317-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="c4317-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="c4317-116">1 つのデリゲートを追加するメールボックスの更新を識別します。</span><span class="sxs-lookup"><span data-stu-id="c4317-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c4317-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c4317-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c4317-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c4317-118">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c4317-119">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4317-119">This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4317-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c4317-120">Text value</span></span>

<span data-ttu-id="c4317-121">**True**の場合、代理人またはクライアント アイテムを表示できますプライベート主体のメールボックス内を示します。</span><span class="sxs-lookup"><span data-stu-id="c4317-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="c4317-122">**False**の値は、プライベートなアイテムが、代理人またはクライアントに表示されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c4317-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c4317-123">備考</span><span class="sxs-lookup"><span data-stu-id="c4317-123">Remarks</span></span>

<span data-ttu-id="c4317-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c4317-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4317-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="c4317-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4317-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="c4317-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4317-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c4317-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c4317-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c4317-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4317-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c4317-129">Validation File</span></span>  <br/> |<span data-ttu-id="c4317-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c4317-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4317-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c4317-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4317-132">False</span><span class="sxs-lookup"><span data-stu-id="c4317-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4317-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="c4317-133">See also</span></span>



[<span data-ttu-id="c4317-134">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c4317-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="c4317-135">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c4317-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="c4317-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c4317-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c4317-137">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="c4317-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

