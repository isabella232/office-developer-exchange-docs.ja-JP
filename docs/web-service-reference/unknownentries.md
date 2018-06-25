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
description: UnknownEntries 要素には、Active Directory ディレクトリ サービスに対して解決できない不明なアクセス許可エントリの配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 306e5f226a56694bb1ff32362f77e7dff80865ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839808"
---
# <a name="unknownentries"></a><span data-ttu-id="6a908-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="6a908-104">UnknownEntries</span></span>

<span data-ttu-id="6a908-105">**UnknownEntries**要素には、Active Directory ディレクトリ サービスに対して解決できない不明なアクセス許可エントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a908-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="6a908-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a908-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="6a908-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="6a908-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a908-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a908-108">Attributes and elements</span></span>

<span data-ttu-id="6a908-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a908-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a908-110">属性</span><span class="sxs-lookup"><span data-stu-id="6a908-110">Attributes</span></span>

<span data-ttu-id="6a908-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6a908-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a908-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6a908-112">Child elements</span></span>

|<span data-ttu-id="6a908-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a908-113">**Element**</span></span>|<span data-ttu-id="6a908-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a908-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a908-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="6a908-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="6a908-116">Active Directory に対して解決することができない 1 つの不明なアクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="6a908-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="6a908-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a908-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a908-118">親要素</span><span class="sxs-lookup"><span data-stu-id="6a908-118">Parent elements</span></span>

|<span data-ttu-id="6a908-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a908-119">**Element**</span></span>|<span data-ttu-id="6a908-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a908-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a908-121">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="6a908-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="6a908-122">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a908-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="6a908-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a908-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6a908-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="6a908-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="6a908-125">予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a908-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="6a908-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a908-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a908-127">備考</span><span class="sxs-lookup"><span data-stu-id="6a908-127">Remarks</span></span>

<span data-ttu-id="6a908-128">UpdateFolder 操作を使用して[SetFolderField](setfolderfield.md)要素を使用して、フォルダーからの不明なエントリを削除できます。</span><span class="sxs-lookup"><span data-stu-id="6a908-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="6a908-129">UpdateFolder 操作の SetFolderField オプションを使用して、PermissionSet をリセットすると、不明なエントリが削除されます。</span><span class="sxs-lookup"><span data-stu-id="6a908-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="6a908-130">Exchange Web サービスは、個々 のエントリの削除をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="6a908-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="6a908-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6a908-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a908-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a908-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a908-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a908-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a908-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a908-134">Schema Name</span></span>  <br/> |<span data-ttu-id="6a908-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6a908-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a908-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a908-136">Validation File</span></span>  <br/> |<span data-ttu-id="6a908-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a908-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a908-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a908-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a908-139">False</span><span class="sxs-lookup"><span data-stu-id="6a908-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a908-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a908-140">See also</span></span>



<span data-ttu-id="6a908-141">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="6a908-141">[UpdateFolder operation](updatefolder-operation.md)</span></span>


- [<span data-ttu-id="6a908-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a908-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6a908-143">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="6a908-143">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

