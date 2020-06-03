---
title: DisplayNameFirstLast
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 013c17c9-cb37-4028-9fe6-c3f47441d0f7
description: DisplayNameFirstLast 要素は、関連付けられたペルソナの表示名を書式、名、姓で指定します。
ms.openlocfilehash: 6ba35b6a17a64d46655e51691847b9aecbf52f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464113"
---
# <a name="displaynamefirstlast"></a><span data-ttu-id="6d835-103">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="6d835-103">DisplayNameFirstLast</span></span>

<span data-ttu-id="6d835-104">**Displaynamefirstlast**要素は、関連付けられたペルソナの表示名を "名"、"姓" の形式で指定します。</span><span class="sxs-lookup"><span data-stu-id="6d835-104">The **DisplayNameFirstLast** element specifies the display name of the associated persona in the format, "First Name", "Last Name".</span></span> 
  
```XML
<DisplayNameFirstLast>
```

 <span data-ttu-id="6d835-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6d835-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d835-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6d835-106">Attributes and elements</span></span>

<span data-ttu-id="6d835-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d835-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d835-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d835-108">Attributes</span></span>

<span data-ttu-id="6d835-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d835-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d835-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d835-110">Child elements</span></span>

<span data-ttu-id="6d835-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6d835-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d835-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6d835-112">Parent elements</span></span>

|<span data-ttu-id="6d835-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d835-113">**Element**</span></span>|<span data-ttu-id="6d835-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d835-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d835-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6d835-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6d835-116">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d835-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d835-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6d835-117">Text value</span></span>

<span data-ttu-id="6d835-118">**Displaynamefirstlast**要素のテキスト値は、表示名を含む文字列値で、指定された名前が先頭になります。</span><span class="sxs-lookup"><span data-stu-id="6d835-118">The text value of the **DisplayNameFirstLast** element is a string value containing the display name, with the given name first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6d835-119">注釈</span><span class="sxs-lookup"><span data-stu-id="6d835-119">Remarks</span></span>

<span data-ttu-id="6d835-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6d835-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6d835-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6d835-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d835-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6d835-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d835-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d835-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d835-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d835-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6d835-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d835-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="6d835-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d835-126">Validation File</span></span>  <br/> |<span data-ttu-id="6d835-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6d835-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d835-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6d835-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6d835-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d835-129">See also</span></span>

- [<span data-ttu-id="6d835-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6d835-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

