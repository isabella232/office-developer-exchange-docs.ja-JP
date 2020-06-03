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
ms.openlocfilehash: 25fccaf0441fa3d9e258ae35f938ad0fc7a5a9eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460870"
---
# <a name="homecity"></a><span data-ttu-id="60acc-103">HomeCity</span><span class="sxs-lookup"><span data-stu-id="60acc-103">HomeCity</span></span>

<span data-ttu-id="60acc-104">**HomeCity**要素は、関連付けられているペルソナの自宅の住所の市区町村を指定します。</span><span class="sxs-lookup"><span data-stu-id="60acc-104">The **HomeCity** element specifies the city of the home address of the associated persona.</span></span> 
  
```XML
<HomeCity></HomeCity>
```

 <span data-ttu-id="60acc-105">**string**</span><span class="sxs-lookup"><span data-stu-id="60acc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60acc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="60acc-106">Attributes and elements</span></span>

<span data-ttu-id="60acc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60acc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60acc-108">属性</span><span class="sxs-lookup"><span data-stu-id="60acc-108">Attributes</span></span>

<span data-ttu-id="60acc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="60acc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60acc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="60acc-110">Child elements</span></span>

<span data-ttu-id="60acc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="60acc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60acc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="60acc-112">Parent elements</span></span>

|<span data-ttu-id="60acc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="60acc-113">**Element**</span></span>|<span data-ttu-id="60acc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="60acc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60acc-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="60acc-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="60acc-116">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="60acc-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60acc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="60acc-117">Text value</span></span>

<span data-ttu-id="60acc-118">**HomeCity**要素のテキスト値は、市区町村を指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="60acc-118">The text value of the **HomeCity** element is a string value that specifies the city.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="60acc-119">注釈</span><span class="sxs-lookup"><span data-stu-id="60acc-119">Remarks</span></span>

<span data-ttu-id="60acc-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="60acc-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="60acc-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="60acc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60acc-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="60acc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60acc-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="60acc-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60acc-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60acc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="60acc-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="60acc-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="60acc-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60acc-126">Validation File</span></span>  <br/> |<span data-ttu-id="60acc-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="60acc-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="60acc-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="60acc-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="60acc-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="60acc-129">See also</span></span>



- [<span data-ttu-id="60acc-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="60acc-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

