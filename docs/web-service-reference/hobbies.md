---
title: 趣味
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f771b066-e42e-4880-bf18-709ad033d2af
description: 趣味要素は、趣味の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: c76f4fc0463928814c61b8d1fb63e4255d6be63d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460954"
---
# <a name="hobbies"></a><span data-ttu-id="76faa-103">趣味</span><span class="sxs-lookup"><span data-stu-id="76faa-103">Hobbies</span></span>

<span data-ttu-id="76faa-104">**趣味**要素は、趣味の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="76faa-104">The **Hobbies** element specifies an array of hobbies and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Hobbies>
    <StringAttributedValue/>
</Hobbies>
```

 <span data-ttu-id="76faa-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="76faa-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76faa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="76faa-106">Attributes and elements</span></span>

<span data-ttu-id="76faa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76faa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76faa-108">属性</span><span class="sxs-lookup"><span data-stu-id="76faa-108">Attributes</span></span>

<span data-ttu-id="76faa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="76faa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76faa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="76faa-110">Child elements</span></span>

|<span data-ttu-id="76faa-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="76faa-111">**Element**</span></span>|<span data-ttu-id="76faa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="76faa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76faa-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="76faa-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="76faa-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="76faa-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76faa-115">親要素</span><span class="sxs-lookup"><span data-stu-id="76faa-115">Parent elements</span></span>

|<span data-ttu-id="76faa-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="76faa-116">**Element**</span></span>|<span data-ttu-id="76faa-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="76faa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76faa-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="76faa-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="76faa-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="76faa-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76faa-120">注釈</span><span class="sxs-lookup"><span data-stu-id="76faa-120">Remarks</span></span>

<span data-ttu-id="76faa-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="76faa-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="76faa-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="76faa-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76faa-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="76faa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76faa-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="76faa-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76faa-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76faa-125">Schema Name</span></span>  <br/> |<span data-ttu-id="76faa-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="76faa-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="76faa-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76faa-127">Validation File</span></span>  <br/> |<span data-ttu-id="76faa-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="76faa-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="76faa-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="76faa-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="76faa-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="76faa-130">See also</span></span>



- [<span data-ttu-id="76faa-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="76faa-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

