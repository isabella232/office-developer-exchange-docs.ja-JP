---
title: 属性 (string)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 736be0bc-12c4-410e-bd17-a89f996ac432
description: 属性要素は、ペルソナの属性を識別するために使用される文字列を指定します。
ms.openlocfilehash: 9a3243904c02c3bdeea7e4a4e7dcb240d4ad3563
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464162"
---
# <a name="attribution-string"></a><span data-ttu-id="01272-103">属性 (string)</span><span class="sxs-lookup"><span data-stu-id="01272-103">Attribution (string)</span></span>

<span data-ttu-id="01272-104">属性**要素は、ペルソナ**の属性を識別するために使用される文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="01272-104">The **Attribution** element specifies a string used to identify an attribute of a persona.</span></span> 
  
```XML
<Attribution></Attribution>
```

 <span data-ttu-id="01272-105">**xs: 文字列**</span><span class="sxs-lookup"><span data-stu-id="01272-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01272-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01272-106">Attributes and elements</span></span>

<span data-ttu-id="01272-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01272-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01272-108">属性</span><span class="sxs-lookup"><span data-stu-id="01272-108">Attributes</span></span>

<span data-ttu-id="01272-109">なし。</span><span class="sxs-lookup"><span data-stu-id="01272-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01272-110">子要素</span><span class="sxs-lookup"><span data-stu-id="01272-110">Child elements</span></span>

<span data-ttu-id="01272-111">なし。</span><span class="sxs-lookup"><span data-stu-id="01272-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01272-112">親要素</span><span class="sxs-lookup"><span data-stu-id="01272-112">Parent elements</span></span>

|<span data-ttu-id="01272-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="01272-113">**Element**</span></span>|<span data-ttu-id="01272-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="01272-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01272-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="01272-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="01272-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="01272-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01272-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01272-117">Text value</span></span>

<span data-ttu-id="01272-118">**属性**要素のテキスト値は、プロパティ値を送信元の連絡先に属性する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="01272-118">The text value of the **attribution** element is a string value that attributes a property value to the source contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01272-119">注釈</span><span class="sxs-lookup"><span data-stu-id="01272-119">Remarks</span></span>

<span data-ttu-id="01272-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="01272-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01272-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01272-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01272-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01272-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01272-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="01272-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01272-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01272-124">Schema Name</span></span>  <br/> |<span data-ttu-id="01272-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="01272-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="01272-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01272-126">Validation File</span></span>  <br/> |<span data-ttu-id="01272-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="01272-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="01272-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01272-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="01272-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="01272-129">See also</span></span>

- [<span data-ttu-id="01272-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="01272-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

