---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: AggregationRestriction 要素は、FindPeople の要求に起因するペルソナ プロパティのセットに適用され、指定した制限に従って結果をフィルター処理する値を指定します。
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759309"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="7a9e9-103">AggregationRestriction</span><span class="sxs-lookup"><span data-stu-id="7a9e9-103">AggregationRestriction</span></span>

<span data-ttu-id="7a9e9-104">**AggregationRestriction**要素は、FindPeople の要求に起因するペルソナ プロパティのセットに適用され、指定した制限に従って結果をフィルター処理する値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="7a9e9-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="7a9e9-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a9e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7a9e9-106">Attributes and elements</span></span>

<span data-ttu-id="7a9e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a9e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a9e9-108">Attributes</span></span>

<span data-ttu-id="7a9e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a9e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7a9e9-110">Child elements</span></span>

[<span data-ttu-id="7a9e9-111">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="7a9e9-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="7a9e9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7a9e9-112">Parent elements</span></span>

[<span data-ttu-id="7a9e9-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="7a9e9-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="7a9e9-114">備考</span><span class="sxs-lookup"><span data-stu-id="7a9e9-114">Remarks</span></span>

<span data-ttu-id="7a9e9-115">**AggregationRestriction**要素は、 **SearchExpression**の代替グループを使用する任意の子要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="7a9e9-116">**SearchExpression**代替グループの一部になっている要素:[含む](contains.md)、[除外](excludes.md)、 [Exists](exists.md)、[しない](not.md)、[または](or.md)、[および](and.md)、 [IsEqualTo](isequalto.md)、 [IsNotEqualTo](isnotequalto.md)、 [IsGreaterThan](isgreaterthan.md)、 [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)、 [IsLessThan](islessthan.md)、および[IsLessThanOrEqualTo](islessthanorequalto.md)。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="7a9e9-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a9e9-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a9e9-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="7a9e9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a9e9-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="7a9e9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a9e9-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a9e9-121">Schema name</span></span>  <br/> |<span data-ttu-id="7a9e9-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7a9e9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7a9e9-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a9e9-123">Validation file</span></span>  <br/> |<span data-ttu-id="7a9e9-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7a9e9-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a9e9-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7a9e9-125">Can be empty</span></span>  <br/> |<span data-ttu-id="7a9e9-126">false</span><span class="sxs-lookup"><span data-stu-id="7a9e9-126">false</span></span>  <br/> |
   

