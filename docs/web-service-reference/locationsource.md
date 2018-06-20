---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: LocationSource 要素は、関連付けられている住所、連絡先、電話番号帳の発生元に関する情報を指定します。
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832248"
---
# <a name="locationsource"></a><span data-ttu-id="ba0e3-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="ba0e3-103">LocationSource</span></span>

<span data-ttu-id="ba0e3-104">**LocationSource**要素は、関連付けられている住所、連絡先、電話番号帳の発生元に関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="ba0e3-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="ba0e3-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba0e3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ba0e3-106">Attributes and elements</span></span>

<span data-ttu-id="ba0e3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba0e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba0e3-108">Attributes</span></span>

<span data-ttu-id="ba0e3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba0e3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba0e3-110">Child elements</span></span>

<span data-ttu-id="ba0e3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba0e3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ba0e3-112">Parent elements</span></span>

<span data-ttu-id="ba0e3-113">[値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(PersonaPostalAddressType) の住所](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="ba0e3-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ba0e3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ba0e3-114">Text value</span></span>

<span data-ttu-id="ba0e3-115">**LocationSource**要素のテキスト値は、次の表のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="ba0e3-116">**LocationSource 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="ba0e3-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="ba0e3-117">**値**</span><span class="sxs-lookup"><span data-stu-id="ba0e3-117">**Value**</span></span>|<span data-ttu-id="ba0e3-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba0e3-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba0e3-119">なし</span><span class="sxs-lookup"><span data-stu-id="ba0e3-119">None</span></span>  <br/> |<span data-ttu-id="ba0e3-120">場所のソースがありません。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="ba0e3-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="ba0e3-121">LocationServices</span></span>  <br/> |<span data-ttu-id="ba0e3-122">情報は、サービスの場所から入手されました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="ba0e3-123">PhonebookServices</span><span class="sxs-lookup"><span data-stu-id="ba0e3-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="ba0e3-124">電話帳サービスから情報を取得しました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="ba0e3-125">デバイス</span><span class="sxs-lookup"><span data-stu-id="ba0e3-125">Device</span></span>  <br/> |<span data-ttu-id="ba0e3-126">デバイスから情報を取得しました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="ba0e3-127">連絡先</span><span class="sxs-lookup"><span data-stu-id="ba0e3-127">Contact</span></span>  <br/> |<span data-ttu-id="ba0e3-128">情報は、取引先担当者から入手されました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="ba0e3-129">リソース</span><span class="sxs-lookup"><span data-stu-id="ba0e3-129">Resource</span></span>  <br/> |<span data-ttu-id="ba0e3-130">リソースから情報を取得しました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba0e3-131">備考</span><span class="sxs-lookup"><span data-stu-id="ba0e3-131">Remarks</span></span>

<span data-ttu-id="ba0e3-132">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ba0e3-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ba0e3-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

