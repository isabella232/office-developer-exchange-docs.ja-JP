---
title: AltitudeAccuracy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aadc1f90-e9ab-4411-b51f-2d43e5e22f2a
description: AltitudeAccuracy 要素は、郵送先住所の高度なプロパティの精度を指定します。
ms.openlocfilehash: 3025982baae130421e5d48aa76ea8dc073f7a656
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464750"
---
# <a name="altitudeaccuracy"></a><span data-ttu-id="98e9f-103">AltitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="98e9f-103">AltitudeAccuracy</span></span>

<span data-ttu-id="98e9f-104">**AltitudeAccuracy**要素は、郵送先住所の高度なプロパティの精度を指定します。</span><span class="sxs-lookup"><span data-stu-id="98e9f-104">The **AltitudeAccuracy** element specifies the accuracy of the altitude property for a postal address.</span></span> 
  
```XML
<AltitudeAccuracy></AltitudeAccuracy>
```

 <span data-ttu-id="98e9f-105">**xs: double**</span><span class="sxs-lookup"><span data-stu-id="98e9f-105">**xs:double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98e9f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="98e9f-106">Attributes and elements</span></span>

<span data-ttu-id="98e9f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="98e9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98e9f-108">属性</span><span class="sxs-lookup"><span data-stu-id="98e9f-108">Attributes</span></span>

<span data-ttu-id="98e9f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="98e9f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98e9f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="98e9f-110">Child elements</span></span>

<span data-ttu-id="98e9f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="98e9f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98e9f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="98e9f-112">Parent elements</span></span>

|<span data-ttu-id="98e9f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="98e9f-113">**Element**</span></span>|<span data-ttu-id="98e9f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="98e9f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98e9f-115">"Postaladdress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="98e9f-115">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="98e9f-116">場所の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="98e9f-116">Specifies the postal address of the location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98e9f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="98e9f-117">Text value</span></span>

<span data-ttu-id="98e9f-118">**AltitudeAccuracy**要素のテキスト値は、郵送先住所の標高プロパティの正確な推定値です。</span><span class="sxs-lookup"><span data-stu-id="98e9f-118">The text value of the **AltitudeAccuracy** element is the accuracy estimate for the altitude property of a postal address.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="98e9f-119">注釈</span><span class="sxs-lookup"><span data-stu-id="98e9f-119">Remarks</span></span>

<span data-ttu-id="98e9f-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="98e9f-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="98e9f-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="98e9f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98e9f-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="98e9f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98e9f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="98e9f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98e9f-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="98e9f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="98e9f-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="98e9f-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="98e9f-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="98e9f-126">Validation File</span></span>  <br/> |<span data-ttu-id="98e9f-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="98e9f-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="98e9f-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="98e9f-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="98e9f-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="98e9f-129">See also</span></span>

- [<span data-ttu-id="98e9f-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="98e9f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

