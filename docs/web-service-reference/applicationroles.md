---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: ApplicationRoles 要素は、呼び出し元パートナーアプリケーションが現在の呼び出しに対して使用するアプリケーションロールを指定します。
ms.openlocfilehash: 8dfe5c745896d02217cbf91375d355954a4e22eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464701"
---
# <a name="applicationroles"></a><span data-ttu-id="1bf30-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="1bf30-103">ApplicationRoles</span></span>

<span data-ttu-id="1bf30-104">**Applicationroles**要素は、呼び出し元パートナーアプリケーションが現在の呼び出しに対して使用するアプリケーションロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="1bf30-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="1bf30-105">**非 Emptyarrayofroletype**</span><span class="sxs-lookup"><span data-stu-id="1bf30-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bf30-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1bf30-106">Attributes and elements</span></span>

<span data-ttu-id="1bf30-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1bf30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bf30-108">属性</span><span class="sxs-lookup"><span data-stu-id="1bf30-108">Attributes</span></span>

<span data-ttu-id="1bf30-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1bf30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bf30-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1bf30-110">Child elements</span></span>

|<span data-ttu-id="1bf30-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1bf30-111">**Element**</span></span>|<span data-ttu-id="1bf30-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1bf30-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bf30-113">役割</span><span class="sxs-lookup"><span data-stu-id="1bf30-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="1bf30-114">管理役割を表す文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bf30-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bf30-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1bf30-115">Parent elements</span></span>

|<span data-ttu-id="1bf30-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1bf30-116">**Element**</span></span>|<span data-ttu-id="1bf30-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1bf30-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bf30-118">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="1bf30-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="1bf30-119">管理役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bf30-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1bf30-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1bf30-120">Remarks</span></span>

<span data-ttu-id="1bf30-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1bf30-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1bf30-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1bf30-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bf30-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1bf30-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bf30-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1bf30-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1bf30-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1bf30-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1bf30-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1bf30-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1bf30-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1bf30-127">Validation File</span></span>  <br/> |<span data-ttu-id="1bf30-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1bf30-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1bf30-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1bf30-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1bf30-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1bf30-130">See also</span></span>

- [<span data-ttu-id="1bf30-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1bf30-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

