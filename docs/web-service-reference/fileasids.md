---
title: FileAsIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 71cae100-b68e-454b-b9b6-ddbcb4d78f3f
description: FileAsIds 要素は、StringAttributedValue 要素の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 52c2c6caea81922f715b40a483f94af5ba44d5e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760482"
---
# <a name="fileasids"></a><span data-ttu-id="e42b4-103">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="e42b4-103">FileAsIds</span></span>

<span data-ttu-id="e42b4-104">**FileAsIds**要素は、 **StringAttributedValue**要素の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e42b4-104">The **FileAsIds** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAsIds>
    <StringAttributedValue/>
<FileAsIds>
```

 <span data-ttu-id="e42b4-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="e42b4-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e42b4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e42b4-106">Attributes and elements</span></span>

<span data-ttu-id="e42b4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e42b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e42b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="e42b4-108">Attributes</span></span>

<span data-ttu-id="e42b4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e42b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e42b4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e42b4-110">Child elements</span></span>

|<span data-ttu-id="e42b4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e42b4-111">**Element**</span></span>|<span data-ttu-id="e42b4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e42b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e42b4-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="e42b4-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="e42b4-114">ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e42b4-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e42b4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e42b4-115">Parent elements</span></span>

|<span data-ttu-id="e42b4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e42b4-116">**Element**</span></span>|<span data-ttu-id="e42b4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e42b4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e42b4-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="e42b4-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e42b4-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="e42b4-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e42b4-120">備考</span><span class="sxs-lookup"><span data-stu-id="e42b4-120">Remarks</span></span>

<span data-ttu-id="e42b4-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e42b4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e42b4-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e42b4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e42b4-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="e42b4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e42b4-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="e42b4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e42b4-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e42b4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e42b4-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="e42b4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e42b4-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e42b4-127">Validation File</span></span>  <br/> |<span data-ttu-id="e42b4-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e42b4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e42b4-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e42b4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e42b4-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e42b4-130">See also</span></span>



- [<span data-ttu-id="e42b4-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e42b4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

