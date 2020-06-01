---
title: ImAddresses (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: ImAddresses 要素は、インスタントメッセージアドレスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 6714af5d88e50047f48da2f10dbb33d2e2feb724
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460443"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="f851e-103">ImAddresses (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="f851e-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="f851e-104">**Imaddresses**要素は、インスタントメッセージアドレスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f851e-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="f851e-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="f851e-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f851e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f851e-106">Attributes and elements</span></span>

<span data-ttu-id="f851e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f851e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f851e-108">属性</span><span class="sxs-lookup"><span data-stu-id="f851e-108">Attributes</span></span>

<span data-ttu-id="f851e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f851e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f851e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f851e-110">Child elements</span></span>

|<span data-ttu-id="f851e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f851e-111">**Element**</span></span>|<span data-ttu-id="f851e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f851e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f851e-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f851e-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="f851e-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="f851e-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f851e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f851e-115">Parent elements</span></span>

|<span data-ttu-id="f851e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f851e-116">**Element**</span></span>|<span data-ttu-id="f851e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f851e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f851e-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="f851e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f851e-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="f851e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f851e-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f851e-120">Remarks</span></span>

<span data-ttu-id="f851e-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f851e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f851e-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f851e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f851e-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f851e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f851e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f851e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f851e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f851e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f851e-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="f851e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f851e-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f851e-127">Validation File</span></span>  <br/> |<span data-ttu-id="f851e-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f851e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f851e-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f851e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f851e-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f851e-130">See also</span></span>



- [<span data-ttu-id="f851e-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f851e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

