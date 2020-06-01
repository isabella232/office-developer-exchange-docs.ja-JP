---
title: 型 (string)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5eea7a8-c40d-42a6-8e0d-67f3252496cf
description: Type 要素は、住所または電話番号の種類を指定します。たとえば、「ホーム」または「ビジネス」です。
ms.openlocfilehash: 83dd6576e8a365be61c4e6d2f3afc8a59aba92a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465717"
---
# <a name="type-string"></a><span data-ttu-id="428ba-103">型 (string)</span><span class="sxs-lookup"><span data-stu-id="428ba-103">Type (string)</span></span>

<span data-ttu-id="428ba-104">**Type**要素は、住所または電話番号の種類を指定します (例: "自宅" または "会社")。</span><span class="sxs-lookup"><span data-stu-id="428ba-104">The **Type** element specifies the type of postal address or phone number, for example, "Home" or "Business".</span></span> 
  
```XML
<Type></Type>
```

 <span data-ttu-id="428ba-105">**string**</span><span class="sxs-lookup"><span data-stu-id="428ba-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="428ba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="428ba-106">Attributes and elements</span></span>

<span data-ttu-id="428ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="428ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="428ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="428ba-108">Attributes</span></span>

<span data-ttu-id="428ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="428ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="428ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="428ba-110">Child elements</span></span>

<span data-ttu-id="428ba-111">なし。</span><span class="sxs-lookup"><span data-stu-id="428ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="428ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="428ba-112">Parent elements</span></span>

<span data-ttu-id="428ba-113">[電話](phone.md)  | [PhoneNumber](phonenumber.md)  | [Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | ["Postaladdress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="428ba-113">[Phone](phone.md) | [PhoneNumber](phonenumber.md) | [Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="428ba-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="428ba-114">Text value</span></span>

<span data-ttu-id="428ba-115">**Type**要素のテキスト値は、住所または電話番号の種類です。</span><span class="sxs-lookup"><span data-stu-id="428ba-115">The text value of the **Type** element is the type of a postal address or phone number.</span></span> <span data-ttu-id="428ba-116">たとえば、 **Type**要素には "Home" または "Business" という値が必要です。</span><span class="sxs-lookup"><span data-stu-id="428ba-116">For example, the values "Home" or "Business" are expected values for the **Type** element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="428ba-117">注釈</span><span class="sxs-lookup"><span data-stu-id="428ba-117">Remarks</span></span>

<span data-ttu-id="428ba-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="428ba-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="428ba-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="428ba-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="428ba-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="428ba-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="428ba-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="428ba-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="428ba-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="428ba-122">Schema name</span></span>  <br/> |<span data-ttu-id="428ba-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="428ba-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="428ba-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="428ba-124">Validation file</span></span>  <br/> |<span data-ttu-id="428ba-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="428ba-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="428ba-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="428ba-126">Can be empty</span></span>  <br/> ||
   

