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
description: CanCreateItems 要素は、ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 313699a15ef3038dd9114c18b76b29aba15e5ab7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759611"
---
# <a name="cancreateitems"></a><span data-ttu-id="60b24-104">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="60b24-104">CanCreateItems</span></span>

<span data-ttu-id="60b24-105">**CanCreateItems**要素は、ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60b24-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="60b24-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="60b24-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="60b24-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="60b24-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60b24-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="60b24-108">Attributes and elements</span></span>

<span data-ttu-id="60b24-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60b24-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60b24-110">属性</span><span class="sxs-lookup"><span data-stu-id="60b24-110">Attributes</span></span>

<span data-ttu-id="60b24-111">なし。</span><span class="sxs-lookup"><span data-stu-id="60b24-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60b24-112">子要素</span><span class="sxs-lookup"><span data-stu-id="60b24-112">Child elements</span></span>

<span data-ttu-id="60b24-113">なし。</span><span class="sxs-lookup"><span data-stu-id="60b24-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60b24-114">親要素</span><span class="sxs-lookup"><span data-stu-id="60b24-114">Parent elements</span></span>

|<span data-ttu-id="60b24-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="60b24-115">**Element**</span></span>|<span data-ttu-id="60b24-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="60b24-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60b24-117">Permission</span><span class="sxs-lookup"><span data-stu-id="60b24-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="60b24-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="60b24-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="60b24-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="60b24-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="60b24-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="60b24-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="60b24-121">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="60b24-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="60b24-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="60b24-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60b24-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="60b24-123">Text value</span></span>

<span data-ttu-id="60b24-124">**True**の場合、テキスト値は、ユーザーがフォルダー内のアイテムを作成できますを示します。</span><span class="sxs-lookup"><span data-stu-id="60b24-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="60b24-125">**False**の値は、ユーザーがフォルダー内のアイテムを作成できませんを示します。</span><span class="sxs-lookup"><span data-stu-id="60b24-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="60b24-126">備考</span><span class="sxs-lookup"><span data-stu-id="60b24-126">Remarks</span></span>

<span data-ttu-id="60b24-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="60b24-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60b24-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="60b24-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60b24-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="60b24-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60b24-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60b24-130">Schema Name</span></span>  <br/> |<span data-ttu-id="60b24-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="60b24-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="60b24-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60b24-132">Validation File</span></span>  <br/> |<span data-ttu-id="60b24-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="60b24-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60b24-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="60b24-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="60b24-135">False</span><span class="sxs-lookup"><span data-stu-id="60b24-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60b24-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="60b24-136">See also</span></span>



- [<span data-ttu-id="60b24-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="60b24-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="60b24-138">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="60b24-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

