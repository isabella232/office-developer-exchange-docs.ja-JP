---
title: AcceptSharingInvitation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptSharingInvitation
api_type:
- schema
ms.assetid: 3c2a47d6-490d-425b-8893-089a4f8882cd
description: AcceptSharingInvitation 要素を使用して、別のユーザーの予定表や連絡先のデータへのアクセスを可能にするための招待を承諾します。
ms.openlocfilehash: 06439739e6cc544d5039ac9d18e0452b1d42a0ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760423"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="187ff-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="187ff-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="187ff-104">**AcceptSharingInvitation**要素を使用して、別のユーザーの予定表や連絡先のデータへのアクセスを可能にするための招待を承諾します。</span><span class="sxs-lookup"><span data-stu-id="187ff-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="187ff-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="187ff-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="187ff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="187ff-106">Attributes and elements</span></span>

<span data-ttu-id="187ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="187ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="187ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="187ff-108">Attributes</span></span>

<span data-ttu-id="187ff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="187ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="187ff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="187ff-110">Child elements</span></span>

|<span data-ttu-id="187ff-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="187ff-111">**Element**</span></span>|<span data-ttu-id="187ff-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="187ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="187ff-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="187ff-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="187ff-114">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="187ff-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="187ff-115">親要素</span><span class="sxs-lookup"><span data-stu-id="187ff-115">Parent elements</span></span>

|<span data-ttu-id="187ff-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="187ff-116">**Element**</span></span>|<span data-ttu-id="187ff-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="187ff-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="187ff-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="187ff-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="187ff-119">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="187ff-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="187ff-120">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="187ff-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="187ff-121">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="187ff-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="187ff-122">備考</span><span class="sxs-lookup"><span data-stu-id="187ff-122">Remarks</span></span>

<span data-ttu-id="187ff-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="187ff-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="187ff-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="187ff-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="187ff-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="187ff-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="187ff-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="187ff-126">Schema Name</span></span>  <br/> |<span data-ttu-id="187ff-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="187ff-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="187ff-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="187ff-128">Validation File</span></span>  <br/> |<span data-ttu-id="187ff-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="187ff-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="187ff-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="187ff-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="187ff-131">False</span><span class="sxs-lookup"><span data-stu-id="187ff-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="187ff-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="187ff-132">See also</span></span>

- [<span data-ttu-id="187ff-133">Createitem メソッド (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="187ff-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="187ff-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="187ff-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

