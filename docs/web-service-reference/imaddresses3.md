---
title: ImAddresses3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cab51a28-dfad-4c70-aafe-e239321b784e
description: ImAddresses3 要素では、インスタント メッセージのアドレスの配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 1d6ebf9d8e831f36ea7d947a72c60c58fa5b1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831874"
---
# <a name="imaddresses3"></a><span data-ttu-id="e5042-103">ImAddresses3</span><span class="sxs-lookup"><span data-stu-id="e5042-103">ImAddresses3</span></span>

<span data-ttu-id="e5042-104">**ImAddresses3**要素では、インスタント メッセージのアドレスの配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5042-104">The **ImAddresses3** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses3>
    <StringAttributedValue/>
</ImAddresses3>
```

 <span data-ttu-id="e5042-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="e5042-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5042-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e5042-106">Attributes and elements</span></span>

<span data-ttu-id="e5042-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5042-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5042-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5042-108">Attributes</span></span>

<span data-ttu-id="e5042-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e5042-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5042-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e5042-110">Child elements</span></span>

|<span data-ttu-id="e5042-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5042-111">**Element**</span></span>|<span data-ttu-id="e5042-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5042-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5042-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="e5042-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="e5042-114">ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5042-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5042-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e5042-115">Parent elements</span></span>

|<span data-ttu-id="e5042-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5042-116">**Element**</span></span>|<span data-ttu-id="e5042-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5042-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5042-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="e5042-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e5042-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5042-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e5042-120">備考</span><span class="sxs-lookup"><span data-stu-id="e5042-120">Remarks</span></span>

<span data-ttu-id="e5042-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e5042-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e5042-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e5042-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5042-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="e5042-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5042-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="e5042-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5042-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e5042-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e5042-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="e5042-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e5042-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e5042-127">Validation File</span></span>  <br/> |<span data-ttu-id="e5042-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5042-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5042-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5042-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e5042-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5042-130">See also</span></span>



- [<span data-ttu-id="e5042-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e5042-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

