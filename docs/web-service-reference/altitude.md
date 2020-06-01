---
title: Altitude
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 14c2c8bd-db54-4b03-9a97-190ff9e908b3
description: 標高要素は、郵送先住所の高度を指定します。
ms.openlocfilehash: 7cbb3872cd0ad53b1617f9f712633e19e6fe397d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458839"
---
# <a name="altitude"></a><span data-ttu-id="b03dc-103">Altitude</span><span class="sxs-lookup"><span data-stu-id="b03dc-103">Altitude</span></span>

<span data-ttu-id="b03dc-104">**標高**要素は、郵送先住所の高度を指定します。</span><span class="sxs-lookup"><span data-stu-id="b03dc-104">The **Altitude** element specifies the altitude of a postal address.</span></span> 
  
```XML
<Altitude></Altitude>
```

 <span data-ttu-id="b03dc-105">**xs: double**</span><span class="sxs-lookup"><span data-stu-id="b03dc-105">**xs:double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b03dc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b03dc-106">Attributes and elements</span></span>

<span data-ttu-id="b03dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b03dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b03dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="b03dc-108">Attributes</span></span>

<span data-ttu-id="b03dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b03dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b03dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b03dc-110">Child elements</span></span>

<span data-ttu-id="b03dc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b03dc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b03dc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b03dc-112">Parent elements</span></span>

|<span data-ttu-id="b03dc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b03dc-113">**Element**</span></span>|<span data-ttu-id="b03dc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b03dc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b03dc-115">"Postaladdress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="b03dc-115">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="b03dc-116">場所の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="b03dc-116">Specifies the postal address of the location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b03dc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b03dc-117">Text value</span></span>

<span data-ttu-id="b03dc-118">標高要素のテキスト値は、郵送先住所の高度です。</span><span class="sxs-lookup"><span data-stu-id="b03dc-118">The text value of the Altitude element is the altitude of a postal address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b03dc-119">注釈</span><span class="sxs-lookup"><span data-stu-id="b03dc-119">Remarks</span></span>

<span data-ttu-id="b03dc-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b03dc-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b03dc-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b03dc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b03dc-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b03dc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b03dc-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b03dc-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b03dc-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b03dc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b03dc-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="b03dc-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="b03dc-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b03dc-126">Validation File</span></span>  <br/> |<span data-ttu-id="b03dc-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b03dc-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b03dc-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b03dc-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b03dc-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b03dc-129">See also</span></span>

- [<span data-ttu-id="b03dc-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b03dc-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

