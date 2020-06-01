---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: UnknownEntries 要素には、Active Directory ディレクトリサービスに対して解決できない、不明なアクセス許可エントリの配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 68cb2518b895ca0a74e6b9ed649ee92b7502ab05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459420"
---
# <a name="unknownentries"></a><span data-ttu-id="04539-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="04539-104">UnknownEntries</span></span>

<span data-ttu-id="04539-105">**UnknownEntries**要素には、Active Directory ディレクトリサービスに対して解決できない、不明なアクセス許可エントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="04539-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="04539-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04539-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="04539-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="04539-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04539-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="04539-108">Attributes and elements</span></span>

<span data-ttu-id="04539-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04539-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04539-110">属性</span><span class="sxs-lookup"><span data-stu-id="04539-110">Attributes</span></span>

<span data-ttu-id="04539-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04539-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04539-112">子要素</span><span class="sxs-lookup"><span data-stu-id="04539-112">Child elements</span></span>

|<span data-ttu-id="04539-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="04539-113">**Element**</span></span>|<span data-ttu-id="04539-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="04539-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04539-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="04539-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="04539-116">Active Directory に対して解決できない1つの不明なアクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="04539-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="04539-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04539-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04539-118">親要素</span><span class="sxs-lookup"><span data-stu-id="04539-118">Parent elements</span></span>

|<span data-ttu-id="04539-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="04539-119">**Element**</span></span>|<span data-ttu-id="04539-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="04539-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04539-121">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="04539-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="04539-122">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="04539-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="04539-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04539-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="04539-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="04539-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="04539-125">予定表フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="04539-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="04539-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04539-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04539-127">注釈</span><span class="sxs-lookup"><span data-stu-id="04539-127">Remarks</span></span>

<span data-ttu-id="04539-128">[Setfolderfield](setfolderfield.md)要素で updatefolder 操作を使用すると、フォルダーから不明なエントリを削除できます。</span><span class="sxs-lookup"><span data-stu-id="04539-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="04539-129">UpdateFolder 操作の SetFolderField オプションを使用して PermissionSet をリセットすると、不明なエントリが削除されます。</span><span class="sxs-lookup"><span data-stu-id="04539-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="04539-130">Exchange Web サービスでは、個々のエントリの削除はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04539-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="04539-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="04539-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04539-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="04539-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04539-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="04539-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04539-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04539-134">Schema Name</span></span>  <br/> |<span data-ttu-id="04539-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="04539-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="04539-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04539-136">Validation File</span></span>  <br/> |<span data-ttu-id="04539-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="04539-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04539-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04539-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="04539-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="04539-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04539-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="04539-140">See also</span></span>



<span data-ttu-id="04539-141">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="04539-141">[UpdateFolder operation](updatefolder-operation.md)</span></span>


- [<span data-ttu-id="04539-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="04539-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="04539-143">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="04539-143">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

