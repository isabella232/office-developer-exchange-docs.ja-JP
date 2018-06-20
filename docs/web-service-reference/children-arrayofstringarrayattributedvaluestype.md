---
title: 子 (ArrayOfStringArrayAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: 子要素は、子の名前の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 7c98e7cb96cecad0d1b5122236b6cd0947c6b3d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759621"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="4d7e8-103">子 (ArrayOfStringArrayAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="4d7e8-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="4d7e8-104">**子**要素は、子の名前の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="4d7e8-105">**ArrayOfStringArrayAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4d7e8-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d7e8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4d7e8-106">Attributes and elements</span></span>

<span data-ttu-id="4d7e8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d7e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d7e8-108">Attributes</span></span>

<span data-ttu-id="4d7e8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d7e8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4d7e8-110">Child elements</span></span>

|<span data-ttu-id="4d7e8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d7e8-111">**Element**</span></span>|<span data-ttu-id="4d7e8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d7e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d7e8-113">StringArrayAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4d7e8-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="4d7e8-114">ペルソナの要素のデータを文字列の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d7e8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4d7e8-115">Parent elements</span></span>

|<span data-ttu-id="4d7e8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d7e8-116">**Element**</span></span>|<span data-ttu-id="4d7e8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d7e8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d7e8-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="4d7e8-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4d7e8-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d7e8-120">備考</span><span class="sxs-lookup"><span data-stu-id="4d7e8-120">Remarks</span></span>

<span data-ttu-id="4d7e8-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d7e8-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d7e8-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="4d7e8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d7e8-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="4d7e8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d7e8-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d7e8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4d7e8-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4d7e8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4d7e8-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d7e8-127">Validation File</span></span>  <br/> |<span data-ttu-id="4d7e8-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d7e8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d7e8-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d7e8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4d7e8-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d7e8-130">See also</span></span>



- [<span data-ttu-id="4d7e8-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4d7e8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

