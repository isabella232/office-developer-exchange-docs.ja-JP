---
title: BusinessHomePages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9961c0c2-7cac-4af1-84ac-0eafdce0a6ab
description: BusinessHomePages 要素は、ビジネスホームページの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: f0e85e0b3c857e44d94bd42c6d3ea757d015eb25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465913"
---
# <a name="businesshomepages"></a><span data-ttu-id="d8efb-103">BusinessHomePages</span><span class="sxs-lookup"><span data-stu-id="d8efb-103">BusinessHomePages</span></span>

<span data-ttu-id="d8efb-104">**BusinessHomePages**要素は、ビジネスホームページの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8efb-104">The **BusinessHomePages** element specifies an array of business home pages and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessHomePages>
    <StringAttributedValue></StringAttributedValue>
</BusinessHomePages>
```

 <span data-ttu-id="d8efb-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="d8efb-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8efb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d8efb-106">Attributes and elements</span></span>

<span data-ttu-id="d8efb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8efb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8efb-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8efb-108">Attributes</span></span>

<span data-ttu-id="d8efb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d8efb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8efb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d8efb-110">Child elements</span></span>

|<span data-ttu-id="d8efb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d8efb-111">**Element**</span></span>|<span data-ttu-id="d8efb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8efb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8efb-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d8efb-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="d8efb-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8efb-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8efb-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d8efb-115">Parent elements</span></span>

|<span data-ttu-id="d8efb-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8efb-116">**Element**</span></span>|<span data-ttu-id="d8efb-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8efb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8efb-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="d8efb-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d8efb-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8efb-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8efb-120">注釈</span><span class="sxs-lookup"><span data-stu-id="d8efb-120">Remarks</span></span>

<span data-ttu-id="d8efb-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d8efb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8efb-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d8efb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8efb-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d8efb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8efb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8efb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8efb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8efb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d8efb-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="d8efb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8efb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8efb-127">Validation File</span></span>  <br/> |<span data-ttu-id="d8efb-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d8efb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8efb-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d8efb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8efb-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8efb-130">See also</span></span>



- [<span data-ttu-id="d8efb-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d8efb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

