---
title: DisplayNamePrefix
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 60363698-7603-4051-a66e-007c02db17cb
description: DisplayNamePrefix 要素は、関連付けられたペルソナの表示名のプレフィックスを指定します。
ms.openlocfilehash: e7c723bb8da0834b96987f82e8f1c03c88c8d68c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458741"
---
# <a name="displaynameprefix"></a><span data-ttu-id="a8a5f-103">DisplayNamePrefix</span><span class="sxs-lookup"><span data-stu-id="a8a5f-103">DisplayNamePrefix</span></span>

<span data-ttu-id="a8a5f-104">**Displaynameprefix**要素は、関連付けられたペルソナの表示名のプレフィックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-104">The **DisplayNamePrefix** element specifies the prefix of the display name of the associated persona.</span></span> 
  
```xml
<DisplayNamePrefix></DisplayNamePrefix>
```

 <span data-ttu-id="a8a5f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="a8a5f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8a5f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8a5f-106">Attributes and elements</span></span>

<span data-ttu-id="a8a5f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8a5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8a5f-108">Attributes</span></span>

<span data-ttu-id="a8a5f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8a5f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a8a5f-110">Child elements</span></span>

<span data-ttu-id="a8a5f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8a5f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a8a5f-112">Parent elements</span></span>

|<span data-ttu-id="a8a5f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8a5f-113">**Element**</span></span>|<span data-ttu-id="a8a5f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8a5f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8a5f-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="a8a5f-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a8a5f-116">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8a5f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8a5f-117">Text value</span></span>

<span data-ttu-id="a8a5f-118">**Displaynameprefix**要素のテキスト値は、表示名のプレフィックスを指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-118">The text value of the **DisplayNamePrefix** element is a string value that specifies the prefix for the display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a8a5f-119">注釈</span><span class="sxs-lookup"><span data-stu-id="a8a5f-119">Remarks</span></span>

<span data-ttu-id="a8a5f-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8a5f-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8a5f-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8a5f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8a5f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8a5f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8a5f-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8a5f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a8a5f-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8a5f-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="a8a5f-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8a5f-126">Validation File</span></span>  <br/> |<span data-ttu-id="a8a5f-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8a5f-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8a5f-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a8a5f-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a8a5f-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8a5f-129">See also</span></span>

- [<span data-ttu-id="a8a5f-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8a5f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

