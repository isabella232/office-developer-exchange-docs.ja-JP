---
title: ReadItems (PermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: 0a11a802-28e2-436b-b5a9-30fd064675a6
description: ReadItems 要素は、ユーザーがフォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: bf266c77106f25b90ffd174e25fb0c3972ab91cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832961"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="da3cf-104">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="da3cf-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="da3cf-105">**ReadItems**要素は、ユーザーがフォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="da3cf-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="da3cf-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="da3cf-107">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="da3cf-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da3cf-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da3cf-108">Attributes and elements</span></span>

<span data-ttu-id="da3cf-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da3cf-110">属性</span><span class="sxs-lookup"><span data-stu-id="da3cf-110">Attributes</span></span>

<span data-ttu-id="da3cf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da3cf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da3cf-112">子要素</span><span class="sxs-lookup"><span data-stu-id="da3cf-112">Child elements</span></span>

<span data-ttu-id="da3cf-113">なし。</span><span class="sxs-lookup"><span data-stu-id="da3cf-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da3cf-114">親要素</span><span class="sxs-lookup"><span data-stu-id="da3cf-114">Parent elements</span></span>

|<span data-ttu-id="da3cf-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="da3cf-115">**Element**</span></span>|<span data-ttu-id="da3cf-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="da3cf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da3cf-117">Permission</span><span class="sxs-lookup"><span data-stu-id="da3cf-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="da3cf-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="da3cf-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="da3cf-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da3cf-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da3cf-120">Text value</span></span>

<span data-ttu-id="da3cf-121">**ReadItems**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="da3cf-122">**ReadItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="da3cf-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="da3cf-123">**値**</span><span class="sxs-lookup"><span data-stu-id="da3cf-123">**Value**</span></span>|<span data-ttu-id="da3cf-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="da3cf-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da3cf-125">なし</span><span class="sxs-lookup"><span data-stu-id="da3cf-125">None</span></span>  <br/> |<span data-ttu-id="da3cf-126">ユーザーに、フォルダー内のアイテムの読み取りアクセス許可がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="da3cf-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="da3cf-127">FullDetails</span></span>  <br/> |<span data-ttu-id="da3cf-128">ユーザーがフォルダー内のすべてのアイテムの読み取りアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="da3cf-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da3cf-129">備考</span><span class="sxs-lookup"><span data-stu-id="da3cf-129">Remarks</span></span>

<span data-ttu-id="da3cf-130">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="da3cf-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da3cf-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="da3cf-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da3cf-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="da3cf-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da3cf-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da3cf-133">Schema Name</span></span>  <br/> |<span data-ttu-id="da3cf-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="da3cf-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="da3cf-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da3cf-135">Validation File</span></span>  <br/> |<span data-ttu-id="da3cf-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da3cf-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da3cf-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="da3cf-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="da3cf-138">False</span><span class="sxs-lookup"><span data-stu-id="da3cf-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da3cf-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="da3cf-139">See also</span></span>



- [<span data-ttu-id="da3cf-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="da3cf-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="da3cf-141">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="da3cf-141">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

