---
title: アドレス (ArrayOfAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 711acc90-8e5b-4658-92d2-16cd441db56e
description: アドレス要素は、要素の配列を指定します。
ms.openlocfilehash: c1ee79611da1d19ce85202f9e3c0f68c421e98c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759303"
---
# <a name="addresses-arrayofaddressestype"></a><span data-ttu-id="2224a-103">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="2224a-103">Addresses (ArrayOfAddressesType)</span></span>

<span data-ttu-id="2224a-104">**アドレス**要素は、**要素**の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2224a-104">The **Addresses** element specifies an array of **Address** elements.</span></span> 
  
```XML
<Addresses>
    <Address></Address>
</Addresses>
```

 <span data-ttu-id="2224a-105">**ArrayOfAddressesType**</span><span class="sxs-lookup"><span data-stu-id="2224a-105">**ArrayOfAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2224a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2224a-106">Attributes and elements</span></span>

<span data-ttu-id="2224a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2224a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2224a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2224a-108">Attributes</span></span>

<span data-ttu-id="2224a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2224a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2224a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2224a-110">Child elements</span></span>

|<span data-ttu-id="2224a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2224a-111">**Element**</span></span>|<span data-ttu-id="2224a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2224a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2224a-113">アドレス (ContactType)</span><span class="sxs-lookup"><span data-stu-id="2224a-113">Address (ContactType)</span></span>](address-contacttype.md) <br/> |<span data-ttu-id="2224a-114">連絡先のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="2224a-114">Specifies the address of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2224a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2224a-115">Parent elements</span></span>

|<span data-ttu-id="2224a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2224a-116">**Element**</span></span>|<span data-ttu-id="2224a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2224a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2224a-118">連絡先 (ContactType)</span><span class="sxs-lookup"><span data-stu-id="2224a-118">Contact (ContactType)</span></span>](contact-contacttype.md) <br/> |<span data-ttu-id="2224a-119">統合連絡先ストアには、取引先担当者を指定します。</span><span class="sxs-lookup"><span data-stu-id="2224a-119">Specifies a contact in the Unified Contact Store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2224a-120">備考</span><span class="sxs-lookup"><span data-stu-id="2224a-120">Remarks</span></span>

<span data-ttu-id="2224a-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2224a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2224a-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2224a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2224a-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="2224a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2224a-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="2224a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2224a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2224a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2224a-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2224a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2224a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2224a-127">Validation File</span></span>  <br/> |<span data-ttu-id="2224a-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2224a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2224a-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2224a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2224a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2224a-130">See also</span></span>

- [<span data-ttu-id="2224a-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2224a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

