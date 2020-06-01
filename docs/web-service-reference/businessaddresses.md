---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: BusinessAddresses 要素は、ビジネスアドレスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: d314d0de679f8eabc51dc9ee3b2e9a57cd0b8da1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465927"
---
# <a name="businessaddresses"></a><span data-ttu-id="66631-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="66631-103">BusinessAddresses</span></span>

<span data-ttu-id="66631-104">**Businessaddresses**要素は、ビジネスアドレスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="66631-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="66631-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="66631-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66631-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="66631-106">Attributes and elements</span></span>

<span data-ttu-id="66631-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66631-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66631-108">属性</span><span class="sxs-lookup"><span data-stu-id="66631-108">Attributes</span></span>

<span data-ttu-id="66631-109">なし。</span><span class="sxs-lookup"><span data-stu-id="66631-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66631-110">子要素</span><span class="sxs-lookup"><span data-stu-id="66631-110">Child elements</span></span>

|<span data-ttu-id="66631-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="66631-111">**Element**</span></span>|<span data-ttu-id="66631-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="66631-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66631-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="66631-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="66631-114">郵送先住所の配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="66631-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66631-115">親要素</span><span class="sxs-lookup"><span data-stu-id="66631-115">Parent elements</span></span>

|<span data-ttu-id="66631-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="66631-116">**Element**</span></span>|<span data-ttu-id="66631-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="66631-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66631-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="66631-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="66631-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="66631-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66631-120">注釈</span><span class="sxs-lookup"><span data-stu-id="66631-120">Remarks</span></span>

<span data-ttu-id="66631-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="66631-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66631-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="66631-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66631-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="66631-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66631-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="66631-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66631-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66631-125">Schema Name</span></span>  <br/> |<span data-ttu-id="66631-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="66631-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="66631-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66631-127">Validation File</span></span>  <br/> |<span data-ttu-id="66631-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="66631-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="66631-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="66631-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="66631-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="66631-130">See also</span></span>



- [<span data-ttu-id="66631-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="66631-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

