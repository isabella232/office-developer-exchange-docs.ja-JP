---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: ApplicationRoles 要素は、現在の呼び出しの呼び出し元のパートナーのアプリケーションを使用するアプリケーション ロールを指定します。
ms.openlocfilehash: ff32b693dae573416263bcb7c0fbb552a933b8d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759334"
---
# <a name="applicationroles"></a><span data-ttu-id="367ec-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="367ec-103">ApplicationRoles</span></span>

<span data-ttu-id="367ec-104">**ApplicationRoles**要素は、現在の呼び出しの呼び出し元のパートナーのアプリケーションを使用するアプリケーション ロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="367ec-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="367ec-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="367ec-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="367ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="367ec-106">Attributes and elements</span></span>

<span data-ttu-id="367ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="367ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="367ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="367ec-108">Attributes</span></span>

<span data-ttu-id="367ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="367ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="367ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="367ec-110">Child elements</span></span>

|<span data-ttu-id="367ec-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="367ec-111">**Element**</span></span>|<span data-ttu-id="367ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="367ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="367ec-113">Role</span><span class="sxs-lookup"><span data-stu-id="367ec-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="367ec-114">管理ロールを表す文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="367ec-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="367ec-115">親要素</span><span class="sxs-lookup"><span data-stu-id="367ec-115">Parent elements</span></span>

|<span data-ttu-id="367ec-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="367ec-116">**Element**</span></span>|<span data-ttu-id="367ec-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="367ec-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="367ec-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="367ec-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="367ec-119">管理の役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="367ec-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="367ec-120">備考</span><span class="sxs-lookup"><span data-stu-id="367ec-120">Remarks</span></span>

<span data-ttu-id="367ec-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="367ec-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="367ec-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="367ec-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="367ec-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="367ec-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="367ec-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="367ec-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="367ec-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="367ec-125">Schema Name</span></span>  <br/> |<span data-ttu-id="367ec-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="367ec-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="367ec-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="367ec-127">Validation File</span></span>  <br/> |<span data-ttu-id="367ec-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="367ec-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="367ec-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="367ec-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="367ec-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="367ec-130">See also</span></span>

- [<span data-ttu-id="367ec-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="367ec-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

