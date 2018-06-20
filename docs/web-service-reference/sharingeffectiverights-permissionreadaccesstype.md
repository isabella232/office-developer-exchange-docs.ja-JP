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
description: SharingEffectiveRights 要素は、ユーザーが共有されている連絡先のデータを持っているアクセス許可を示します。
ms.openlocfilehash: 19e67827dd2dbff6fb70423980d670da5cc257a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833486"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="9fefd-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="9fefd-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="9fefd-104">**SharingEffectiveRights**要素は、ユーザーが共有されている連絡先のデータを持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="9fefd-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="9fefd-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fefd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9fefd-106">Attributes and elements</span></span>

<span data-ttu-id="9fefd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fefd-108">属性</span><span class="sxs-lookup"><span data-stu-id="9fefd-108">Attributes</span></span>

<span data-ttu-id="9fefd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9fefd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fefd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9fefd-110">Child elements</span></span>

<span data-ttu-id="9fefd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9fefd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fefd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9fefd-112">Parent elements</span></span>

|<span data-ttu-id="9fefd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9fefd-113">**Element**</span></span>|<span data-ttu-id="9fefd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fefd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fefd-115">メッセージ</span><span class="sxs-lookup"><span data-stu-id="9fefd-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9fefd-116">メールボックスに格納されている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fefd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9fefd-117">Text value</span></span>

<span data-ttu-id="9fefd-118">次の表は、 **SharingEffectiveRights**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="9fefd-119">**SharingEffectiveRights 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="9fefd-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="9fefd-120">**値**</span><span class="sxs-lookup"><span data-stu-id="9fefd-120">**Value**</span></span>|<span data-ttu-id="9fefd-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fefd-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9fefd-122">なし</span><span class="sxs-lookup"><span data-stu-id="9fefd-122">None</span></span>  <br/> |<span data-ttu-id="9fefd-123">ユーザーに、フォルダー内のアイテムの読み取りアクセス許可がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="9fefd-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="9fefd-124">FullDetails</span></span>  <br/> |<span data-ttu-id="9fefd-125">ユーザーがフォルダー内のすべてのアイテムの読み取りアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9fefd-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fefd-126">備考</span><span class="sxs-lookup"><span data-stu-id="9fefd-126">Remarks</span></span>

<span data-ttu-id="9fefd-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9fefd-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fefd-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="9fefd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fefd-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="9fefd-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fefd-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9fefd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9fefd-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9fefd-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fefd-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9fefd-132">Validation File</span></span>  <br/> |<span data-ttu-id="9fefd-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fefd-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fefd-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9fefd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fefd-135">False</span><span class="sxs-lookup"><span data-stu-id="9fefd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fefd-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="9fefd-136">See also</span></span>



- [<span data-ttu-id="9fefd-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9fefd-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

