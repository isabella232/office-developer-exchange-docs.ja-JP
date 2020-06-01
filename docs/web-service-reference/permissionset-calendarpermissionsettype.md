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
ms.openlocfilehash: 9564608397ac8a5ab0ddd4508eacd8cad665d76e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458034"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="87ebd-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="87ebd-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="87ebd-104">**PermissionSet**要素には、予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="87ebd-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="87ebd-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="87ebd-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87ebd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="87ebd-106">Attributes and elements</span></span>

<span data-ttu-id="87ebd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="87ebd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87ebd-108">属性</span><span class="sxs-lookup"><span data-stu-id="87ebd-108">Attributes</span></span>

<span data-ttu-id="87ebd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="87ebd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87ebd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="87ebd-110">Child elements</span></span>

|<span data-ttu-id="87ebd-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="87ebd-111">**Element**</span></span>|<span data-ttu-id="87ebd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="87ebd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87ebd-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="87ebd-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="87ebd-114">フォルダーに対する予定表のアクセス許可の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="87ebd-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="87ebd-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="87ebd-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="87ebd-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="87ebd-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="87ebd-117">Active Directory ディレクトリサービスに対して解決できない不明なエントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="87ebd-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="87ebd-118">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="87ebd-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87ebd-119">親要素</span><span class="sxs-lookup"><span data-stu-id="87ebd-119">Parent elements</span></span>

|<span data-ttu-id="87ebd-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="87ebd-120">**Element**</span></span>|<span data-ttu-id="87ebd-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="87ebd-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87ebd-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="87ebd-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="87ebd-123">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="87ebd-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87ebd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="87ebd-124">Remarks</span></span>

<span data-ttu-id="87ebd-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="87ebd-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="87ebd-126">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="87ebd-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="87ebd-127">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="87ebd-127">Version differences</span></span>

<span data-ttu-id="87ebd-128">Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。</span><span class="sxs-lookup"><span data-stu-id="87ebd-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="87ebd-129">フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="87ebd-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="87ebd-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="87ebd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87ebd-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="87ebd-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87ebd-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="87ebd-132">Schema Name</span></span>  <br/> |<span data-ttu-id="87ebd-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="87ebd-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="87ebd-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="87ebd-134">Validation File</span></span>  <br/> |<span data-ttu-id="87ebd-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="87ebd-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87ebd-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="87ebd-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="87ebd-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="87ebd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87ebd-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="87ebd-138">See also</span></span>



- [<span data-ttu-id="87ebd-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="87ebd-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="87ebd-140">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="87ebd-140">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

