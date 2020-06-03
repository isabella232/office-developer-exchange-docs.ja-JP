---
title: BusinessPhoneNumbers2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f335ea74-9b5b-4224-9475-40ef33fe76bd
description: BusinessPhoneNumbers2 要素は、BusinessPhoneNumber2 要素の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: c8879e3f7ab996d7e761a72b7ce5f332a9006aed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461605"
---
# <a name="businessphonenumbers2"></a><span data-ttu-id="21809-103">BusinessPhoneNumbers2</span><span class="sxs-lookup"><span data-stu-id="21809-103">BusinessPhoneNumbers2</span></span>

<span data-ttu-id="21809-104">**BusinessPhoneNumbers2**要素は、 **BusinessPhoneNumber2**要素の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="21809-104">The **BusinessPhoneNumbers2** element specifies an array of **BusinessPhoneNumber2** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers2>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers2>
```

 <span data-ttu-id="21809-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="21809-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21809-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21809-106">Attributes and elements</span></span>

<span data-ttu-id="21809-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21809-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21809-108">属性</span><span class="sxs-lookup"><span data-stu-id="21809-108">Attributes</span></span>

<span data-ttu-id="21809-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21809-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21809-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21809-110">Child elements</span></span>

|<span data-ttu-id="21809-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="21809-111">**Element**</span></span>|<span data-ttu-id="21809-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="21809-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21809-113">Value (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="21809-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="21809-114">電話番号と種類の情報を指定し、attributions のセットに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="21809-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="21809-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="21809-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="21809-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="21809-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21809-117">親要素</span><span class="sxs-lookup"><span data-stu-id="21809-117">Parent elements</span></span>

|<span data-ttu-id="21809-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="21809-118">**Element**</span></span>|<span data-ttu-id="21809-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="21809-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21809-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="21809-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="21809-121">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="21809-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21809-122">注釈</span><span class="sxs-lookup"><span data-stu-id="21809-122">Remarks</span></span>

<span data-ttu-id="21809-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="21809-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="21809-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="21809-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21809-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21809-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21809-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="21809-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21809-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21809-127">Schema Name</span></span>  <br/> |<span data-ttu-id="21809-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="21809-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="21809-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21809-129">Validation File</span></span>  <br/> |<span data-ttu-id="21809-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="21809-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="21809-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="21809-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="21809-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="21809-132">See also</span></span>



- [<span data-ttu-id="21809-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="21809-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

