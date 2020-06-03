---
title: ReplyAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 880af57e-0fa1-473c-b87c-f02f1133ba5e
description: ReplyAllowed 要素は、権限管理データに対して返信を許可するかどうかを指定します。
ms.openlocfilehash: f9aa97fc5d85837323d6d9e3e1e13c7b9fd11715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529862"
---
# <a name="replyallowed"></a><span data-ttu-id="05472-103">ReplyAllowed</span><span class="sxs-lookup"><span data-stu-id="05472-103">ReplyAllowed</span></span>

<span data-ttu-id="05472-104">**ReplyAllowed**要素は、権限管理データに対して返信を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="05472-104">The **ReplyAllowed** element specifies whether a reply is allowed for rights managed data.</span></span> 
  
```XML
<ReplyAllowed> true | false </ReplyAllowed>
```

 <span data-ttu-id="05472-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="05472-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05472-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="05472-106">Attributes and elements</span></span>

<span data-ttu-id="05472-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05472-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05472-108">属性</span><span class="sxs-lookup"><span data-stu-id="05472-108">Attributes</span></span>

<span data-ttu-id="05472-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05472-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05472-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05472-110">Child elements</span></span>

<span data-ttu-id="05472-111">なし。</span><span class="sxs-lookup"><span data-stu-id="05472-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05472-112">親要素</span><span class="sxs-lookup"><span data-stu-id="05472-112">Parent elements</span></span>

[<span data-ttu-id="05472-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="05472-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="05472-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05472-114">Text value</span></span>

<span data-ttu-id="05472-115">**ReplyAllowed**要素のテキスト値が**true**の場合は、権限管理データに対して返信が許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="05472-115">A text value of **true** for the **ReplyAllowed** element indicates that replies are allowed for the rights managed data.</span></span> <span data-ttu-id="05472-116">値が**false**の場合は、返信が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="05472-116">A value of **false** indicates that replies are not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="05472-117">注釈</span><span class="sxs-lookup"><span data-stu-id="05472-117">Remarks</span></span>

<span data-ttu-id="05472-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="05472-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05472-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="05472-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05472-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="05472-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05472-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="05472-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05472-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05472-122">Schema name</span></span>  <br/> |<span data-ttu-id="05472-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="05472-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="05472-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05472-124">Validation file</span></span>  <br/> |<span data-ttu-id="05472-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="05472-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05472-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="05472-126">Can be empty</span></span>  <br/> ||
   

