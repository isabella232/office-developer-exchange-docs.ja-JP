---
title: ReplyAllAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d22f68cf-b18b-45d0-a9ff-414b7db0e67e
description: ReplyAllAllowed 要素は、すべての返信を権限管理データに対して許可するかどうかを指定します。
ms.openlocfilehash: 56dfe7670ed87581999bfe0a340bcc72c99d04ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467915"
---
# <a name="replyallallowed"></a><span data-ttu-id="de8ba-103">ReplyAllAllowed</span><span class="sxs-lookup"><span data-stu-id="de8ba-103">ReplyAllAllowed</span></span>

<span data-ttu-id="de8ba-104">**ReplyAllAllowed**要素は、すべての返信を権限管理データに対して許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="de8ba-104">The **ReplyAllAllowed** element specifies whether a reply all is allowed for rights managed data.</span></span> 
  
```XML
<ReplyAllAllowed> true | false </ReplyAllAllowed>
```

 <span data-ttu-id="de8ba-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="de8ba-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de8ba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="de8ba-106">Attributes and elements</span></span>

<span data-ttu-id="de8ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="de8ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de8ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="de8ba-108">Attributes</span></span>

<span data-ttu-id="de8ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="de8ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de8ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="de8ba-110">Child elements</span></span>

<span data-ttu-id="de8ba-111">なし。</span><span class="sxs-lookup"><span data-stu-id="de8ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de8ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="de8ba-112">Parent elements</span></span>

[<span data-ttu-id="de8ba-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="de8ba-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="de8ba-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="de8ba-114">Text value</span></span>

<span data-ttu-id="de8ba-115">**ReplyAllAllowed**要素のテキスト値が**true**の場合は、すべての返信が権限管理データに対して許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="de8ba-115">A text value of **true** for the **ReplyAllAllowed** element indicates that a reply all is allowed for the rights managed data.</span></span> <span data-ttu-id="de8ba-116">値が**false**の場合は、全員に返信が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="de8ba-116">A value of **false** indicates that a reply all is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="de8ba-117">注釈</span><span class="sxs-lookup"><span data-stu-id="de8ba-117">Remarks</span></span>

<span data-ttu-id="de8ba-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="de8ba-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="de8ba-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="de8ba-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de8ba-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="de8ba-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de8ba-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="de8ba-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de8ba-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="de8ba-122">Schema name</span></span>  <br/> |<span data-ttu-id="de8ba-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="de8ba-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="de8ba-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="de8ba-124">Validation file</span></span>  <br/> |<span data-ttu-id="de8ba-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="de8ba-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de8ba-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="de8ba-126">Can be empty</span></span>  <br/> ||
   

