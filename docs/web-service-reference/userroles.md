---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: UserRoles 要素は、呼び出し元のユーザー、または通話パートナーアプリケーションが動作しているユーザーが現在の呼び出しに適用するユーザーの役割を指定します。
ms.openlocfilehash: 5155b82781321b16d1b58fdcaffe7b8cf2372717
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467131"
---
# <a name="userroles"></a><span data-ttu-id="56e7d-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="56e7d-103">UserRoles</span></span>

<span data-ttu-id="56e7d-104">**Userroles**要素は、呼び出し元のユーザー、または通話パートナーアプリケーションが動作しているユーザーが現在の呼び出しに適用するユーザーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e7d-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="56e7d-105">**非 Emptyarrayofroletype**</span><span class="sxs-lookup"><span data-stu-id="56e7d-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56e7d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56e7d-106">Attributes and elements</span></span>

<span data-ttu-id="56e7d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56e7d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56e7d-108">属性</span><span class="sxs-lookup"><span data-stu-id="56e7d-108">Attributes</span></span>

<span data-ttu-id="56e7d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="56e7d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56e7d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="56e7d-110">Child elements</span></span>

[<span data-ttu-id="56e7d-111">役割</span><span class="sxs-lookup"><span data-stu-id="56e7d-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="56e7d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="56e7d-112">Parent elements</span></span>

[<span data-ttu-id="56e7d-113">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="56e7d-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="56e7d-114">注釈</span><span class="sxs-lookup"><span data-stu-id="56e7d-114">Remarks</span></span>

<span data-ttu-id="56e7d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="56e7d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56e7d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="56e7d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56e7d-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="56e7d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56e7d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="56e7d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56e7d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56e7d-119">Schema name</span></span>  <br/> |<span data-ttu-id="56e7d-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="56e7d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="56e7d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56e7d-121">Validation file</span></span>  <br/> |<span data-ttu-id="56e7d-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="56e7d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56e7d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="56e7d-123">Can be empty</span></span>  <br/> ||
   

