---
title: Address (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c39f37bf-5cf5-47a7-8a2a-337b5e68f94f
description: Address 要素は、連絡先のアドレスを指定します。
ms.openlocfilehash: ffb13c8fed28dc1baee5002dc11f7acd7d4c3db5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464911"
---
# <a name="address-contacttype"></a><span data-ttu-id="b9bab-103">Address (ContactType)</span><span class="sxs-lookup"><span data-stu-id="b9bab-103">Address (ContactType)</span></span>

<span data-ttu-id="b9bab-104">**Address**要素は、連絡先のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b9bab-104">The **Address** element specifies the address of a contact.</span></span> 
  
```XML
<Address></Address>
```

 <span data-ttu-id="b9bab-105">**xs: 文字列**</span><span class="sxs-lookup"><span data-stu-id="b9bab-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9bab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b9bab-106">Attributes and elements</span></span>

<span data-ttu-id="b9bab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9bab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9bab-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9bab-108">Attributes</span></span>

<span data-ttu-id="b9bab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b9bab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9bab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b9bab-110">Child elements</span></span>

<span data-ttu-id="b9bab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b9bab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9bab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b9bab-112">Parent elements</span></span>

|<span data-ttu-id="b9bab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9bab-113">**Element**</span></span>|<span data-ttu-id="b9bab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9bab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9bab-115">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="b9bab-115">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="b9bab-116">**Address**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9bab-116">Specifies an array of **Address** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9bab-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9bab-117">Text value</span></span>

<span data-ttu-id="b9bab-118">**Address**要素のテキスト値は、連絡先の住所です。</span><span class="sxs-lookup"><span data-stu-id="b9bab-118">The text value of the **Address** element is the contact's postal address.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b9bab-119">注釈</span><span class="sxs-lookup"><span data-stu-id="b9bab-119">Remarks</span></span>

<span data-ttu-id="b9bab-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b9bab-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b9bab-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b9bab-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9bab-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b9bab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9bab-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9bab-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9bab-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9bab-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b9bab-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9bab-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="b9bab-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9bab-126">Validation File</span></span>  <br/> |<span data-ttu-id="b9bab-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b9bab-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9bab-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9bab-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b9bab-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9bab-129">See also</span></span>

- [<span data-ttu-id="b9bab-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b9bab-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

