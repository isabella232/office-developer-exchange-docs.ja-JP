---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: PermissionSet 要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれています。
ms.openlocfilehash: 5639ee8ba64742f39c0274f4e3aaa76d75bea42b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468132"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="f7102-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f7102-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="f7102-104">**PermissionSet**要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f7102-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="f7102-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="f7102-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7102-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f7102-106">Attributes and elements</span></span>

<span data-ttu-id="f7102-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7102-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7102-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7102-108">Attributes</span></span>

<span data-ttu-id="f7102-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f7102-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7102-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f7102-110">Child elements</span></span>

|<span data-ttu-id="f7102-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f7102-111">**Element**</span></span>|<span data-ttu-id="f7102-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7102-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7102-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7102-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="f7102-114">フォルダーのアクセス許可のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="f7102-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="f7102-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f7102-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f7102-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="f7102-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="f7102-117">Active Directory ディレクトリサービスに対して解決できない不明なエントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f7102-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="f7102-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f7102-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7102-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f7102-119">Parent elements</span></span>

|<span data-ttu-id="f7102-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f7102-120">**Element**</span></span>|<span data-ttu-id="f7102-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7102-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7102-122">Folder</span><span class="sxs-lookup"><span data-stu-id="f7102-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="f7102-123">作成、取得、検索、同期、更新を行うフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="f7102-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="f7102-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f7102-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f7102-125">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f7102-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f7102-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="f7102-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="f7102-127">メールボックスに含まれている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f7102-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f7102-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="f7102-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="f7102-129">メールボックスに含まれる tasks フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f7102-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7102-130">注釈</span><span class="sxs-lookup"><span data-stu-id="f7102-130">Remarks</span></span>

<span data-ttu-id="f7102-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f7102-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f7102-132">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f7102-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f7102-133">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="f7102-133">Version differences</span></span>

<span data-ttu-id="f7102-134">Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。</span><span class="sxs-lookup"><span data-stu-id="f7102-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="f7102-135">フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="f7102-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f7102-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f7102-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7102-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7102-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7102-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7102-138">Schema Name</span></span>  <br/> |<span data-ttu-id="f7102-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f7102-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7102-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7102-140">Validation File</span></span>  <br/> |<span data-ttu-id="f7102-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f7102-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7102-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f7102-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7102-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="f7102-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7102-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="f7102-144">See also</span></span>



- [<span data-ttu-id="f7102-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f7102-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f7102-146">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="f7102-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

