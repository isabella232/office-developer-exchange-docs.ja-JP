---
title: IsFolderContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderContact
api_type:
- schema
ms.assetid: 8b456255-f4ae-4ca0-845a-13c195f1c867
description: IsFolderContact 要素は、ユーザーがフォルダーの連絡先かどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 51a79b4535667685517ff55ef9f6c2b2aaea564c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832015"
---
# <a name="isfoldercontact"></a><span data-ttu-id="bf447-104">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="bf447-104">IsFolderContact</span></span>

<span data-ttu-id="bf447-105">**IsFolderContact**要素は、ユーザーがフォルダーの連絡先かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf447-105">The **IsFolderContact** element indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="bf447-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bf447-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderContact/>
```

 <span data-ttu-id="bf447-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="bf447-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf447-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bf447-108">Attributes and elements</span></span>

<span data-ttu-id="bf447-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bf447-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf447-110">属性</span><span class="sxs-lookup"><span data-stu-id="bf447-110">Attributes</span></span>

<span data-ttu-id="bf447-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bf447-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf447-112">子要素</span><span class="sxs-lookup"><span data-stu-id="bf447-112">Child elements</span></span>

<span data-ttu-id="bf447-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bf447-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf447-114">親要素</span><span class="sxs-lookup"><span data-stu-id="bf447-114">Parent elements</span></span>

|<span data-ttu-id="bf447-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="bf447-115">**Element**</span></span>|<span data-ttu-id="bf447-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf447-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf447-117">Permission</span><span class="sxs-lookup"><span data-stu-id="bf447-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="bf447-118">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="bf447-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="bf447-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bf447-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="bf447-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="bf447-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="bf447-121">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="bf447-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="bf447-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bf447-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf447-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bf447-123">Text value</span></span>

<span data-ttu-id="bf447-124">**True**の場合、テキスト値は、ユーザーが指定したフォルダーの連絡先であることを示します。</span><span class="sxs-lookup"><span data-stu-id="bf447-124">A text value of **true** indicates that the user is a contact for the specified folder.</span></span> <span data-ttu-id="bf447-125">**False**の値は、ユーザーが指定したフォルダーの連絡先ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="bf447-125">A value of **false** indicates that the user is not a contact for the specified folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bf447-126">備考</span><span class="sxs-lookup"><span data-stu-id="bf447-126">Remarks</span></span>

<span data-ttu-id="bf447-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bf447-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf447-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="bf447-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf447-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="bf447-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf447-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bf447-130">Schema Name</span></span>  <br/> |<span data-ttu-id="bf447-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bf447-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf447-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bf447-132">Validation File</span></span>  <br/> |<span data-ttu-id="bf447-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf447-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf447-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bf447-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf447-135">False</span><span class="sxs-lookup"><span data-stu-id="bf447-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf447-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="bf447-136">See also</span></span>



- [<span data-ttu-id="bf447-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bf447-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="bf447-138">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="bf447-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

