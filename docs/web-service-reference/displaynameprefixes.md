---
title: DisplayNamePrefixes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04250f8d-1b83-43ae-8d2f-e052079bf2fc
description: DisplayNamePrefixes 要素は、表示名プレフィックスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 09e1e974cbe84ec8c7a4848c3367f2501269b797
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530748"
---
# <a name="displaynameprefixes"></a><span data-ttu-id="17b6e-103">DisplayNamePrefixes</span><span class="sxs-lookup"><span data-stu-id="17b6e-103">DisplayNamePrefixes</span></span>

<span data-ttu-id="17b6e-104">**Displaynameprefixes**要素は、表示名プレフィックスの配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="17b6e-104">The **DisplayNamePrefixes** element specifies an array of display name prefixes and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<DisplayNamePrefixes>
    <StringAttributedValue></StringAttributedValue>
</DisplayNamePrefixes>
```

 <span data-ttu-id="17b6e-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="17b6e-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17b6e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17b6e-106">Attributes and elements</span></span>

<span data-ttu-id="17b6e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17b6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17b6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="17b6e-108">Attributes</span></span>

<span data-ttu-id="17b6e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="17b6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17b6e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="17b6e-110">Child elements</span></span>

|<span data-ttu-id="17b6e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="17b6e-111">**Element**</span></span>|<span data-ttu-id="17b6e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="17b6e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17b6e-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="17b6e-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="17b6e-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="17b6e-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17b6e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="17b6e-115">Parent elements</span></span>

|<span data-ttu-id="17b6e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="17b6e-116">**Element**</span></span>|<span data-ttu-id="17b6e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="17b6e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17b6e-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="17b6e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="17b6e-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="17b6e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="17b6e-120">注釈</span><span class="sxs-lookup"><span data-stu-id="17b6e-120">Remarks</span></span>

<span data-ttu-id="17b6e-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="17b6e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="17b6e-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="17b6e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17b6e-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="17b6e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17b6e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="17b6e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17b6e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17b6e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="17b6e-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="17b6e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="17b6e-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17b6e-127">Validation File</span></span>  <br/> |<span data-ttu-id="17b6e-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="17b6e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="17b6e-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="17b6e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="17b6e-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="17b6e-130">See also</span></span>

- [<span data-ttu-id="17b6e-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="17b6e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

