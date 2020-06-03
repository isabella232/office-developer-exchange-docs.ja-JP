---
title: HomePhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: ホーム電話要素は、関連付けられたペルソナの自宅の電話番号の配列とソース attributions の識別子を指定します。
ms.openlocfilehash: b55d6ca752a5b00a27eb158c6a22412a9f4ecdda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460835"
---
# <a name="homephones"></a><span data-ttu-id="6e536-103">HomePhones</span><span class="sxs-lookup"><span data-stu-id="6e536-103">HomePhones</span></span>

<span data-ttu-id="6e536-104">ホーム**電話要素は、関連**付けられたペルソナの自宅の電話番号の配列とソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e536-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="6e536-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="6e536-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e536-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6e536-106">Attributes and elements</span></span>

<span data-ttu-id="6e536-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e536-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e536-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e536-108">Attributes</span></span>

<span data-ttu-id="6e536-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6e536-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e536-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6e536-110">Child elements</span></span>

|<span data-ttu-id="6e536-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6e536-111">**Element**</span></span>|<span data-ttu-id="6e536-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e536-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e536-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6e536-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="6e536-114">ペルソナの1つの属性付き電話番号が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e536-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e536-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6e536-115">Parent elements</span></span>

|<span data-ttu-id="6e536-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e536-116">**Element**</span></span>|<span data-ttu-id="6e536-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e536-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e536-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6e536-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6e536-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="6e536-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e536-120">注釈</span><span class="sxs-lookup"><span data-stu-id="6e536-120">Remarks</span></span>

<span data-ttu-id="6e536-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6e536-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6e536-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6e536-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e536-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6e536-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e536-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e536-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e536-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e536-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6e536-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="6e536-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6e536-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e536-127">Validation File</span></span>  <br/> |<span data-ttu-id="6e536-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6e536-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e536-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6e536-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6e536-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e536-130">See also</span></span>



- [<span data-ttu-id="6e536-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6e536-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

