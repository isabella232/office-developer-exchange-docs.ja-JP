---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: QueryString 要素は、FindPeople 操作要求のクエリ文字列に一致する、返される値のセットを指定します。 QueryString が指定されていない検索では、指定されたフォルダーからすべてのアイテムが返されます。
ms.openlocfilehash: ec025f86d3e6fb74810e9c539eba102d05adbb93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465325"
---
# <a name="querystring-string"></a><span data-ttu-id="6c99f-104">QueryString (String)</span><span class="sxs-lookup"><span data-stu-id="6c99f-104">QueryString (String)</span></span>

<span data-ttu-id="6c99f-105">**QueryString**要素は、 [findpeople 操作](findpeople-operation.md)要求のクエリ文字列に一致する、返される値のセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c99f-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="6c99f-106">**QueryString**が指定されていない検索では、指定されたフォルダーからすべてのアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c99f-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="6c99f-107">**string**</span><span class="sxs-lookup"><span data-stu-id="6c99f-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c99f-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c99f-108">Attributes and elements</span></span>

<span data-ttu-id="6c99f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c99f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c99f-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c99f-110">Attributes</span></span>

<span data-ttu-id="6c99f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c99f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c99f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c99f-112">Child elements</span></span>

<span data-ttu-id="6c99f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6c99f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c99f-114">親要素</span><span class="sxs-lookup"><span data-stu-id="6c99f-114">Parent elements</span></span>

|<span data-ttu-id="6c99f-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c99f-115">**Element**</span></span>|<span data-ttu-id="6c99f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c99f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c99f-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="6c99f-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="6c99f-118">[Findpeople 操作](findpeople-operation.md)検索の引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c99f-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c99f-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c99f-119">Text value</span></span>

<span data-ttu-id="6c99f-120">**QueryString**テキスト値は、[高度なクエリ構文 (aqs)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx)のサブセットを使用して作成されたメールボックスクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="6c99f-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="6c99f-121">この要素の構文については、「 [QueryString (QueryStringType)](querystring-querystringtype.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c99f-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c99f-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6c99f-122">Remarks</span></span>

<span data-ttu-id="6c99f-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c99f-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c99f-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c99f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c99f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c99f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c99f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c99f-126">Schema name</span></span>  <br/> |<span data-ttu-id="6c99f-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c99f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c99f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c99f-128">Validation file</span></span>  <br/> |<span data-ttu-id="6c99f-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6c99f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c99f-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6c99f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="6c99f-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c99f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c99f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c99f-132">See also</span></span>



[<span data-ttu-id="6c99f-133">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="6c99f-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="6c99f-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c99f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

