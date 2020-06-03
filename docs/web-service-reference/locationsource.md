---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: LocationSource 要素は、関連付けられた郵便番号の発信元に関する情報を指定します。たとえば、連絡先または電話帳などです。
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467103"
---
# <a name="locationsource"></a><span data-ttu-id="cc7b0-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="cc7b0-103">LocationSource</span></span>

<span data-ttu-id="cc7b0-104">**Locationsource**要素は、関連付けられた郵便番号の発信元に関する情報を指定します。たとえば、連絡先または電話帳などです。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="cc7b0-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="cc7b0-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc7b0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc7b0-106">Attributes and elements</span></span>

<span data-ttu-id="cc7b0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc7b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc7b0-108">Attributes</span></span>

<span data-ttu-id="cc7b0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc7b0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc7b0-110">Child elements</span></span>

<span data-ttu-id="cc7b0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc7b0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cc7b0-112">Parent elements</span></span>

<span data-ttu-id="cc7b0-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | ["Postaladdress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="cc7b0-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cc7b0-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cc7b0-114">Text value</span></span>

<span data-ttu-id="cc7b0-115">次の表に、 **Locationsource**要素のテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="cc7b0-116">**LocationSource 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="cc7b0-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="cc7b0-117">**値**</span><span class="sxs-lookup"><span data-stu-id="cc7b0-117">**Value**</span></span>|<span data-ttu-id="cc7b0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7b0-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cc7b0-119">なし</span><span class="sxs-lookup"><span data-stu-id="cc7b0-119">None</span></span>  <br/> |<span data-ttu-id="cc7b0-120">場所のソースはありません。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="cc7b0-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="cc7b0-121">LocationServices</span></span>  <br/> |<span data-ttu-id="cc7b0-122">情報は場所サービスから取得されました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="cc7b0-123">電話帳サービス</span><span class="sxs-lookup"><span data-stu-id="cc7b0-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="cc7b0-124">情報は、電話帳サービスから取得されました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="cc7b0-125">Device</span><span class="sxs-lookup"><span data-stu-id="cc7b0-125">Device</span></span>  <br/> |<span data-ttu-id="cc7b0-126">情報はデバイスから取得されました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="cc7b0-127">Contact</span><span class="sxs-lookup"><span data-stu-id="cc7b0-127">Contact</span></span>  <br/> |<span data-ttu-id="cc7b0-128">連絡先から情報を取得しました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="cc7b0-129">関連情報</span><span class="sxs-lookup"><span data-stu-id="cc7b0-129">Resource</span></span>  <br/> |<span data-ttu-id="cc7b0-130">情報はリソースから取得されました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc7b0-131">注釈</span><span class="sxs-lookup"><span data-stu-id="cc7b0-131">Remarks</span></span>

<span data-ttu-id="cc7b0-132">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc7b0-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc7b0-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

