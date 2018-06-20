---
title: Altitude
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 14c2c8bd-db54-4b03-9a97-190ff9e908b3
description: 高度の要素では、住所の高度を指定します。
ms.openlocfilehash: 03517dd3ffa38e435da8f4f5f3aae23f276411bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759317"
---
# <a name="altitude"></a><span data-ttu-id="c3ecb-103">Altitude</span><span class="sxs-lookup"><span data-stu-id="c3ecb-103">Altitude</span></span>

<span data-ttu-id="c3ecb-104">**高度**の要素では、住所の高度を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-104">The **Altitude** element specifies the altitude of a postal address.</span></span> 
  
```XML
<Altitude></Altitude>
```

 <span data-ttu-id="c3ecb-105">**xs:double**</span><span class="sxs-lookup"><span data-stu-id="c3ecb-105">**xs:double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3ecb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c3ecb-106">Attributes and elements</span></span>

<span data-ttu-id="c3ecb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3ecb-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3ecb-108">Attributes</span></span>

<span data-ttu-id="c3ecb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3ecb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c3ecb-110">Child elements</span></span>

<span data-ttu-id="c3ecb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3ecb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c3ecb-112">Parent elements</span></span>

|<span data-ttu-id="c3ecb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c3ecb-113">**Element**</span></span>|<span data-ttu-id="c3ecb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c3ecb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3ecb-115">住所 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="c3ecb-115">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="c3ecb-116">場所の郵便の宛先を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-116">Specifies the postal address of the location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3ecb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c3ecb-117">Text value</span></span>

<span data-ttu-id="c3ecb-118">高度要素のテキスト値は、住所の高度です。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-118">The text value of the Altitude element is the altitude of a postal address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3ecb-119">備考</span><span class="sxs-lookup"><span data-stu-id="c3ecb-119">Remarks</span></span>

<span data-ttu-id="c3ecb-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c3ecb-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3ecb-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="c3ecb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3ecb-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="c3ecb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3ecb-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c3ecb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c3ecb-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="c3ecb-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="c3ecb-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c3ecb-126">Validation File</span></span>  <br/> |<span data-ttu-id="c3ecb-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c3ecb-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3ecb-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c3ecb-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c3ecb-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3ecb-129">See also</span></span>

- [<span data-ttu-id="c3ecb-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c3ecb-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

