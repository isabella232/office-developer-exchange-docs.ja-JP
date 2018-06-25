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
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832732"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="14775-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="14775-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="14775-104">**PermissionSet**要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="14775-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="14775-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="14775-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14775-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="14775-106">Attributes and elements</span></span>

<span data-ttu-id="14775-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="14775-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14775-108">属性</span><span class="sxs-lookup"><span data-stu-id="14775-108">Attributes</span></span>

<span data-ttu-id="14775-109">なし。</span><span class="sxs-lookup"><span data-stu-id="14775-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14775-110">子要素</span><span class="sxs-lookup"><span data-stu-id="14775-110">Child elements</span></span>

|<span data-ttu-id="14775-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="14775-111">**Element**</span></span>|<span data-ttu-id="14775-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="14775-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14775-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14775-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="14775-114">フォルダーのアクセス許可のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="14775-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="14775-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="14775-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="14775-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="14775-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="14775-117">Active Directory ディレクトリ サービスに対して解決できない不明なエントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="14775-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="14775-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="14775-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14775-119">親要素</span><span class="sxs-lookup"><span data-stu-id="14775-119">Parent elements</span></span>

|<span data-ttu-id="14775-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="14775-120">**Element**</span></span>|<span data-ttu-id="14775-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="14775-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14775-122">Folder</span><span class="sxs-lookup"><span data-stu-id="14775-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="14775-123">作成、取得、検索、同期、または更新するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="14775-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="14775-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="14775-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="14775-125">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="14775-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="14775-126">メッセージ</span><span class="sxs-lookup"><span data-stu-id="14775-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="14775-127">メールボックスに格納されている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="14775-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="14775-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="14775-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="14775-129">メールボックスに含まれるタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="14775-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="14775-130">備考</span><span class="sxs-lookup"><span data-stu-id="14775-130">Remarks</span></span>

<span data-ttu-id="14775-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="14775-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="14775-132">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="14775-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="14775-133">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="14775-133">Version differences</span></span>

<span data-ttu-id="14775-134">アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。</span><span class="sxs-lookup"><span data-stu-id="14775-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="14775-135">フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="14775-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="14775-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="14775-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14775-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="14775-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="14775-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="14775-138">Schema Name</span></span>  <br/> |<span data-ttu-id="14775-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="14775-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="14775-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="14775-140">Validation File</span></span>  <br/> |<span data-ttu-id="14775-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="14775-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14775-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="14775-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="14775-143">False</span><span class="sxs-lookup"><span data-stu-id="14775-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14775-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="14775-144">See also</span></span>



- [<span data-ttu-id="14775-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="14775-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="14775-146">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="14775-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

