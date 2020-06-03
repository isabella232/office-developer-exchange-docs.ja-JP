---
title: アクセス許可
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: Permissions 要素には、フォルダーのアクセス許可のコレクションが含まれています。
ms.openlocfilehash: b8616cefdb8c453106753fb0788a6c7d6a0ded79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459217"
---
# <a name="permissions"></a><span data-ttu-id="e9344-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="e9344-103">Permissions</span></span>

<span data-ttu-id="e9344-104">**Permissions**要素には、フォルダーのアクセス許可のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9344-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="e9344-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="e9344-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9344-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9344-106">Attributes and elements</span></span>

<span data-ttu-id="e9344-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9344-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9344-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9344-108">Attributes</span></span>

<span data-ttu-id="e9344-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9344-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9344-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9344-110">Child elements</span></span>

|<span data-ttu-id="e9344-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e9344-111">**Element**</span></span>|<span data-ttu-id="e9344-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9344-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9344-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9344-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="e9344-114">代理人がフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="e9344-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="e9344-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9344-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9344-116">親要素</span><span class="sxs-lookup"><span data-stu-id="e9344-116">Parent elements</span></span>

|<span data-ttu-id="e9344-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9344-117">**Element**</span></span>|<span data-ttu-id="e9344-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9344-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9344-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="e9344-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="e9344-120">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e9344-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="e9344-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9344-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9344-122">注釈</span><span class="sxs-lookup"><span data-stu-id="e9344-122">Remarks</span></span>

<span data-ttu-id="e9344-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9344-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e9344-124">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9344-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="e9344-125">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="e9344-125">Version differences</span></span>

<span data-ttu-id="e9344-126">Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。</span><span class="sxs-lookup"><span data-stu-id="e9344-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="e9344-127">フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="e9344-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e9344-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9344-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9344-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9344-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9344-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9344-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e9344-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9344-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9344-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9344-132">Validation File</span></span>  <br/> |<span data-ttu-id="e9344-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9344-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9344-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9344-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9344-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="e9344-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9344-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9344-136">See also</span></span>



- [<span data-ttu-id="e9344-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e9344-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e9344-138">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="e9344-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

