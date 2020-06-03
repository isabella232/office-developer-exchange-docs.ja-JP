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
description: ReadItems 要素は、ユーザーがフォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: af6ef5107b5e4f2b3071c0bc9b4b528efea6dcca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468272"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="04161-104">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="04161-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="04161-105">**ReadItems**要素は、ユーザーがフォルダー内のアイテムを読み取る権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04161-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="04161-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04161-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="04161-107">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="04161-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04161-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="04161-108">Attributes and elements</span></span>

<span data-ttu-id="04161-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04161-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04161-110">属性</span><span class="sxs-lookup"><span data-stu-id="04161-110">Attributes</span></span>

<span data-ttu-id="04161-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04161-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04161-112">子要素</span><span class="sxs-lookup"><span data-stu-id="04161-112">Child elements</span></span>

<span data-ttu-id="04161-113">なし。</span><span class="sxs-lookup"><span data-stu-id="04161-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04161-114">親要素</span><span class="sxs-lookup"><span data-stu-id="04161-114">Parent elements</span></span>

|<span data-ttu-id="04161-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="04161-115">**Element**</span></span>|<span data-ttu-id="04161-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="04161-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04161-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04161-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="04161-118">ユーザーがフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="04161-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="04161-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04161-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04161-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04161-120">Text value</span></span>

<span data-ttu-id="04161-121">次の表に、 **ReadItems**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="04161-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="04161-122">**ReadItems 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="04161-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="04161-123">**値**</span><span class="sxs-lookup"><span data-stu-id="04161-123">**Value**</span></span>|<span data-ttu-id="04161-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="04161-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04161-125">なし</span><span class="sxs-lookup"><span data-stu-id="04161-125">None</span></span>  <br/> |<span data-ttu-id="04161-126">ユーザーがフォルダー内のアイテムを読み取るためのアクセス許可を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="04161-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="04161-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="04161-127">FullDetails</span></span>  <br/> |<span data-ttu-id="04161-128">ユーザーがフォルダー内のすべてのアイテムを読み取る権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="04161-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04161-129">注釈</span><span class="sxs-lookup"><span data-stu-id="04161-129">Remarks</span></span>

<span data-ttu-id="04161-130">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="04161-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04161-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="04161-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04161-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="04161-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04161-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04161-133">Schema Name</span></span>  <br/> |<span data-ttu-id="04161-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="04161-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="04161-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04161-135">Validation File</span></span>  <br/> |<span data-ttu-id="04161-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="04161-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04161-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04161-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="04161-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="04161-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04161-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="04161-139">See also</span></span>



- [<span data-ttu-id="04161-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="04161-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="04161-141">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="04161-141">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

