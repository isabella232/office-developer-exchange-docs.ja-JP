---
title: CanCreateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateItems
api_type:
- schema
ms.assetid: c4574e9a-3c42-40a1-a5f9-79b6560e9b30
description: CanCreateItems 要素は、ユーザーがフォルダー内にアイテムを作成する権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 73d3d967774d9fcff53722d0936462025e02b659
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458783"
---
# <a name="cancreateitems"></a><span data-ttu-id="08e35-104">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="08e35-104">CanCreateItems</span></span>

<span data-ttu-id="08e35-105">**Cancreateitems**要素は、ユーザーがフォルダー内にアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08e35-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="08e35-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08e35-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="08e35-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="08e35-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08e35-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="08e35-108">Attributes and elements</span></span>

<span data-ttu-id="08e35-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08e35-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08e35-110">属性</span><span class="sxs-lookup"><span data-stu-id="08e35-110">Attributes</span></span>

<span data-ttu-id="08e35-111">なし。</span><span class="sxs-lookup"><span data-stu-id="08e35-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08e35-112">子要素</span><span class="sxs-lookup"><span data-stu-id="08e35-112">Child elements</span></span>

<span data-ttu-id="08e35-113">なし。</span><span class="sxs-lookup"><span data-stu-id="08e35-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08e35-114">親要素</span><span class="sxs-lookup"><span data-stu-id="08e35-114">Parent elements</span></span>

|<span data-ttu-id="08e35-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="08e35-115">**Element**</span></span>|<span data-ttu-id="08e35-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="08e35-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08e35-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08e35-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="08e35-118">ユーザーがフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="08e35-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="08e35-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08e35-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="08e35-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="08e35-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="08e35-121">ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="08e35-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="08e35-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08e35-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08e35-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08e35-123">Text value</span></span>

<span data-ttu-id="08e35-124">テキスト値が**true の場合**は、ユーザーがフォルダー内にアイテムを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="08e35-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="08e35-125">値が**false**の場合は、ユーザーがフォルダー内にアイテムを作成できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="08e35-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08e35-126">注釈</span><span class="sxs-lookup"><span data-stu-id="08e35-126">Remarks</span></span>

<span data-ttu-id="08e35-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="08e35-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08e35-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="08e35-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08e35-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="08e35-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08e35-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08e35-130">Schema Name</span></span>  <br/> |<span data-ttu-id="08e35-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="08e35-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="08e35-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08e35-132">Validation File</span></span>  <br/> |<span data-ttu-id="08e35-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="08e35-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08e35-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="08e35-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="08e35-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="08e35-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08e35-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="08e35-136">See also</span></span>



- [<span data-ttu-id="08e35-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="08e35-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="08e35-138">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="08e35-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

