---
title: FileAses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81efc37-bb70-4d52-a614-cec87d1b0f04
description: FileAses 要素は、StringAttributedValue 要素の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: e660c74135dca9a2eb58b3486e0d2e19f85e012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19760474"
---
# <a name="fileases"></a><span data-ttu-id="f1589-103">FileAses</span><span class="sxs-lookup"><span data-stu-id="f1589-103">FileAses</span></span>

<span data-ttu-id="f1589-104">**FileAses**要素は、 **StringAttributedValue**要素の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1589-104">The **FileAses** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAses>
    <StringAttributedValue/>
</FileAses>
```

 <span data-ttu-id="f1589-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="f1589-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1589-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f1589-106">Attributes and elements</span></span>

<span data-ttu-id="f1589-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f1589-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1589-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1589-108">Attributes</span></span>

<span data-ttu-id="f1589-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f1589-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1589-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f1589-110">Child elements</span></span>

|<span data-ttu-id="f1589-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f1589-111">**Element**</span></span>|<span data-ttu-id="f1589-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1589-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1589-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f1589-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="f1589-114">ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1589-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1589-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f1589-115">Parent elements</span></span>

|<span data-ttu-id="f1589-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f1589-116">**Element**</span></span>|<span data-ttu-id="f1589-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1589-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1589-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="f1589-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f1589-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1589-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1589-120">備考</span><span class="sxs-lookup"><span data-stu-id="f1589-120">Remarks</span></span>

<span data-ttu-id="f1589-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f1589-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f1589-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f1589-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1589-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="f1589-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1589-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="f1589-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1589-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f1589-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f1589-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="f1589-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f1589-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f1589-127">Validation File</span></span>  <br/> |<span data-ttu-id="f1589-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1589-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1589-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f1589-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f1589-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f1589-130">See also</span></span>



- [<span data-ttu-id="f1589-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f1589-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

