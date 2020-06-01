---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: FormattedAddress 要素は、関連付けられている郵便番号の書式設定された表示値を指定します。
ms.openlocfilehash: 9150a3bb5bc81f7afecdafbf0cc33fafff597578
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461941"
---
# <a name="formattedaddress"></a><span data-ttu-id="aed70-103">FormattedAddress</span><span class="sxs-lookup"><span data-stu-id="aed70-103">FormattedAddress</span></span>

<span data-ttu-id="aed70-104">**FormattedAddress**要素は、関連付けられている郵便番号の書式設定された表示値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aed70-104">The **FormattedAddress** element specifies the formatted display value of the associated postal address.</span></span> 
  
```XML
<FormattedAddress></FormattedAddress>
```

 <span data-ttu-id="aed70-105">**string**</span><span class="sxs-lookup"><span data-stu-id="aed70-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aed70-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aed70-106">Attributes and elements</span></span>

<span data-ttu-id="aed70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aed70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aed70-108">属性</span><span class="sxs-lookup"><span data-stu-id="aed70-108">Attributes</span></span>

<span data-ttu-id="aed70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aed70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aed70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aed70-110">Child elements</span></span>

<span data-ttu-id="aed70-111">なし。</span><span class="sxs-lookup"><span data-stu-id="aed70-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aed70-112">親要素</span><span class="sxs-lookup"><span data-stu-id="aed70-112">Parent elements</span></span>

|<span data-ttu-id="aed70-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="aed70-113">**Element**</span></span>|<span data-ttu-id="aed70-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="aed70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aed70-115">Value (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="aed70-115">Value (PersonaPostalAddressType)</span></span>](value-personapostaladdresstype.md) <br/> |<span data-ttu-id="aed70-116">住所に関連付けられている情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="aed70-116">Specifies information associated with a postal address.</span></span>  <br/> |
|[<span data-ttu-id="aed70-117">"Postaladdress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="aed70-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="aed70-118">場所の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="aed70-118">Specifies the postal address of the location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aed70-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aed70-119">Text value</span></span>

<span data-ttu-id="aed70-120">**FormattedAddress**要素のテキスト値は、書式設定されたアドレスを指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="aed70-120">The text value of the **FormattedAddress** element is a string value that specifies the formatted address.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aed70-121">注釈</span><span class="sxs-lookup"><span data-stu-id="aed70-121">Remarks</span></span>

<span data-ttu-id="aed70-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aed70-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aed70-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aed70-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aed70-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aed70-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aed70-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="aed70-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aed70-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aed70-126">Schema Name</span></span>  <br/> |<span data-ttu-id="aed70-127">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="aed70-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="aed70-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aed70-128">Validation File</span></span>  <br/> |<span data-ttu-id="aed70-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="aed70-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aed70-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aed70-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aed70-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="aed70-131">See also</span></span>



- [<span data-ttu-id="aed70-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="aed70-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

