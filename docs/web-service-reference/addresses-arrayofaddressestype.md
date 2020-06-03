---
title: アドレス (ArrayOfAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 711acc90-8e5b-4658-92d2-16cd441db56e
description: Addresses 要素は、Address 要素の配列を指定します。
ms.openlocfilehash: 8b3a62e22cb7fc983fba78517fe4636797d06f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463623"
---
# <a name="addresses-arrayofaddressestype"></a><span data-ttu-id="1bd5c-103">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="1bd5c-103">Addresses (ArrayOfAddressesType)</span></span>

<span data-ttu-id="1bd5c-104">**Addresses**要素は、 **Address**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-104">The **Addresses** element specifies an array of **Address** elements.</span></span> 
  
```XML
<Addresses>
    <Address></Address>
</Addresses>
```

 <span data-ttu-id="1bd5c-105">**ArrayOfAddressesType**</span><span class="sxs-lookup"><span data-stu-id="1bd5c-105">**ArrayOfAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bd5c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1bd5c-106">Attributes and elements</span></span>

<span data-ttu-id="1bd5c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bd5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1bd5c-108">Attributes</span></span>

<span data-ttu-id="1bd5c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bd5c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1bd5c-110">Child elements</span></span>

|<span data-ttu-id="1bd5c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1bd5c-111">**Element**</span></span>|<span data-ttu-id="1bd5c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1bd5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bd5c-113">Address (ContactType)</span><span class="sxs-lookup"><span data-stu-id="1bd5c-113">Address (ContactType)</span></span>](address-contacttype.md) <br/> |<span data-ttu-id="1bd5c-114">連絡先のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-114">Specifies the address of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bd5c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1bd5c-115">Parent elements</span></span>

|<span data-ttu-id="1bd5c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1bd5c-116">**Element**</span></span>|<span data-ttu-id="1bd5c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1bd5c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bd5c-118">Contact (ContactType)</span><span class="sxs-lookup"><span data-stu-id="1bd5c-118">Contact (ContactType)</span></span>](contact-contacttype.md) <br/> |<span data-ttu-id="1bd5c-119">統合連絡先ストアの連絡先を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-119">Specifies a contact in the Unified Contact Store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1bd5c-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1bd5c-120">Remarks</span></span>

<span data-ttu-id="1bd5c-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1bd5c-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bd5c-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1bd5c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bd5c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1bd5c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1bd5c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1bd5c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1bd5c-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1bd5c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1bd5c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1bd5c-127">Validation File</span></span>  <br/> |<span data-ttu-id="1bd5c-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1bd5c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1bd5c-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1bd5c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1bd5c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1bd5c-130">See also</span></span>

- [<span data-ttu-id="1bd5c-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1bd5c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

