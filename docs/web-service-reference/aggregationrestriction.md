---
title: 集約 Ationrestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: 集約 Ationrestriction 要素は、FindPeople 要求の結果として得られる一連のペルソナプロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463525"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="9e089-103">集約 Ationrestriction</span><span class="sxs-lookup"><span data-stu-id="9e089-103">AggregationRestriction</span></span>

<span data-ttu-id="9e089-104">**集約 Ationrestriction**要素は、findpeople 要求の結果として得られる一連のペルソナプロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="9e089-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="9e089-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="9e089-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e089-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9e089-106">Attributes and elements</span></span>

<span data-ttu-id="9e089-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e089-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e089-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e089-108">Attributes</span></span>

<span data-ttu-id="9e089-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e089-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e089-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e089-110">Child elements</span></span>

[<span data-ttu-id="9e089-111">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="9e089-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="9e089-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9e089-112">Parent elements</span></span>

[<span data-ttu-id="9e089-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="9e089-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="9e089-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9e089-114">Remarks</span></span>

<span data-ttu-id="9e089-115">**集約 Ationrestriction**要素には、 **searchexpression** substitution グループを使用する子要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9e089-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="9e089-116">**Searchexpression**置換グループの一部である要素は次のとおりです[。 Contains](contains.md)、[除外](excludes.md)、 [Exists](exists.md)、 [Not](not.md)、 [and](and.md) [、](or.md) [IsEqualTo](isequalto.md)、IsNotEqualTo、 [IsGreaterThan](isgreaterthan.md)、 [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)、 [is](isnotequalto.md)、および[IsLessThan](islessthan.md) [IsLessThanOrEqualTo](islessthanorequalto.md)。</span><span class="sxs-lookup"><span data-stu-id="9e089-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="9e089-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9e089-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e089-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e089-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e089-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9e089-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e089-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e089-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e089-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e089-121">Schema name</span></span>  <br/> |<span data-ttu-id="9e089-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9e089-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e089-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e089-123">Validation file</span></span>  <br/> |<span data-ttu-id="9e089-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9e089-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e089-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9e089-125">Can be empty</span></span>  <br/> |<span data-ttu-id="9e089-126">false</span><span class="sxs-lookup"><span data-stu-id="9e089-126">false</span></span>  <br/> |
   

