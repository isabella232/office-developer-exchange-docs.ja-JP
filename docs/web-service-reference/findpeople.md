---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: FindPeople 要素は、FindPeople 要求で使用されるデータのセットを指定します。 データには、次の要素の0つ以上が含まれます。ペルソナ図形 (省略可能)、インデックス付きページアイテムビュー、制限 (省略可能)、集計制限 (省略可能)、並べ替え順序 (省略可能)、親フォルダー Id、およびクエリ文字列 (省略可能)。
ms.openlocfilehash: 4777601b7146ec857b5c79fa9d4ced59a7247889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462902"
---
# <a name="findpeople"></a><span data-ttu-id="e8d1c-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="e8d1c-104">FindPeople</span></span>

<span data-ttu-id="e8d1c-105">**Findpeople**要素は、findpeople 要求で使用されるデータのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="e8d1c-106">データには、次の要素の0つ以上が含まれます。ペルソナ図形 (省略可能)、インデックス付きページアイテムビュー、制限 (省略可能)、集計制限 (省略可能)、並べ替え順序 (省略可能)、親フォルダー Id、およびクエリ文字列 (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 <span data-ttu-id="e8d1c-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="e8d1c-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8d1c-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8d1c-108">Attributes and elements</span></span>

<span data-ttu-id="e8d1c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8d1c-110">属性</span><span class="sxs-lookup"><span data-stu-id="e8d1c-110">Attributes</span></span>

<span data-ttu-id="e8d1c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8d1c-112">子要素</span><span class="sxs-lookup"><span data-stu-id="e8d1c-112">Child elements</span></span>

<span data-ttu-id="e8d1c-113">[PersonaShape](personashape.md)  | [Indexedpageitemview](indexedpageitemview.md)  | [制限](restriction.md)  | [集約 Ationrestriction](aggregationrestriction.md)  | [ソート順序](sortorder.md)  | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  | [QueryString (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="e8d1c-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8d1c-114">親要素</span><span class="sxs-lookup"><span data-stu-id="e8d1c-114">Parent elements</span></span>

<span data-ttu-id="e8d1c-115">なし。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8d1c-116">注釈</span><span class="sxs-lookup"><span data-stu-id="e8d1c-116">Remarks</span></span>

<span data-ttu-id="e8d1c-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8d1c-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8d1c-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8d1c-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8d1c-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8d1c-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8d1c-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8d1c-121">Schema name</span></span>  <br/> |<span data-ttu-id="e8d1c-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e8d1c-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8d1c-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8d1c-123">Validation file</span></span>  <br/> |<span data-ttu-id="e8d1c-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e8d1c-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8d1c-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8d1c-125">Can be empty</span></span>  <br/> |<span data-ttu-id="e8d1c-126">false</span><span class="sxs-lookup"><span data-stu-id="e8d1c-126">false</span></span>  <br/> |
   

