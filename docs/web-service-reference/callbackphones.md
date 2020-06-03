---
title: 電話機
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: Attributions は、呼び出し元の電話番号の配列と、関連付けられたペルソナのソースの識別子を指定します。
ms.openlocfilehash: 79d74beffb8de8981e042b0c80e1aa5505a1048c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529463"
---
# <a name="callbackphones"></a><span data-ttu-id="64565-103">電話機</span><span class="sxs-lookup"><span data-stu-id="64565-103">CallbackPhones</span></span>

<span data-ttu-id="64565-104">Attributions**は、呼び出し**元の電話番号の配列と、関連付けられたペルソナのソースの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="64565-104">The **CallbackPhones** element specifies an array of call-back phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 <span data-ttu-id="64565-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="64565-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64565-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64565-106">Attributes and elements</span></span>

<span data-ttu-id="64565-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64565-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64565-108">属性</span><span class="sxs-lookup"><span data-stu-id="64565-108">Attributes</span></span>

<span data-ttu-id="64565-109">なし。</span><span class="sxs-lookup"><span data-stu-id="64565-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64565-110">子要素</span><span class="sxs-lookup"><span data-stu-id="64565-110">Child elements</span></span>

|<span data-ttu-id="64565-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="64565-111">**Element**</span></span>|<span data-ttu-id="64565-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="64565-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64565-113">Value (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="64565-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="64565-114">電話番号と種類の情報を指定し、attributions のセットに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="64565-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="64565-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="64565-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="64565-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="64565-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64565-117">親要素</span><span class="sxs-lookup"><span data-stu-id="64565-117">Parent elements</span></span>

|<span data-ttu-id="64565-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="64565-118">**Element**</span></span>|<span data-ttu-id="64565-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="64565-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64565-120">ユーザー</span><span class="sxs-lookup"><span data-stu-id="64565-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="64565-121">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="64565-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64565-122">注釈</span><span class="sxs-lookup"><span data-stu-id="64565-122">Remarks</span></span>

<span data-ttu-id="64565-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="64565-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64565-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="64565-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64565-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="64565-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64565-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="64565-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64565-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64565-127">Schema Name</span></span>  <br/> |<span data-ttu-id="64565-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="64565-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="64565-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64565-129">Validation File</span></span>  <br/> |<span data-ttu-id="64565-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="64565-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="64565-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="64565-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="64565-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="64565-132">See also</span></span>



- [<span data-ttu-id="64565-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="64565-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

