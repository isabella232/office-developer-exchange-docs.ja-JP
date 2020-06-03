---
title: カーフォン
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: CarPhone 要素は、車両電話番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 41d0cc264da69ab17b8ebf109759139c4249719e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462228"
---
# <a name="carphones"></a><span data-ttu-id="8e26b-103">カーフォン</span><span class="sxs-lookup"><span data-stu-id="8e26b-103">CarPhones</span></span>

<span data-ttu-id="8e26b-104">**Carphone**要素は、車両電話番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e26b-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="8e26b-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="8e26b-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e26b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e26b-106">Attributes and elements</span></span>

<span data-ttu-id="8e26b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e26b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e26b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e26b-108">Attributes</span></span>

<span data-ttu-id="8e26b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8e26b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e26b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8e26b-110">Child elements</span></span>

|<span data-ttu-id="8e26b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8e26b-111">**Element**</span></span>|<span data-ttu-id="8e26b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e26b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e26b-113">Value (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="8e26b-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="8e26b-114">電話番号と種類の情報を指定し、attributions のセットに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="8e26b-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="8e26b-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="8e26b-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="8e26b-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e26b-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e26b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="8e26b-117">Parent elements</span></span>

|<span data-ttu-id="8e26b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e26b-118">**Element**</span></span>|<span data-ttu-id="8e26b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e26b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e26b-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="8e26b-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8e26b-121">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e26b-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e26b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="8e26b-122">Remarks</span></span>

<span data-ttu-id="8e26b-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e26b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e26b-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e26b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e26b-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e26b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e26b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e26b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e26b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e26b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8e26b-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="8e26b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="8e26b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e26b-129">Validation File</span></span>  <br/> |<span data-ttu-id="8e26b-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8e26b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e26b-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e26b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8e26b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e26b-132">See also</span></span>



- [<span data-ttu-id="8e26b-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e26b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

