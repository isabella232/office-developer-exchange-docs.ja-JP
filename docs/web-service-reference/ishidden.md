---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: IsHidden 要素には、基になるメンバーを非表示またはペルソナの一部として表示するかどうかを示すブール値が含まれています。
ms.openlocfilehash: ee20bf0af287e3cddaedb5bc6d3c63ef9a7a7006
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832032"
---
# <a name="ishidden"></a><span data-ttu-id="e5f82-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="e5f82-103">IsHidden</span></span>

<span data-ttu-id="e5f82-104">**IsHidden**要素には、基になるメンバーを非表示またはペルソナの一部として表示するかどうかを示すブール値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e5f82-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="e5f82-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="e5f82-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5f82-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e5f82-106">Attributes and elements</span></span>

<span data-ttu-id="e5f82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5f82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5f82-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5f82-108">Attributes</span></span>

<span data-ttu-id="e5f82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e5f82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5f82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e5f82-110">Child elements</span></span>

<span data-ttu-id="e5f82-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e5f82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5f82-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e5f82-112">Parent elements</span></span>

|<span data-ttu-id="e5f82-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5f82-113">**Element**</span></span>|<span data-ttu-id="e5f82-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5f82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5f82-115">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="e5f82-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="e5f82-116">**ペルソナ**の要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5f82-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5f82-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e5f82-117">Text value</span></span>

<span data-ttu-id="e5f82-118">の**場合は true** 、 **IsHidden**要素のテキスト値は、基になるメンバーを非表示またはペルソナの一部として表示することを示します。</span><span class="sxs-lookup"><span data-stu-id="e5f82-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="e5f82-119">値が**false**のかを示して連絡先を基になる必要がありますいない非表示に、ペルソナの一部として表示されます。</span><span class="sxs-lookup"><span data-stu-id="e5f82-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e5f82-120">備考</span><span class="sxs-lookup"><span data-stu-id="e5f82-120">Remarks</span></span>

<span data-ttu-id="e5f82-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e5f82-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e5f82-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e5f82-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5f82-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="e5f82-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5f82-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="e5f82-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5f82-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e5f82-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e5f82-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="e5f82-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e5f82-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e5f82-127">Validation File</span></span>  <br/> |<span data-ttu-id="e5f82-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5f82-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5f82-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5f82-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e5f82-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5f82-130">See also</span></span>



- [<span data-ttu-id="e5f82-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e5f82-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

