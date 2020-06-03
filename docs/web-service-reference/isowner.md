---
title: IsOwner 場合
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: IsOwner 要素は、指定された電子メールユーザーが所有者であるかどうかを指定します。
ms.openlocfilehash: 2dd085aba34052d95efd1e72edca7be4aba71155
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466522"
---
# <a name="isowner"></a><span data-ttu-id="fdb53-103">IsOwner 場合</span><span class="sxs-lookup"><span data-stu-id="fdb53-103">IsOwner</span></span>

<span data-ttu-id="fdb53-104">**Isowner**要素は、指定された電子メールユーザーが所有者であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fdb53-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="fdb53-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fdb53-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdb53-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fdb53-106">Attributes and elements</span></span>

<span data-ttu-id="fdb53-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fdb53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdb53-108">属性</span><span class="sxs-lookup"><span data-stu-id="fdb53-108">Attributes</span></span>

<span data-ttu-id="fdb53-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fdb53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdb53-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fdb53-110">Child elements</span></span>

<span data-ttu-id="fdb53-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fdb53-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdb53-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fdb53-112">Parent elements</span></span>

|<span data-ttu-id="fdb53-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fdb53-113">**Element**</span></span>|<span data-ttu-id="fdb53-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fdb53-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdb53-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="fdb53-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="fdb53-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdb53-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fdb53-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fdb53-117">Text value</span></span>

<span data-ttu-id="fdb53-118">**Isowner**要素のテキスト値が**true の場合**は、ユーザーがアイテムに対して発行された権限の所有者であることを示します。</span><span class="sxs-lookup"><span data-stu-id="fdb53-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="fdb53-119">値が**false**の場合は、ユーザーがアイテムに対して発行された権限の所有者ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="fdb53-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fdb53-120">注釈</span><span class="sxs-lookup"><span data-stu-id="fdb53-120">Remarks</span></span>

<span data-ttu-id="fdb53-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fdb53-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fdb53-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fdb53-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdb53-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fdb53-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdb53-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fdb53-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fdb53-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fdb53-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fdb53-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="fdb53-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="fdb53-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fdb53-127">Validation File</span></span>  <br/> |<span data-ttu-id="fdb53-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fdb53-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fdb53-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fdb53-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fdb53-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="fdb53-130">See also</span></span>



- [<span data-ttu-id="fdb53-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fdb53-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

