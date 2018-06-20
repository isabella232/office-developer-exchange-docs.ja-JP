---
title: HomeFaxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: HomeFaxes 要素は、自宅の fax 番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: dd2cd8bba2c4cc7d08e88787d648e96ea996a251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831840"
---
# <a name="homefaxes"></a><span data-ttu-id="b85e9-103">HomeFaxes</span><span class="sxs-lookup"><span data-stu-id="b85e9-103">HomeFaxes</span></span>

<span data-ttu-id="b85e9-104">**HomeFaxes**要素は、自宅の fax 番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="b85e9-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="b85e9-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b85e9-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b85e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b85e9-106">Attributes and elements</span></span>

<span data-ttu-id="b85e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b85e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b85e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b85e9-108">Attributes</span></span>

<span data-ttu-id="b85e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b85e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b85e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b85e9-110">Child elements</span></span>

|<span data-ttu-id="b85e9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b85e9-111">**Element**</span></span>|<span data-ttu-id="b85e9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b85e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b85e9-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b85e9-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="b85e9-114">ペルソナの 1 つの属性付きの電話番号が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b85e9-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b85e9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b85e9-115">Parent elements</span></span>

|<span data-ttu-id="b85e9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b85e9-116">**Element**</span></span>|<span data-ttu-id="b85e9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b85e9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b85e9-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="b85e9-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b85e9-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="b85e9-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b85e9-120">備考</span><span class="sxs-lookup"><span data-stu-id="b85e9-120">Remarks</span></span>

<span data-ttu-id="b85e9-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b85e9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b85e9-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b85e9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b85e9-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="b85e9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b85e9-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="b85e9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b85e9-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b85e9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b85e9-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="b85e9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b85e9-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b85e9-127">Validation File</span></span>  <br/> |<span data-ttu-id="b85e9-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b85e9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b85e9-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b85e9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b85e9-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b85e9-130">See also</span></span>



- [<span data-ttu-id="b85e9-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b85e9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

