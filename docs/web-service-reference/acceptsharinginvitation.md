---
title: AcceptSharingInvitation 状
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
description: AcceptSharingInvitation 要素は、別のユーザーの予定表または連絡先データへのアクセスを許可する招待を受け入れるために使用されます。
ms.openlocfilehash: c8cdae707bd122e74fa0e284163d1540d857c3de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461710"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="d4fd3-103">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="d4fd3-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="d4fd3-104">**Acceptsharinginvitation**要素は、別のユーザーの予定表または連絡先データへのアクセスを許可する招待を受け入れるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="d4fd3-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="d4fd3-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4fd3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d4fd3-106">Attributes and elements</span></span>

<span data-ttu-id="d4fd3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4fd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4fd3-108">Attributes</span></span>

<span data-ttu-id="d4fd3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4fd3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4fd3-110">Child elements</span></span>

|<span data-ttu-id="d4fd3-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d4fd3-111">**Element**</span></span>|<span data-ttu-id="d4fd3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fd3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fd3-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="d4fd3-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="d4fd3-114">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4fd3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d4fd3-115">Parent elements</span></span>

|<span data-ttu-id="d4fd3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4fd3-116">**Element**</span></span>|<span data-ttu-id="d4fd3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fd3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fd3-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="d4fd3-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="d4fd3-119">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d4fd3-120">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="d4fd3-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="d4fd3-121">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4fd3-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d4fd3-122">Remarks</span></span>

<span data-ttu-id="d4fd3-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d4fd3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4fd3-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d4fd3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4fd3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4fd3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4fd3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4fd3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d4fd3-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d4fd3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4fd3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4fd3-128">Validation File</span></span>  <br/> |<span data-ttu-id="d4fd3-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d4fd3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4fd3-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d4fd3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4fd3-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="d4fd3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4fd3-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4fd3-132">See also</span></span>

- [<span data-ttu-id="d4fd3-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="d4fd3-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="d4fd3-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4fd3-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

