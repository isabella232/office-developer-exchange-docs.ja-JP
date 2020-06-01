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
description: SyncScope 要素は、同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463035"
---
# <a name="syncscope"></a><span data-ttu-id="5f5f5-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="5f5f5-103">SyncScope</span></span>

<span data-ttu-id="5f5f5-104">**Syncscope**要素は、同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="5f5f5-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f5f5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5f5f5-106">Attributes and elements</span></span>

<span data-ttu-id="5f5f5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f5f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f5f5-108">Attributes</span></span>

<span data-ttu-id="5f5f5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f5f5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5f5f5-110">Child elements</span></span>

<span data-ttu-id="5f5f5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f5f5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5f5f5-112">Parent elements</span></span>

|<span data-ttu-id="5f5f5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-113">**Element**</span></span>|<span data-ttu-id="5f5f5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f5f5-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5f5f5-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="5f5f5-116">Exchange ストアフォルダー内のアイテムを同期する要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="5f5f5-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="5f5f5-118">/Syncfolderitems</span><span class="sxs-lookup"><span data-stu-id="5f5f5-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f5f5-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5f5f5-119">Text value</span></span>

<span data-ttu-id="5f5f5-120">次の表に、 **Syncscope**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="5f5f5-121">**SyncScope 要素の値**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-121">**SyncScope element values**</span></span>

|<span data-ttu-id="5f5f5-122">**値**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-122">**Value**</span></span>|<span data-ttu-id="5f5f5-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f5f5-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5f5f5-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="5f5f5-124">NormalItems</span></span>  <br/> |<span data-ttu-id="5f5f5-125">同期応答でフォルダー内のアイテムのみが返されるように指定します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="5f5f5-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="5f5f5-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="5f5f5-127">フォルダーとフォルダーに関連付けられたアイテムの両方が同期応答で返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5f5f5-128">注釈</span><span class="sxs-lookup"><span data-stu-id="5f5f5-128">Remarks</span></span>

<span data-ttu-id="5f5f5-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5f5f5-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f5f5-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5f5f5-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f5f5-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f5f5-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5f5f5-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f5f5-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5f5f5-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5f5f5-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5f5f5-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f5f5-134">Validation File</span></span>  <br/> |<span data-ttu-id="5f5f5-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5f5f5-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5f5f5-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5f5f5-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f5f5-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="5f5f5-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f5f5-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f5f5-138">See also</span></span>



[<span data-ttu-id="5f5f5-139">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="5f5f5-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="5f5f5-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f5f5-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

