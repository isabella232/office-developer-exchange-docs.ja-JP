---
title: DisplayNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dedd43c8-c1d6-4671-89c5-ce7ab3979fda
description: DisplayNames 要素は、表示名の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 7d0c528b5b7f9adae271a42380550115fbcf94d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460737"
---
# <a name="displaynames"></a><span data-ttu-id="9a5b2-103">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="9a5b2-103">DisplayNames</span></span>

<span data-ttu-id="9a5b2-104">**Displaynames**要素は、表示名の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-104">The **DisplayNames** element specifies an array of display names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<DisplayNames>
    <StringAttributedValue></StringAttributedValue>
</DisplayNames>
```

 <span data-ttu-id="9a5b2-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9a5b2-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a5b2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9a5b2-106">Attributes and elements</span></span>

<span data-ttu-id="9a5b2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a5b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a5b2-108">Attributes</span></span>

<span data-ttu-id="9a5b2-109">なし</span><span class="sxs-lookup"><span data-stu-id="9a5b2-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a5b2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9a5b2-110">Child elements</span></span>

|<span data-ttu-id="9a5b2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9a5b2-111">**Element**</span></span>|<span data-ttu-id="9a5b2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a5b2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a5b2-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9a5b2-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="9a5b2-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a5b2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9a5b2-115">Parent elements</span></span>

|<span data-ttu-id="9a5b2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a5b2-116">**Element**</span></span>|<span data-ttu-id="9a5b2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a5b2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a5b2-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="9a5b2-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9a5b2-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9a5b2-120">注釈</span><span class="sxs-lookup"><span data-stu-id="9a5b2-120">Remarks</span></span>

<span data-ttu-id="9a5b2-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9a5b2-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a5b2-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9a5b2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a5b2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a5b2-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a5b2-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a5b2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9a5b2-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="9a5b2-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9a5b2-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a5b2-127">Validation File</span></span>  <br/> |<span data-ttu-id="9a5b2-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9a5b2-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a5b2-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9a5b2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a5b2-130">See also</span></span>

- [<span data-ttu-id="9a5b2-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9a5b2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

