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
ms.openlocfilehash: b0129e3d3acb43ada16a824e3d21706999d7053c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831802"
---
# <a name="haschanged"></a><span data-ttu-id="fe52a-103">HasChanged</span><span class="sxs-lookup"><span data-stu-id="fe52a-103">HasChanged</span></span>

<span data-ttu-id="fe52a-104">**HasChanged**要素は、ユーザーの写真が変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fe52a-104">The **HasChanged** element indicates whether a user's photo has changed.</span></span> 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="fe52a-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fe52a-105">Attributes and elements</span></span>

<span data-ttu-id="fe52a-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe52a-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe52a-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe52a-107">Attributes</span></span>

<span data-ttu-id="fe52a-108">なし。</span><span class="sxs-lookup"><span data-stu-id="fe52a-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe52a-109">子要素</span><span class="sxs-lookup"><span data-stu-id="fe52a-109">Child elements</span></span>

<span data-ttu-id="fe52a-110">なし。</span><span class="sxs-lookup"><span data-stu-id="fe52a-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe52a-111">親要素</span><span class="sxs-lookup"><span data-stu-id="fe52a-111">Parent elements</span></span>

[<span data-ttu-id="fe52a-112">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="fe52a-112">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
  
## <a name="text-value"></a><span data-ttu-id="fe52a-113">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fe52a-113">Text value</span></span>

<span data-ttu-id="fe52a-114">の**場合は true** 、 **HasChanged**要素のテキスト値は、最後に返された後の写真が変更されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="fe52a-114">A text value of **true** for the **HasChanged** element indicates that the photo has changed since the last time it was returned.</span></span> <span data-ttu-id="fe52a-115">**False**の値は、最後に返された後、写真が変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="fe52a-115">A value of **false** indicates that the photo has not changed since the last time it was returned.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fe52a-116">備考</span><span class="sxs-lookup"><span data-stu-id="fe52a-116">Remarks</span></span>

<span data-ttu-id="fe52a-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fe52a-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fe52a-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fe52a-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe52a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="fe52a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe52a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="fe52a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe52a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fe52a-121">Schema name</span></span>  <br/> |<span data-ttu-id="fe52a-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fe52a-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe52a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fe52a-123">Validation file</span></span>  <br/> |<span data-ttu-id="fe52a-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fe52a-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe52a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fe52a-125">Can be empty</span></span>  <br/> ||
   

