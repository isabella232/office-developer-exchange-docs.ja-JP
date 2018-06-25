---
title: 権限
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
description: アクセス許可要素には、フォルダーのアクセス許可のコレクションが含まれています。
ms.openlocfilehash: 08d015c3b1afb58fce0fb4b99466965cc5c29fc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832727"
---
# <a name="permissions"></a><span data-ttu-id="f571d-103">権限</span><span class="sxs-lookup"><span data-stu-id="f571d-103">Permissions</span></span>

<span data-ttu-id="f571d-104">**アクセス許可**要素には、フォルダーのアクセス許可のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f571d-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="f571d-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="f571d-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f571d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f571d-106">Attributes and elements</span></span>

<span data-ttu-id="f571d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f571d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f571d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f571d-108">Attributes</span></span>

<span data-ttu-id="f571d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f571d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f571d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f571d-110">Child elements</span></span>

|<span data-ttu-id="f571d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f571d-111">**Element**</span></span>|<span data-ttu-id="f571d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f571d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f571d-113">Permission</span><span class="sxs-lookup"><span data-stu-id="f571d-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="f571d-114">フォルダーに代理人のアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="f571d-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="f571d-115">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f571d-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f571d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f571d-116">Parent elements</span></span>

|<span data-ttu-id="f571d-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f571d-117">**Element**</span></span>|<span data-ttu-id="f571d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f571d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f571d-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f571d-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="f571d-120">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f571d-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="f571d-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f571d-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f571d-122">備考</span><span class="sxs-lookup"><span data-stu-id="f571d-122">Remarks</span></span>

<span data-ttu-id="f571d-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f571d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f571d-124">この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f571d-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f571d-125">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="f571d-125">Version differences</span></span>

<span data-ttu-id="f571d-126">アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。</span><span class="sxs-lookup"><span data-stu-id="f571d-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="f571d-127">フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="f571d-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f571d-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="f571d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f571d-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="f571d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f571d-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f571d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f571d-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f571d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f571d-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f571d-132">Validation File</span></span>  <br/> |<span data-ttu-id="f571d-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f571d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f571d-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f571d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f571d-135">False</span><span class="sxs-lookup"><span data-stu-id="f571d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f571d-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f571d-136">See also</span></span>



- [<span data-ttu-id="f571d-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f571d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f571d-138">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="f571d-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

