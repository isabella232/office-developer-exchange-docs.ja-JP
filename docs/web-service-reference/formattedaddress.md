---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: FormattedAddress 要素は、関連付けられている住所の書式設定された表示値を指定します。
ms.openlocfilehash: 14c970fcbe20567546e99e637c9c78c6003d9c0f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760581"
---
# <a name="formattedaddress"></a><span data-ttu-id="d8565-103">FormattedAddress</span><span class="sxs-lookup"><span data-stu-id="d8565-103">FormattedAddress</span></span>

<span data-ttu-id="d8565-104">**FormattedAddress**要素は、関連付けられている住所の書式設定された表示値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8565-104">The **FormattedAddress** element specifies the formatted display value of the associated postal address.</span></span> 
  
```XML
<FormattedAddress></FormattedAddress>
```

 <span data-ttu-id="d8565-105">**string**</span><span class="sxs-lookup"><span data-stu-id="d8565-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8565-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d8565-106">Attributes and elements</span></span>

<span data-ttu-id="d8565-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8565-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8565-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8565-108">Attributes</span></span>

<span data-ttu-id="d8565-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d8565-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8565-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d8565-110">Child elements</span></span>

<span data-ttu-id="d8565-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d8565-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8565-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d8565-112">Parent elements</span></span>

|<span data-ttu-id="d8565-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8565-113">**Element**</span></span>|<span data-ttu-id="d8565-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8565-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8565-115">値 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="d8565-115">Value (PersonaPostalAddressType)</span></span>](value-personapostaladdresstype.md) <br/> |<span data-ttu-id="d8565-116">郵送先住所に関連付けられている情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8565-116">Specifies information associated with a postal address.</span></span>  <br/> |
|[<span data-ttu-id="d8565-117">住所 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="d8565-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="d8565-118">場所の郵便の宛先を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8565-118">Specifies the postal address of the location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8565-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d8565-119">Text value</span></span>

<span data-ttu-id="d8565-120">**FormattedAddress**要素のテキスト値は、書式設定されたアドレスを指定する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="d8565-120">The text value of the **FormattedAddress** element is a string value that specifies the formatted address.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d8565-121">備考</span><span class="sxs-lookup"><span data-stu-id="d8565-121">Remarks</span></span>

<span data-ttu-id="d8565-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d8565-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8565-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d8565-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8565-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="d8565-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8565-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="d8565-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8565-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8565-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d8565-127">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d8565-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8565-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8565-128">Validation File</span></span>  <br/> |<span data-ttu-id="d8565-129">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8565-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8565-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d8565-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8565-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8565-131">See also</span></span>



- [<span data-ttu-id="d8565-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d8565-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

