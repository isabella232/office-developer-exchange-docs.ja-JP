---
title: ホーム Fax
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: '[ホーム fax] 要素は、自宅の fax 番号の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。'
ms.openlocfilehash: d49eb9e12547e4011e4ba403cb898c0fe6e9bf02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460849"
---
# <a name="homefaxes"></a><span data-ttu-id="2e44d-103">ホーム Fax</span><span class="sxs-lookup"><span data-stu-id="2e44d-103">HomeFaxes</span></span>

<span data-ttu-id="2e44d-104">[**ホーム fax]** 要素は、自宅の fax 番号の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e44d-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="2e44d-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2e44d-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e44d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2e44d-106">Attributes and elements</span></span>

<span data-ttu-id="2e44d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e44d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e44d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e44d-108">Attributes</span></span>

<span data-ttu-id="2e44d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2e44d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e44d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2e44d-110">Child elements</span></span>

|<span data-ttu-id="2e44d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2e44d-111">**Element**</span></span>|<span data-ttu-id="2e44d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e44d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e44d-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2e44d-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="2e44d-114">ペルソナの1つの属性付き電話番号が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e44d-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e44d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2e44d-115">Parent elements</span></span>

|<span data-ttu-id="2e44d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2e44d-116">**Element**</span></span>|<span data-ttu-id="2e44d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e44d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e44d-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="2e44d-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2e44d-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="2e44d-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e44d-120">注釈</span><span class="sxs-lookup"><span data-stu-id="2e44d-120">Remarks</span></span>

<span data-ttu-id="2e44d-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2e44d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e44d-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2e44d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e44d-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2e44d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e44d-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e44d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e44d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2e44d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2e44d-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="2e44d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2e44d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2e44d-127">Validation File</span></span>  <br/> |<span data-ttu-id="2e44d-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2e44d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e44d-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2e44d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2e44d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2e44d-130">See also</span></span>



- [<span data-ttu-id="2e44d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2e44d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

