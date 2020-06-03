---
title: イニシャル (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 060c0cf1-c632-484c-87f5-f577017a7090
description: '[イニシャル] 要素は、イニシャル値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。'
ms.openlocfilehash: 16133192fa1d9ef066e46a181f490248a8197e5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458202"
---
# <a name="initials-arrayofstringattributedvaluestype"></a><span data-ttu-id="30d29-103">イニシャル (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="30d29-103">Initials (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="30d29-104">[**イニシャル**] 要素は、イニシャル値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="30d29-104">The **Initials** element specifies an array of initials values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Initials>
    <StringAttributedValue/>
</Initials>
```

 <span data-ttu-id="30d29-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="30d29-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30d29-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="30d29-106">Attributes and elements</span></span>

<span data-ttu-id="30d29-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="30d29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30d29-108">属性</span><span class="sxs-lookup"><span data-stu-id="30d29-108">Attributes</span></span>

<span data-ttu-id="30d29-109">なし。</span><span class="sxs-lookup"><span data-stu-id="30d29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30d29-110">子要素</span><span class="sxs-lookup"><span data-stu-id="30d29-110">Child elements</span></span>

|<span data-ttu-id="30d29-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="30d29-111">**Element**</span></span>|<span data-ttu-id="30d29-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="30d29-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30d29-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="30d29-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="30d29-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="30d29-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30d29-115">親要素</span><span class="sxs-lookup"><span data-stu-id="30d29-115">Parent elements</span></span>

|<span data-ttu-id="30d29-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="30d29-116">**Element**</span></span>|<span data-ttu-id="30d29-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="30d29-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30d29-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="30d29-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="30d29-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="30d29-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30d29-120">注釈</span><span class="sxs-lookup"><span data-stu-id="30d29-120">Remarks</span></span>

<span data-ttu-id="30d29-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="30d29-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30d29-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="30d29-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30d29-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="30d29-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30d29-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="30d29-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30d29-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="30d29-125">Schema Name</span></span>  <br/> |<span data-ttu-id="30d29-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="30d29-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="30d29-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="30d29-127">Validation File</span></span>  <br/> |<span data-ttu-id="30d29-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="30d29-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="30d29-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="30d29-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="30d29-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="30d29-130">See also</span></span>



- [<span data-ttu-id="30d29-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="30d29-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

