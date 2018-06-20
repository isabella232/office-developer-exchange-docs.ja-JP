---
title: DisplayNamePrefix
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 60363698-7603-4051-a66e-007c02db17cb
description: DisplayNamePrefix 要素は、関連付けられているペルソナの表示名のプレフィックスを指定します。
ms.openlocfilehash: 120a6402be386bc0c11f5859265098324ce4687f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760122"
---
# <a name="displaynameprefix"></a><span data-ttu-id="b7bd7-103">DisplayNamePrefix</span><span class="sxs-lookup"><span data-stu-id="b7bd7-103">DisplayNamePrefix</span></span>

<span data-ttu-id="b7bd7-104">**DisplayNamePrefix**要素は、関連付けられているペルソナの表示名のプレフィックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-104">The **DisplayNamePrefix** element specifies the prefix of the display name of the associated persona.</span></span> 
  
```xml
<DisplayNamePrefix></DisplayNamePrefix>
```

 <span data-ttu-id="b7bd7-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b7bd7-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7bd7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b7bd7-106">Attributes and elements</span></span>

<span data-ttu-id="b7bd7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7bd7-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7bd7-108">Attributes</span></span>

<span data-ttu-id="b7bd7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7bd7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b7bd7-110">Child elements</span></span>

<span data-ttu-id="b7bd7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7bd7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b7bd7-112">Parent elements</span></span>

|<span data-ttu-id="b7bd7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7bd7-113">**Element**</span></span>|<span data-ttu-id="b7bd7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7bd7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7bd7-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="b7bd7-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b7bd7-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7bd7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b7bd7-117">Text value</span></span>

<span data-ttu-id="b7bd7-118">**DisplayNamePrefix**要素のテキスト値は、表示名のプレフィックスを指定する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-118">The text value of the **DisplayNamePrefix** element is a string value that specifies the prefix for the display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b7bd7-119">備考</span><span class="sxs-lookup"><span data-stu-id="b7bd7-119">Remarks</span></span>

<span data-ttu-id="b7bd7-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b7bd7-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7bd7-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="b7bd7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7bd7-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="b7bd7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7bd7-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b7bd7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b7bd7-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="b7bd7-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="b7bd7-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b7bd7-126">Validation File</span></span>  <br/> |<span data-ttu-id="b7bd7-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7bd7-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7bd7-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b7bd7-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b7bd7-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b7bd7-129">See also</span></span>

- [<span data-ttu-id="b7bd7-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b7bd7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

