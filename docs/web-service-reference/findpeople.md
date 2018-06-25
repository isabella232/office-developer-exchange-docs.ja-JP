---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'FindPeople 要素は、FindPeople 要求で使用されるデータのセットを指定します。 次の要素の 0 個以上のデータが含まれています: ペルソナの図形 (オプション)、ページのインデックス付きのアイテム ビュー、制限 (省略可能) に集約が制限 (省略可能)、(省略可能) の並べ替え順序、親フォルダー Id、およびクエリ文字列 (省略可能)。'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760531"
---
# <a name="findpeople"></a><span data-ttu-id="dc85d-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="dc85d-104">FindPeople</span></span>

<span data-ttu-id="dc85d-105">**FindPeople**要素は、FindPeople 要求で使用されるデータのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc85d-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="dc85d-106">次の要素の 0 個以上のデータが含まれています: ペルソナの図形 (オプション)、ページのインデックス付きのアイテム ビュー、制限 (省略可能) に集約が制限 (省略可能)、(省略可能) の並べ替え順序、親フォルダー Id、およびクエリ文字列 (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="dc85d-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
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

 <span data-ttu-id="dc85d-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="dc85d-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc85d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dc85d-108">Attributes and elements</span></span>

<span data-ttu-id="dc85d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc85d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc85d-110">属性</span><span class="sxs-lookup"><span data-stu-id="dc85d-110">Attributes</span></span>

<span data-ttu-id="dc85d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dc85d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc85d-112">子要素</span><span class="sxs-lookup"><span data-stu-id="dc85d-112">Child elements</span></span>

<span data-ttu-id="dc85d-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [制限](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [ソート順序](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [クエリ文字列 (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="dc85d-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc85d-114">親要素</span><span class="sxs-lookup"><span data-stu-id="dc85d-114">Parent elements</span></span>

<span data-ttu-id="dc85d-115">なし。</span><span class="sxs-lookup"><span data-stu-id="dc85d-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc85d-116">備考</span><span class="sxs-lookup"><span data-stu-id="dc85d-116">Remarks</span></span>

<span data-ttu-id="dc85d-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dc85d-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dc85d-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dc85d-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc85d-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="dc85d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc85d-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="dc85d-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc85d-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc85d-121">Schema name</span></span>  <br/> |<span data-ttu-id="dc85d-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc85d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc85d-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc85d-123">Validation file</span></span>  <br/> |<span data-ttu-id="dc85d-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dc85d-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc85d-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dc85d-125">Can be empty</span></span>  <br/> |<span data-ttu-id="dc85d-126">false</span><span class="sxs-lookup"><span data-stu-id="dc85d-126">false</span></span>  <br/> |
   

