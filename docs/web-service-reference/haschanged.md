---
title: HasChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 15ff513d-f39e-44ed-a13f-ab3f86fa37e1
description: HasChanged 要素は、ユーザーの写真が変更されたかどうかを示します。
ms.openlocfilehash: d777220f55d33cde548d8257cf249b57481a43f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462788"
---
# <a name="haschanged"></a><span data-ttu-id="c5295-103">HasChanged</span><span class="sxs-lookup"><span data-stu-id="c5295-103">HasChanged</span></span>

<span data-ttu-id="c5295-104">**Haschanged**要素は、ユーザーの写真が変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5295-104">The **HasChanged** element indicates whether a user's photo has changed.</span></span> 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="c5295-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5295-105">Attributes and elements</span></span>

<span data-ttu-id="c5295-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5295-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5295-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5295-107">Attributes</span></span>

<span data-ttu-id="c5295-108">なし。</span><span class="sxs-lookup"><span data-stu-id="c5295-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5295-109">子要素</span><span class="sxs-lookup"><span data-stu-id="c5295-109">Child elements</span></span>

<span data-ttu-id="c5295-110">なし。</span><span class="sxs-lookup"><span data-stu-id="c5295-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5295-111">親要素</span><span class="sxs-lookup"><span data-stu-id="c5295-111">Parent elements</span></span>

[<span data-ttu-id="c5295-112">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="c5295-112">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
  
## <a name="text-value"></a><span data-ttu-id="c5295-113">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5295-113">Text value</span></span>

<span data-ttu-id="c5295-114">**Haschanged**要素のテキスト値が**true**の場合は、写真が最後に返されてから変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="c5295-114">A text value of **true** for the **HasChanged** element indicates that the photo has changed since the last time it was returned.</span></span> <span data-ttu-id="c5295-115">値が**false**の場合、写真が最後に返されてから変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c5295-115">A value of **false** indicates that the photo has not changed since the last time it was returned.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c5295-116">注釈</span><span class="sxs-lookup"><span data-stu-id="c5295-116">Remarks</span></span>

<span data-ttu-id="c5295-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c5295-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c5295-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c5295-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5295-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5295-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5295-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5295-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5295-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5295-121">Schema name</span></span>  <br/> |<span data-ttu-id="c5295-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5295-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5295-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5295-123">Validation file</span></span>  <br/> |<span data-ttu-id="c5295-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5295-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5295-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c5295-125">Can be empty</span></span>  <br/> ||
   

