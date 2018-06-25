---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: SyncScope 要素は、同期応答内のアイテムまたはアイテムおよびフォルダーに関連付けられている情報だけを返すかどうかを指定します。
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839642"
---
# <a name="syncscope"></a><span data-ttu-id="82522-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="82522-103">SyncScope</span></span>

<span data-ttu-id="82522-104">**SyncScope**要素は、同期応答内のアイテムまたはアイテムおよびフォルダーに関連付けられている情報だけを返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="82522-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="82522-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="82522-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82522-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="82522-106">Attributes and elements</span></span>

<span data-ttu-id="82522-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82522-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82522-108">属性</span><span class="sxs-lookup"><span data-stu-id="82522-108">Attributes</span></span>

<span data-ttu-id="82522-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82522-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82522-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82522-110">Child elements</span></span>

<span data-ttu-id="82522-111">なし。</span><span class="sxs-lookup"><span data-stu-id="82522-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82522-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82522-112">Parent elements</span></span>

|<span data-ttu-id="82522-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="82522-113">**Element**</span></span>|<span data-ttu-id="82522-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="82522-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82522-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="82522-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="82522-116">Exchange ストア フォルダー内のアイテムを同期するための要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="82522-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="82522-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="82522-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="82522-118">/SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="82522-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82522-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82522-119">Text value</span></span>

<span data-ttu-id="82522-120">次の表は、 **SyncScope**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="82522-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="82522-121">**SyncScope 要素の値**</span><span class="sxs-lookup"><span data-stu-id="82522-121">**SyncScope element values**</span></span>

|<span data-ttu-id="82522-122">**値**</span><span class="sxs-lookup"><span data-stu-id="82522-122">**Value**</span></span>|<span data-ttu-id="82522-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="82522-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82522-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="82522-124">NormalItems</span></span>  <br/> |<span data-ttu-id="82522-125">フォルダー内のアイテムのみが同期の応答で返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="82522-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="82522-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="82522-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="82522-127">フォルダーと関連付けられているフォルダーの情報の両方の項目が同期応答で返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="82522-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="82522-128">備考</span><span class="sxs-lookup"><span data-stu-id="82522-128">Remarks</span></span>

<span data-ttu-id="82522-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="82522-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82522-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="82522-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82522-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="82522-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82522-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82522-132">Schema Name</span></span>  <br/> |<span data-ttu-id="82522-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="82522-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82522-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82522-134">Validation File</span></span>  <br/> |<span data-ttu-id="82522-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="82522-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82522-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82522-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="82522-137">False</span><span class="sxs-lookup"><span data-stu-id="82522-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82522-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="82522-138">See also</span></span>



[<span data-ttu-id="82522-139">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="82522-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="82522-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="82522-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

