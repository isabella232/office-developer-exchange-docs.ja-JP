---
title: HomeAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: HomeAddresses 要素では、ホーム アドレスの配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: a9d4ceafcac9cf0809668871b4df932b31525ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831817"
---
# <a name="homeaddresses"></a><span data-ttu-id="4c8af-103">HomeAddresses</span><span class="sxs-lookup"><span data-stu-id="4c8af-103">HomeAddresses</span></span>

<span data-ttu-id="4c8af-104">**HomeAddresses**要素では、ホーム アドレスの配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c8af-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="4c8af-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4c8af-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c8af-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4c8af-106">Attributes and elements</span></span>

<span data-ttu-id="4c8af-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c8af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c8af-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c8af-108">Attributes</span></span>

<span data-ttu-id="4c8af-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4c8af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c8af-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4c8af-110">Child elements</span></span>

|<span data-ttu-id="4c8af-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4c8af-111">**Element**</span></span>|<span data-ttu-id="4c8af-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c8af-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c8af-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4c8af-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="4c8af-114">郵送先住所と、関連付けられている帰属の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c8af-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c8af-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4c8af-115">Parent elements</span></span>

|<span data-ttu-id="4c8af-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4c8af-116">**Element**</span></span>|<span data-ttu-id="4c8af-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c8af-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c8af-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="4c8af-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4c8af-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c8af-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4c8af-120">備考</span><span class="sxs-lookup"><span data-stu-id="4c8af-120">Remarks</span></span>

<span data-ttu-id="4c8af-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4c8af-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c8af-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4c8af-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c8af-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="4c8af-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c8af-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="4c8af-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c8af-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4c8af-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4c8af-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4c8af-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4c8af-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4c8af-127">Validation File</span></span>  <br/> |<span data-ttu-id="4c8af-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c8af-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c8af-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4c8af-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4c8af-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4c8af-130">See also</span></span>



- [<span data-ttu-id="4c8af-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4c8af-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

