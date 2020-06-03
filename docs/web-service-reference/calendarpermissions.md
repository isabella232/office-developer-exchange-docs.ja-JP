---
title: CalendarPermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: CalendarPermissions 要素には、フォルダーに対する予定表のアクセス許可の配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: f072339212d0fdff3983fbfb6bc8f53c272350c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529470"
---
# <a name="calendarpermissions"></a><span data-ttu-id="af343-104">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="af343-104">CalendarPermissions</span></span>

<span data-ttu-id="af343-105">**Calendarpermissions**要素には、フォルダーに対する予定表のアクセス許可の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af343-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="af343-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="af343-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="af343-107">**ArrayOfCalendarPermissionsType**</span><span class="sxs-lookup"><span data-stu-id="af343-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af343-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="af343-108">Attributes and elements</span></span>

<span data-ttu-id="af343-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af343-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af343-110">属性</span><span class="sxs-lookup"><span data-stu-id="af343-110">Attributes</span></span>

<span data-ttu-id="af343-111">なし。</span><span class="sxs-lookup"><span data-stu-id="af343-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af343-112">子要素</span><span class="sxs-lookup"><span data-stu-id="af343-112">Child elements</span></span>

|<span data-ttu-id="af343-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="af343-113">**Element**</span></span>|<span data-ttu-id="af343-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="af343-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af343-115">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="af343-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="af343-116">代理ユーザーが予定表フォルダーに対して持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="af343-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af343-117">親要素</span><span class="sxs-lookup"><span data-stu-id="af343-117">Parent elements</span></span>

|<span data-ttu-id="af343-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="af343-118">**Element**</span></span>|<span data-ttu-id="af343-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="af343-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af343-120">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="af343-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="af343-121">予定表フォルダーに対して構成されているアクセス許可がすべて含まれます。</span><span class="sxs-lookup"><span data-stu-id="af343-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="af343-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="af343-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af343-123">注釈</span><span class="sxs-lookup"><span data-stu-id="af343-123">Remarks</span></span>

<span data-ttu-id="af343-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="af343-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af343-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="af343-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af343-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="af343-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af343-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af343-127">Schema Name</span></span>  <br/> |<span data-ttu-id="af343-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="af343-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="af343-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af343-129">Validation File</span></span>  <br/> |<span data-ttu-id="af343-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="af343-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af343-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af343-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="af343-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="af343-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af343-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="af343-133">See also</span></span>



- [<span data-ttu-id="af343-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="af343-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="af343-135">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="af343-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

