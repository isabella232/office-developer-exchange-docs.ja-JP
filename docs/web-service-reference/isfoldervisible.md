---
title: IsFolderVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderVisible
api_type:
- schema
ms.assetid: dd611fb5-9424-4ff9-bb27-c882c73c0c74
description: IsFolderVisible 要素は、ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 27a6bca9ae71bc93de6c22cb87c8d582025144e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832019"
---
# <a name="isfoldervisible"></a><span data-ttu-id="21352-104">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="21352-104">IsFolderVisible</span></span>

<span data-ttu-id="21352-105">**IsFolderVisible**要素は、ユーザーがフォルダーを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="21352-105">The **IsFolderVisible** element indicates whether a user can view a folder.</span></span> <span data-ttu-id="21352-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="21352-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderVisible/>
```

 <span data-ttu-id="21352-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="21352-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21352-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21352-108">Attributes and elements</span></span>

<span data-ttu-id="21352-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21352-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21352-110">属性</span><span class="sxs-lookup"><span data-stu-id="21352-110">Attributes</span></span>

<span data-ttu-id="21352-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21352-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21352-112">子要素</span><span class="sxs-lookup"><span data-stu-id="21352-112">Child elements</span></span>

<span data-ttu-id="21352-113">なし。</span><span class="sxs-lookup"><span data-stu-id="21352-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21352-114">親要素</span><span class="sxs-lookup"><span data-stu-id="21352-114">Parent elements</span></span>

|<span data-ttu-id="21352-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="21352-115">**Element**</span></span>|<span data-ttu-id="21352-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="21352-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21352-117">Permission</span><span class="sxs-lookup"><span data-stu-id="21352-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="21352-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="21352-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="21352-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="21352-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="21352-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="21352-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="21352-121">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="21352-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="21352-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="21352-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21352-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21352-123">Text value</span></span>

<span data-ttu-id="21352-124">**True**の場合、テキスト値は、ユーザーがフォルダーを表示できますを示します。</span><span class="sxs-lookup"><span data-stu-id="21352-124">A text value of **true** indicates that the user can view the folder.</span></span> <span data-ttu-id="21352-125">**False**の値は、ユーザーがフォルダーを表示できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="21352-125">A value of **false** indicates that the user cannot view the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="21352-126">備考</span><span class="sxs-lookup"><span data-stu-id="21352-126">Remarks</span></span>

<span data-ttu-id="21352-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21352-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21352-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="21352-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21352-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="21352-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21352-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21352-130">Schema Name</span></span>  <br/> |<span data-ttu-id="21352-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="21352-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="21352-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21352-132">Validation File</span></span>  <br/> |<span data-ttu-id="21352-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="21352-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21352-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21352-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="21352-135">False</span><span class="sxs-lookup"><span data-stu-id="21352-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21352-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="21352-136">See also</span></span>



- [<span data-ttu-id="21352-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="21352-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="21352-138">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="21352-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

