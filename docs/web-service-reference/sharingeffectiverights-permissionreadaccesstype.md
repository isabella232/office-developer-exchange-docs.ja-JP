---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: SharingEffectiveRights 要素は、共有されている連絡先データに対してユーザーが持っているアクセス許可を示します。
ms.openlocfilehash: 64b1e6d831068e9699e9cd47693e74919e0416a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526663"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="29e47-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="29e47-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="29e47-104">**SharingEffectiveRights**要素は、共有されている連絡先データに対してユーザーが持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="29e47-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="29e47-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="29e47-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29e47-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29e47-106">Attributes and elements</span></span>

<span data-ttu-id="29e47-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29e47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29e47-108">属性</span><span class="sxs-lookup"><span data-stu-id="29e47-108">Attributes</span></span>

<span data-ttu-id="29e47-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29e47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29e47-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29e47-110">Child elements</span></span>

<span data-ttu-id="29e47-111">なし。</span><span class="sxs-lookup"><span data-stu-id="29e47-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29e47-112">親要素</span><span class="sxs-lookup"><span data-stu-id="29e47-112">Parent elements</span></span>

|<span data-ttu-id="29e47-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="29e47-113">**Element**</span></span>|<span data-ttu-id="29e47-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="29e47-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29e47-115">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="29e47-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="29e47-116">メールボックスに含まれている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="29e47-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29e47-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29e47-117">Text value</span></span>

<span data-ttu-id="29e47-118">次の表に、 **SharingEffectiveRights**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="29e47-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="29e47-119">**SharingEffectiveRights 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="29e47-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="29e47-120">**値**</span><span class="sxs-lookup"><span data-stu-id="29e47-120">**Value**</span></span>|<span data-ttu-id="29e47-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="29e47-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29e47-122">なし</span><span class="sxs-lookup"><span data-stu-id="29e47-122">None</span></span>  <br/> |<span data-ttu-id="29e47-123">ユーザーがフォルダー内のアイテムを読み取るためのアクセス許可を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="29e47-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="29e47-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="29e47-124">FullDetails</span></span>  <br/> |<span data-ttu-id="29e47-125">ユーザーがフォルダー内のすべてのアイテムを読み取る権限を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="29e47-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29e47-126">注釈</span><span class="sxs-lookup"><span data-stu-id="29e47-126">Remarks</span></span>

<span data-ttu-id="29e47-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="29e47-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29e47-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29e47-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29e47-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="29e47-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29e47-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29e47-130">Schema Name</span></span>  <br/> |<span data-ttu-id="29e47-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="29e47-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="29e47-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29e47-132">Validation File</span></span>  <br/> |<span data-ttu-id="29e47-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29e47-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29e47-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29e47-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="29e47-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="29e47-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29e47-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="29e47-136">See also</span></span>



- [<span data-ttu-id="29e47-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29e47-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

