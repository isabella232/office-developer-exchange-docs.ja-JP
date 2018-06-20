---
title: 頭文字 (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 060c0cf1-c632-484c-87f5-f577017a7090
description: '[頭文字] 要素は、[頭文字] の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。'
ms.openlocfilehash: 5b9fe4062bcc0d60de828ed6b0cb08faa45b5c19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831926"
---
# <a name="initials-arrayofstringattributedvaluestype"></a><span data-ttu-id="289a6-103">頭文字 (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="289a6-103">Initials (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="289a6-104">**[頭文字]** 要素は、[頭文字] の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="289a6-104">The **Initials** element specifies an array of initials values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Initials>
    <StringAttributedValue/>
</Initials>
```

 <span data-ttu-id="289a6-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="289a6-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="289a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="289a6-106">Attributes and elements</span></span>

<span data-ttu-id="289a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="289a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="289a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="289a6-108">Attributes</span></span>

<span data-ttu-id="289a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="289a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="289a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="289a6-110">Child elements</span></span>

|<span data-ttu-id="289a6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="289a6-111">**Element**</span></span>|<span data-ttu-id="289a6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="289a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="289a6-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="289a6-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="289a6-114">ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="289a6-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="289a6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="289a6-115">Parent elements</span></span>

|<span data-ttu-id="289a6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="289a6-116">**Element**</span></span>|<span data-ttu-id="289a6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="289a6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="289a6-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="289a6-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="289a6-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="289a6-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="289a6-120">備考</span><span class="sxs-lookup"><span data-stu-id="289a6-120">Remarks</span></span>

<span data-ttu-id="289a6-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="289a6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="289a6-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="289a6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="289a6-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="289a6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="289a6-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="289a6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="289a6-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="289a6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="289a6-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="289a6-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="289a6-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="289a6-127">Validation File</span></span>  <br/> |<span data-ttu-id="289a6-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="289a6-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="289a6-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="289a6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="289a6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="289a6-130">See also</span></span>



- [<span data-ttu-id="289a6-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="289a6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

