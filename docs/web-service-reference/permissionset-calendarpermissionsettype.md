---
title: PermissionSet (CalendarPermissionSetType)
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
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: PermissionSet 要素には、予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832728"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="92011-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="92011-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="92011-104">**PermissionSet**要素には、予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92011-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="92011-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="92011-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92011-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="92011-106">Attributes and elements</span></span>

<span data-ttu-id="92011-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92011-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92011-108">属性</span><span class="sxs-lookup"><span data-stu-id="92011-108">Attributes</span></span>

<span data-ttu-id="92011-109">なし。</span><span class="sxs-lookup"><span data-stu-id="92011-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92011-110">子要素</span><span class="sxs-lookup"><span data-stu-id="92011-110">Child elements</span></span>

|<span data-ttu-id="92011-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="92011-111">**Element**</span></span>|<span data-ttu-id="92011-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="92011-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92011-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="92011-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="92011-114">フォルダーのアクセス許可を予定表の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92011-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="92011-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92011-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="92011-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="92011-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="92011-117">Active Directory ディレクトリ サービスに対して解決できない不明なエントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92011-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="92011-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92011-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92011-119">親要素</span><span class="sxs-lookup"><span data-stu-id="92011-119">Parent elements</span></span>

|<span data-ttu-id="92011-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="92011-120">**Element**</span></span>|<span data-ttu-id="92011-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="92011-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92011-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="92011-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="92011-123">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="92011-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92011-124">備考</span><span class="sxs-lookup"><span data-stu-id="92011-124">Remarks</span></span>

<span data-ttu-id="92011-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="92011-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="92011-126">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92011-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="92011-127">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="92011-127">Version differences</span></span>

<span data-ttu-id="92011-128">アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。</span><span class="sxs-lookup"><span data-stu-id="92011-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="92011-129">フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="92011-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="92011-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="92011-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92011-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="92011-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92011-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92011-132">Schema Name</span></span>  <br/> |<span data-ttu-id="92011-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="92011-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="92011-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92011-134">Validation File</span></span>  <br/> |<span data-ttu-id="92011-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92011-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92011-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="92011-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="92011-137">False</span><span class="sxs-lookup"><span data-stu-id="92011-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92011-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="92011-138">See also</span></span>



- [<span data-ttu-id="92011-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="92011-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="92011-140">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="92011-140">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

