---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: IsOwner 要素は、指定された電子メールのユーザーは、所有者であるかどうかを指定します。
ms.openlocfilehash: aac3c2a599093282542025468d73c55ec4569e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832080"
---
# <a name="isowner"></a><span data-ttu-id="847f9-103">IsOwner</span><span class="sxs-lookup"><span data-stu-id="847f9-103">IsOwner</span></span>

<span data-ttu-id="847f9-104">**IsOwner**要素は、指定された電子メールのユーザーは、所有者であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="847f9-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="847f9-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="847f9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="847f9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="847f9-106">Attributes and elements</span></span>

<span data-ttu-id="847f9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="847f9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="847f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="847f9-108">Attributes</span></span>

<span data-ttu-id="847f9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="847f9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="847f9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="847f9-110">Child elements</span></span>

<span data-ttu-id="847f9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="847f9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="847f9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="847f9-112">Parent elements</span></span>

|<span data-ttu-id="847f9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="847f9-113">**Element**</span></span>|<span data-ttu-id="847f9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="847f9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="847f9-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="847f9-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="847f9-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="847f9-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="847f9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="847f9-117">Text value</span></span>

<span data-ttu-id="847f9-118">の**場合は true** 、 **IsOwner**要素のテキスト値は、ユーザーが項目を発行する権限の所有者であることを示します。</span><span class="sxs-lookup"><span data-stu-id="847f9-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="847f9-119">**False**の値は、ユーザーが項目を発行する権限の所有者ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="847f9-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="847f9-120">備考</span><span class="sxs-lookup"><span data-stu-id="847f9-120">Remarks</span></span>

<span data-ttu-id="847f9-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="847f9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="847f9-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="847f9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="847f9-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="847f9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="847f9-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="847f9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="847f9-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="847f9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="847f9-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="847f9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="847f9-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="847f9-127">Validation File</span></span>  <br/> |<span data-ttu-id="847f9-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="847f9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="847f9-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="847f9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="847f9-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="847f9-130">See also</span></span>



- [<span data-ttu-id="847f9-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="847f9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

