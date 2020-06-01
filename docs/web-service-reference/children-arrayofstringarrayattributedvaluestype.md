---
title: 子 (ArrayOfStringArrayAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: 子要素は、関連付けられたペルソナの子の名前とソース attributions の id の配列を指定します。
ms.openlocfilehash: f4217f8a444bfdb6d86ff7b912294cfad9cbdcdc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460233"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="50180-103">子 (ArrayOfStringArrayAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="50180-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="50180-104">**子**要素は、関連付けられたペルソナの子の名前とソース attributions の id の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="50180-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="50180-105">**ArrayOfStringArrayAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="50180-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50180-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="50180-106">Attributes and elements</span></span>

<span data-ttu-id="50180-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50180-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50180-108">属性</span><span class="sxs-lookup"><span data-stu-id="50180-108">Attributes</span></span>

<span data-ttu-id="50180-109">なし。</span><span class="sxs-lookup"><span data-stu-id="50180-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50180-110">子要素</span><span class="sxs-lookup"><span data-stu-id="50180-110">Child elements</span></span>

|<span data-ttu-id="50180-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="50180-111">**Element**</span></span>|<span data-ttu-id="50180-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="50180-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50180-113">StringArrayAttributedValue</span><span class="sxs-lookup"><span data-stu-id="50180-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="50180-114">Persona 要素の文字列データの配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="50180-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50180-115">親要素</span><span class="sxs-lookup"><span data-stu-id="50180-115">Parent elements</span></span>

|<span data-ttu-id="50180-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="50180-116">**Element**</span></span>|<span data-ttu-id="50180-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="50180-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50180-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="50180-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="50180-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="50180-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50180-120">注釈</span><span class="sxs-lookup"><span data-stu-id="50180-120">Remarks</span></span>

<span data-ttu-id="50180-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="50180-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="50180-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="50180-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50180-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="50180-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50180-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="50180-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50180-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="50180-125">Schema Name</span></span>  <br/> |<span data-ttu-id="50180-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="50180-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="50180-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="50180-127">Validation File</span></span>  <br/> |<span data-ttu-id="50180-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="50180-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="50180-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="50180-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="50180-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="50180-130">See also</span></span>



- [<span data-ttu-id="50180-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="50180-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

