---
title: IsFolderOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderOwner
api_type:
- schema
ms.assetid: 6541ee78-d6e6-42a7-8e7a-d8736172b245
description: IsFolderOwner 要素は、ユーザーがフォルダーの所有者であるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: a8838b2a7ed1b16c1e332d34a38038ba8254fc3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832016"
---
# <a name="isfolderowner"></a><span data-ttu-id="5e2cd-104">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="5e2cd-104">IsFolderOwner</span></span>

<span data-ttu-id="5e2cd-105">**IsFolderOwner**要素は、ユーザーがフォルダーの所有者であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-105">The **IsFolderOwner** element indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="5e2cd-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderOwner/>
```

 <span data-ttu-id="5e2cd-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="5e2cd-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e2cd-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5e2cd-108">Attributes and elements</span></span>

<span data-ttu-id="5e2cd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e2cd-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e2cd-110">Attributes</span></span>

<span data-ttu-id="5e2cd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e2cd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="5e2cd-112">Child elements</span></span>

<span data-ttu-id="5e2cd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e2cd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="5e2cd-114">Parent elements</span></span>

|<span data-ttu-id="5e2cd-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="5e2cd-115">**Element**</span></span>|<span data-ttu-id="5e2cd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e2cd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e2cd-117">Permission</span><span class="sxs-lookup"><span data-stu-id="5e2cd-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="5e2cd-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="5e2cd-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="5e2cd-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="5e2cd-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="5e2cd-121">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="5e2cd-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e2cd-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5e2cd-123">Text value</span></span>

<span data-ttu-id="5e2cd-124">**True**の場合、テキスト値は、ユーザーがフォルダーの所有者であることを示します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-124">A text value of **true** indicates that the user is the owner of the folder.</span></span> <span data-ttu-id="5e2cd-125">**False**の値は、ユーザーがフォルダーの所有者ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-125">A value of **false** indicates that the user is not the owner of the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5e2cd-126">備考</span><span class="sxs-lookup"><span data-stu-id="5e2cd-126">Remarks</span></span>

<span data-ttu-id="5e2cd-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5e2cd-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e2cd-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="5e2cd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e2cd-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="5e2cd-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e2cd-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5e2cd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5e2cd-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5e2cd-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e2cd-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5e2cd-132">Validation File</span></span>  <br/> |<span data-ttu-id="5e2cd-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e2cd-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e2cd-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5e2cd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e2cd-135">False</span><span class="sxs-lookup"><span data-stu-id="5e2cd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e2cd-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e2cd-136">See also</span></span>



- [<span data-ttu-id="5e2cd-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5e2cd-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5e2cd-138">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="5e2cd-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

