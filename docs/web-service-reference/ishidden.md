---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: IsHidden 要素には、基になる連絡先を非表示にするか、ペルソナの一部として表示するかを示すブール値が含まれています。
ms.openlocfilehash: a22628e9ab4a46de04fe395f2d6c1b70083a5c77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464239"
---
# <a name="ishidden"></a><span data-ttu-id="23cd0-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="23cd0-103">IsHidden</span></span>

<span data-ttu-id="23cd0-104">**IsHidden**要素には、基になる連絡先を非表示にするか、ペルソナの一部として表示するかを示すブール値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="23cd0-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="23cd0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="23cd0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23cd0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="23cd0-106">Attributes and elements</span></span>

<span data-ttu-id="23cd0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23cd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23cd0-108">属性</span><span class="sxs-lookup"><span data-stu-id="23cd0-108">Attributes</span></span>

<span data-ttu-id="23cd0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="23cd0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23cd0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="23cd0-110">Child elements</span></span>

<span data-ttu-id="23cd0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="23cd0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23cd0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="23cd0-112">Parent elements</span></span>

|<span data-ttu-id="23cd0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="23cd0-113">**Element**</span></span>|<span data-ttu-id="23cd0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="23cd0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23cd0-115">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="23cd0-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="23cd0-116">**Persona**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="23cd0-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23cd0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="23cd0-117">Text value</span></span>

<span data-ttu-id="23cd0-118">**IsHidden**要素のテキスト値が**true**になっている場合は、基になる連絡先を非表示にするか、ペルソナの一部として表示する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="23cd0-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="23cd0-119">値が**false**の場合は、基になる連絡先を非表示にしたり、ペルソナの一部として表示したりしないことを示します。</span><span class="sxs-lookup"><span data-stu-id="23cd0-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="23cd0-120">注釈</span><span class="sxs-lookup"><span data-stu-id="23cd0-120">Remarks</span></span>

<span data-ttu-id="23cd0-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="23cd0-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23cd0-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="23cd0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23cd0-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="23cd0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23cd0-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="23cd0-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23cd0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23cd0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="23cd0-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="23cd0-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="23cd0-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23cd0-127">Validation File</span></span>  <br/> |<span data-ttu-id="23cd0-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="23cd0-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="23cd0-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="23cd0-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="23cd0-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="23cd0-130">See also</span></span>



- [<span data-ttu-id="23cd0-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="23cd0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

