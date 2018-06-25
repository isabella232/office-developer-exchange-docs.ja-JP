---
title: ボディ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a71a75f0-0b77-4cb9-8f9d-319de72fc1fd
description: 本文要素は、BodyContentAttributedValue 要素の配列を指定します。
ms.openlocfilehash: 3316d25a567a791301c0e703a912ef28da42fa74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759522"
---
# <a name="bodies"></a><span data-ttu-id="319d1-103">ボディ</span><span class="sxs-lookup"><span data-stu-id="319d1-103">Bodies</span></span>

<span data-ttu-id="319d1-104">**本文**要素は、 **BodyContentAttributedValue**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="319d1-104">The **Bodies** element specifies an array of **BodyContentAttributedValue** elements.</span></span> 
  
```XML
<Bodies>
    <BodyContentAttributedValue></BodyContentAttributedValue>
<Bodies>
```

 <span data-ttu-id="319d1-105">**ArrayOfBodyContentAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="319d1-105">**ArrayOfBodyContentAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="319d1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="319d1-106">Attributes and elements</span></span>

<span data-ttu-id="319d1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="319d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="319d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="319d1-108">Attributes</span></span>

<span data-ttu-id="319d1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="319d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="319d1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="319d1-110">Child elements</span></span>

|<span data-ttu-id="319d1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="319d1-111">**Element**</span></span>|<span data-ttu-id="319d1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="319d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="319d1-113">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="319d1-113">BodyContentAttributedValue</span></span>](bodycontentattributedvalue.md) <br/> |<span data-ttu-id="319d1-114">アイテムの本文の内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="319d1-114">Specifies the body content of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="319d1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="319d1-115">Parent elements</span></span>

|<span data-ttu-id="319d1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="319d1-116">**Element**</span></span>|<span data-ttu-id="319d1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="319d1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="319d1-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="319d1-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="319d1-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="319d1-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="319d1-120">備考</span><span class="sxs-lookup"><span data-stu-id="319d1-120">Remarks</span></span>

<span data-ttu-id="319d1-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="319d1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="319d1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="319d1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="319d1-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="319d1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="319d1-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="319d1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="319d1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="319d1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="319d1-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="319d1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="319d1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="319d1-127">Validation File</span></span>  <br/> |<span data-ttu-id="319d1-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="319d1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="319d1-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="319d1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="319d1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="319d1-130">See also</span></span>



- [<span data-ttu-id="319d1-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="319d1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

