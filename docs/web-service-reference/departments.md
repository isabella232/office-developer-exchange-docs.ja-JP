---
title: 所属
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0a6b0a4-f0dd-4945-af69-628da93f5452
description: Department 要素は、部署名の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 17590793e00a914cb53b479994bcc89e37bb0e31
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467936"
---
# <a name="departments"></a><span data-ttu-id="cc7e9-103">所属</span><span class="sxs-lookup"><span data-stu-id="cc7e9-103">Departments</span></span>

<span data-ttu-id="cc7e9-104">Department**要素は、部署**名の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-104">The **Departments** element specifies an array of department names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Departments>
    <StringAttributedValue></StringAttributedValue>
</Departments>
```

 <span data-ttu-id="cc7e9-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="cc7e9-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc7e9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc7e9-106">Attributes and elements</span></span>

<span data-ttu-id="cc7e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc7e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc7e9-108">Attributes</span></span>

<span data-ttu-id="cc7e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc7e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc7e9-110">Child elements</span></span>

|<span data-ttu-id="cc7e9-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="cc7e9-111">**Element**</span></span>|<span data-ttu-id="cc7e9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc7e9-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="cc7e9-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="cc7e9-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc7e9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="cc7e9-115">Parent elements</span></span>

|<span data-ttu-id="cc7e9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc7e9-116">**Element**</span></span>|<span data-ttu-id="cc7e9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7e9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc7e9-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="cc7e9-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="cc7e9-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc7e9-120">注釈</span><span class="sxs-lookup"><span data-stu-id="cc7e9-120">Remarks</span></span>

<span data-ttu-id="cc7e9-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc7e9-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc7e9-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cc7e9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc7e9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc7e9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc7e9-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc7e9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cc7e9-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="cc7e9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="cc7e9-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc7e9-127">Validation File</span></span>  <br/> |<span data-ttu-id="cc7e9-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cc7e9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc7e9-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cc7e9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cc7e9-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc7e9-130">See also</span></span>

- [<span data-ttu-id="cc7e9-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc7e9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

