---
title: 型 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5eea7a8-c40d-42a6-8e0d-67f3252496cf
description: 型の要素では、郵便住所、電話番号、たとえば、HomeorBusiness の種類を指定します。
ms.openlocfilehash: b2262a01b03922e36daa3b13436f1e070918b72c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839760"
---
# <a name="type-string"></a><span data-ttu-id="91190-103">型 (文字列)</span><span class="sxs-lookup"><span data-stu-id="91190-103">Type (string)</span></span>

<span data-ttu-id="91190-104">**型**の要素では、郵便番号と住所や電話番号、たとえば、「自宅」または「ビジネス」の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="91190-104">The **Type** element specifies the type of postal address or phone number, for example, "Home" or "Business".</span></span> 
  
```XML
<Type></Type>
```

 <span data-ttu-id="91190-105">**string**</span><span class="sxs-lookup"><span data-stu-id="91190-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91190-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="91190-106">Attributes and elements</span></span>

<span data-ttu-id="91190-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91190-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91190-108">属性</span><span class="sxs-lookup"><span data-stu-id="91190-108">Attributes</span></span>

<span data-ttu-id="91190-109">なし。</span><span class="sxs-lookup"><span data-stu-id="91190-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91190-110">子要素</span><span class="sxs-lookup"><span data-stu-id="91190-110">Child elements</span></span>

<span data-ttu-id="91190-111">なし。</span><span class="sxs-lookup"><span data-stu-id="91190-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91190-112">親要素</span><span class="sxs-lookup"><span data-stu-id="91190-112">Parent elements</span></span>

<span data-ttu-id="91190-113">[電話](phone.md) | [電話番号](phonenumber.md) | [値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(PersonaPostalAddressType) の住所](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="91190-113">[Phone](phone.md) | [PhoneNumber](phonenumber.md) | [Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="91190-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="91190-114">Text value</span></span>

<span data-ttu-id="91190-115">**型**の要素のテキスト値は、郵便番号と住所や電話番号の種類です。</span><span class="sxs-lookup"><span data-stu-id="91190-115">The text value of the **Type** element is the type of a postal address or phone number.</span></span> <span data-ttu-id="91190-116">たとえば、「自宅」または「ビジネス」の値は、**型**の要素の予期される値です。</span><span class="sxs-lookup"><span data-stu-id="91190-116">For example, the values "Home" or "Business" are expected values for the **Type** element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91190-117">備考</span><span class="sxs-lookup"><span data-stu-id="91190-117">Remarks</span></span>

<span data-ttu-id="91190-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="91190-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91190-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="91190-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91190-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="91190-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91190-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="91190-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91190-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91190-122">Schema name</span></span>  <br/> |<span data-ttu-id="91190-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="91190-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="91190-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91190-124">Validation file</span></span>  <br/> |<span data-ttu-id="91190-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91190-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91190-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="91190-126">Can be empty</span></span>  <br/> ||
   

