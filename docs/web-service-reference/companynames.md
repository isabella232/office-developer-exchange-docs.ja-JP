---
title: 会社名
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 615fa52d-86ff-4630-b188-5fdb9391eee2
description: 会社名要素には、会社名の配列と、関連付けられたペルソナのソース attributions の識別子が含まれています。
ms.openlocfilehash: 25daa43873fe00837004217e3f814a7201638450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463259"
---
# <a name="companynames"></a><span data-ttu-id="3d13a-103">会社名</span><span class="sxs-lookup"><span data-stu-id="3d13a-103">CompanyNames</span></span>

<span data-ttu-id="3d13a-104">会社**名**要素には、会社名の配列と、関連付けられたペルソナのソース attributions の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3d13a-104">The **CompanyNames** element contains an array of company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CompanyNames>
    <StringAttributedValue></StringAttributedValue>
</CompanyNames>
```

 <span data-ttu-id="3d13a-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="3d13a-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d13a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3d13a-106">Attributes and elements</span></span>

<span data-ttu-id="3d13a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3d13a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d13a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d13a-108">Attributes</span></span>

<span data-ttu-id="3d13a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3d13a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d13a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3d13a-110">Child elements</span></span>

|<span data-ttu-id="3d13a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3d13a-111">**Element**</span></span>|<span data-ttu-id="3d13a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d13a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d13a-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="3d13a-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="3d13a-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d13a-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d13a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3d13a-115">Parent elements</span></span>

|<span data-ttu-id="3d13a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3d13a-116">**Element**</span></span>|<span data-ttu-id="3d13a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d13a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d13a-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3d13a-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="3d13a-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="3d13a-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3d13a-120">注釈</span><span class="sxs-lookup"><span data-stu-id="3d13a-120">Remarks</span></span>

<span data-ttu-id="3d13a-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3d13a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3d13a-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3d13a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d13a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3d13a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d13a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d13a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d13a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3d13a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3d13a-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="3d13a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="3d13a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3d13a-127">Validation File</span></span>  <br/> |<span data-ttu-id="3d13a-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3d13a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d13a-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3d13a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3d13a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="3d13a-130">See also</span></span>



- [<span data-ttu-id="3d13a-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3d13a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

