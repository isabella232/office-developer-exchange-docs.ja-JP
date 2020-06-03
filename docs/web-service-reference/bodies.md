---
title: 本文
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a71a75f0-0b77-4cb9-8f9d-319de72fc1fd
description: ボディ要素は、BodyContentAttributedValue 要素の配列を指定します。
ms.openlocfilehash: d7087cf213d3c659a55458e021f4b8f0400efb1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461514"
---
# <a name="bodies"></a><span data-ttu-id="8e905-103">本文</span><span class="sxs-lookup"><span data-stu-id="8e905-103">Bodies</span></span>

<span data-ttu-id="8e905-104">**ボディ**要素は、 **BodyContentAttributedValue**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e905-104">The **Bodies** element specifies an array of **BodyContentAttributedValue** elements.</span></span> 
  
```XML
<Bodies>
    <BodyContentAttributedValue></BodyContentAttributedValue>
<Bodies>
```

 <span data-ttu-id="8e905-105">**ArrayOfBodyContentAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="8e905-105">**ArrayOfBodyContentAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e905-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e905-106">Attributes and elements</span></span>

<span data-ttu-id="8e905-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e905-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e905-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e905-108">Attributes</span></span>

<span data-ttu-id="8e905-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8e905-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e905-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8e905-110">Child elements</span></span>

|<span data-ttu-id="8e905-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8e905-111">**Element**</span></span>|<span data-ttu-id="8e905-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e905-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e905-113">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8e905-113">BodyContentAttributedValue</span></span>](bodycontentattributedvalue.md) <br/> |<span data-ttu-id="8e905-114">アイテムの本文のコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e905-114">Specifies the body content of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e905-115">親要素</span><span class="sxs-lookup"><span data-stu-id="8e905-115">Parent elements</span></span>

|<span data-ttu-id="8e905-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e905-116">**Element**</span></span>|<span data-ttu-id="8e905-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e905-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e905-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="8e905-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8e905-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e905-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e905-120">注釈</span><span class="sxs-lookup"><span data-stu-id="8e905-120">Remarks</span></span>

<span data-ttu-id="8e905-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e905-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e905-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e905-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e905-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e905-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e905-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e905-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e905-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e905-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8e905-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="8e905-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8e905-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e905-127">Validation File</span></span>  <br/> |<span data-ttu-id="8e905-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8e905-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e905-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e905-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8e905-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e905-130">See also</span></span>



- [<span data-ttu-id="8e905-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e905-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

