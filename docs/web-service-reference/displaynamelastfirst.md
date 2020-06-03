---
title: DisplayNameLastFirst
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d392e138-a514-4bce-81b1-1f484e353d1c
description: DisplayNameLastFirst 要素は、関連付けられたペルソナの表示名を書式、姓、名に指定します。
ms.openlocfilehash: d569a87ce77a4f1840ed4f865e671399726ede78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463161"
---
# <a name="displaynamelastfirst"></a><span data-ttu-id="6f9ab-103">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="6f9ab-103">DisplayNameLastFirst</span></span>

<span data-ttu-id="6f9ab-104">**Displaynamelastfirst**要素は、関連付けられたペルソナの表示名を "姓"、"名" という形式で指定します。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-104">The **DisplayNameLastFirst** element specifies the display name of the associated persona in the format, "Last Name", "First Name".</span></span> 
  
```XML
<DisplayNameLastFirst></DisplayNameLastFirst>
```

 <span data-ttu-id="6f9ab-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6f9ab-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f9ab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6f9ab-106">Attributes and elements</span></span>

<span data-ttu-id="6f9ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f9ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f9ab-108">Attributes</span></span>

<span data-ttu-id="6f9ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f9ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6f9ab-110">Child elements</span></span>

<span data-ttu-id="6f9ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f9ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6f9ab-112">Parent elements</span></span>

|<span data-ttu-id="6f9ab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6f9ab-113">**Element**</span></span>|<span data-ttu-id="6f9ab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f9ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f9ab-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6f9ab-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6f9ab-116">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f9ab-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6f9ab-117">Text value</span></span>

<span data-ttu-id="6f9ab-118">**Displaynamelastfirst**要素のテキスト値は、姓が先頭の表示名を指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-118">The text value of the **DisplayNameLastFirst** element is a string value that specifies the display name, with the surname first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6f9ab-119">注釈</span><span class="sxs-lookup"><span data-stu-id="6f9ab-119">Remarks</span></span>

<span data-ttu-id="6f9ab-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6f9ab-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f9ab-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6f9ab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f9ab-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f9ab-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f9ab-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f9ab-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6f9ab-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="6f9ab-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="6f9ab-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f9ab-126">Validation File</span></span>  <br/> |<span data-ttu-id="6f9ab-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6f9ab-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f9ab-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f9ab-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6f9ab-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f9ab-129">See also</span></span>

- [<span data-ttu-id="6f9ab-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6f9ab-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

