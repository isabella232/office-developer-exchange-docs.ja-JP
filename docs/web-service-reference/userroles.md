---
title: 作成します
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: 作成します要素は、呼び出し元のユーザー、または、呼び出し先のアプリケーションが動作しているユーザーが現在の呼び出しに適用する必要があるユーザーのロールを指定します。
ms.openlocfilehash: 19dc1a7e00decb9141326b53b650d72101013c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839950"
---
# <a name="userroles"></a><span data-ttu-id="99514-103">作成します</span><span class="sxs-lookup"><span data-stu-id="99514-103">UserRoles</span></span>

<span data-ttu-id="99514-104">**作成します**要素は、呼び出し元のユーザー、または、呼び出し先のアプリケーションが動作しているユーザーが現在の呼び出しに適用する必要があるユーザーのロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="99514-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="99514-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="99514-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99514-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="99514-106">Attributes and elements</span></span>

<span data-ttu-id="99514-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="99514-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99514-108">属性</span><span class="sxs-lookup"><span data-stu-id="99514-108">Attributes</span></span>

<span data-ttu-id="99514-109">なし。</span><span class="sxs-lookup"><span data-stu-id="99514-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99514-110">子要素</span><span class="sxs-lookup"><span data-stu-id="99514-110">Child elements</span></span>

[<span data-ttu-id="99514-111">Role</span><span class="sxs-lookup"><span data-stu-id="99514-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="99514-112">親要素</span><span class="sxs-lookup"><span data-stu-id="99514-112">Parent elements</span></span>

[<span data-ttu-id="99514-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="99514-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="99514-114">備考</span><span class="sxs-lookup"><span data-stu-id="99514-114">Remarks</span></span>

<span data-ttu-id="99514-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="99514-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="99514-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="99514-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99514-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="99514-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99514-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="99514-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99514-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="99514-119">Schema name</span></span>  <br/> |<span data-ttu-id="99514-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="99514-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="99514-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="99514-121">Validation file</span></span>  <br/> |<span data-ttu-id="99514-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="99514-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99514-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="99514-123">Can be empty</span></span>  <br/> ||
   

