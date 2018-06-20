---
title: HomePhones2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba9bb159-362d-48e0-889d-823cb46ecebf
description: HomePhones2 要素は、HomePhone2 の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 205f2f71421a0dfc7d0057412529bcefdb6636d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831842"
---
# <a name="homephones2"></a><span data-ttu-id="6cca2-103">HomePhones2</span><span class="sxs-lookup"><span data-stu-id="6cca2-103">HomePhones2</span></span>

<span data-ttu-id="6cca2-104">**HomePhones2**要素は、 **HomePhone2**の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cca2-104">The **HomePhones2** element specifies an array of **HomePhone2** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones2>
    <PhoneNumberAttributedValue/>
</HomePhones2>
```

 <span data-ttu-id="6cca2-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="6cca2-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cca2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6cca2-106">Attributes and elements</span></span>

<span data-ttu-id="6cca2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cca2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cca2-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cca2-108">Attributes</span></span>

<span data-ttu-id="6cca2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6cca2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cca2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6cca2-110">Child elements</span></span>

|<span data-ttu-id="6cca2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cca2-111">**Element**</span></span>|<span data-ttu-id="6cca2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cca2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cca2-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6cca2-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="6cca2-114">ペルソナの 1 つの属性付きの電話番号が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cca2-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cca2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6cca2-115">Parent elements</span></span>

|<span data-ttu-id="6cca2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cca2-116">**Element**</span></span>|<span data-ttu-id="6cca2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cca2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cca2-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="6cca2-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6cca2-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cca2-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6cca2-120">備考</span><span class="sxs-lookup"><span data-stu-id="6cca2-120">Remarks</span></span>

<span data-ttu-id="6cca2-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6cca2-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6cca2-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6cca2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cca2-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="6cca2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cca2-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="6cca2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6cca2-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cca2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6cca2-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="6cca2-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6cca2-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cca2-127">Validation File</span></span>  <br/> |<span data-ttu-id="6cca2-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="6cca2-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6cca2-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6cca2-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6cca2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cca2-130">See also</span></span>



- [<span data-ttu-id="6cca2-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cca2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

