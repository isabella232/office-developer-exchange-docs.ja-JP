---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: CarPhone 要素では、自動車電話の番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 694b3578e127a84dfd2fb844c6e81b28553b687c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759610"
---
# <a name="carphones"></a><span data-ttu-id="2c6c5-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="2c6c5-103">CarPhones</span></span>

<span data-ttu-id="2c6c5-104">**CarPhone**要素では、自動車電話の番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="2c6c5-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2c6c5-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c6c5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2c6c5-106">Attributes and elements</span></span>

<span data-ttu-id="2c6c5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c6c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c6c5-108">Attributes</span></span>

<span data-ttu-id="2c6c5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c6c5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2c6c5-110">Child elements</span></span>

|<span data-ttu-id="2c6c5-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2c6c5-111">**Element**</span></span>|<span data-ttu-id="2c6c5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c6c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c6c5-113">値 (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="2c6c5-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="2c6c5-114">帰属のセットが関連付けられているし、電話の数と種類の情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="2c6c5-115">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="2c6c5-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="2c6c5-116">帰属、関連付けられている**値**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c6c5-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2c6c5-117">Parent elements</span></span>

|<span data-ttu-id="2c6c5-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2c6c5-118">**Element**</span></span>|<span data-ttu-id="2c6c5-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c6c5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c6c5-120">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="2c6c5-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2c6c5-121">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c6c5-122">備考</span><span class="sxs-lookup"><span data-stu-id="2c6c5-122">Remarks</span></span>

<span data-ttu-id="2c6c5-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2c6c5-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c6c5-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="2c6c5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c6c5-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="2c6c5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c6c5-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c6c5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2c6c5-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2c6c5-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="2c6c5-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c6c5-129">Validation File</span></span>  <br/> |<span data-ttu-id="2c6c5-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c6c5-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c6c5-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2c6c5-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2c6c5-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c6c5-132">See also</span></span>



- [<span data-ttu-id="2c6c5-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2c6c5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

