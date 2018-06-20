---
title: HomeCity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 410efc09-5c38-46fb-85b5-eb365be0ba35
description: HomeCity 要素は、関連付けられているペルソナの自宅の住所の市区町村を指定します。
ms.openlocfilehash: 1d9c3153d3c6232082f699697fc7faf108b43c70
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831832"
---
# <a name="homecity"></a><span data-ttu-id="9cab5-103">HomeCity</span><span class="sxs-lookup"><span data-stu-id="9cab5-103">HomeCity</span></span>

<span data-ttu-id="9cab5-104">**HomeCity**要素は、関連付けられているペルソナの自宅の住所の市区町村を指定します。</span><span class="sxs-lookup"><span data-stu-id="9cab5-104">The **HomeCity** element specifies the city of the home address of the associated persona.</span></span> 
  
```XML
<HomeCity></HomeCity>
```

 <span data-ttu-id="9cab5-105">**string**</span><span class="sxs-lookup"><span data-stu-id="9cab5-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cab5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9cab5-106">Attributes and elements</span></span>

<span data-ttu-id="9cab5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9cab5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cab5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cab5-108">Attributes</span></span>

<span data-ttu-id="9cab5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9cab5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cab5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9cab5-110">Child elements</span></span>

<span data-ttu-id="9cab5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cab5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cab5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9cab5-112">Parent elements</span></span>

|<span data-ttu-id="9cab5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9cab5-113">**Element**</span></span>|<span data-ttu-id="9cab5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cab5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cab5-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="9cab5-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9cab5-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="9cab5-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cab5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9cab5-117">Text value</span></span>

<span data-ttu-id="9cab5-118">**HomeCity**要素のテキスト値は、市区町村名を指定する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="9cab5-118">The text value of the **HomeCity** element is a string value that specifies the city.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9cab5-119">備考</span><span class="sxs-lookup"><span data-stu-id="9cab5-119">Remarks</span></span>

<span data-ttu-id="9cab5-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9cab5-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9cab5-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9cab5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cab5-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9cab5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cab5-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9cab5-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cab5-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9cab5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9cab5-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="9cab5-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9cab5-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9cab5-126">Validation File</span></span>  <br/> |<span data-ttu-id="9cab5-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9cab5-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cab5-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9cab5-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9cab5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9cab5-129">See also</span></span>



- [<span data-ttu-id="9cab5-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9cab5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

