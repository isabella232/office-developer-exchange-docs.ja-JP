---
title: クエリ文字列 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: クエリ文字列要素は、FindPeople の操作要求のクエリ文字列に一致する返される値のセットを指定します。 指定なしのクエリ文字列の検索は、指定したフォルダーからすべての項目を返します。
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832935"
---
# <a name="querystring-string"></a><span data-ttu-id="34b8d-104">クエリ文字列 (文字列)</span><span class="sxs-lookup"><span data-stu-id="34b8d-104">QueryString (String)</span></span>

<span data-ttu-id="34b8d-105">**クエリ文字列**要素は、 [FindPeople 操作](findpeople-operation.md)の要求のクエリ文字列に一致する返される値のセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="34b8d-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="34b8d-106">指定されていない**クエリ文字列**の検索は、指定したフォルダーからすべての項目を返します。</span><span class="sxs-lookup"><span data-stu-id="34b8d-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="34b8d-107">**string**</span><span class="sxs-lookup"><span data-stu-id="34b8d-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34b8d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="34b8d-108">Attributes and elements</span></span>

<span data-ttu-id="34b8d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="34b8d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34b8d-110">属性</span><span class="sxs-lookup"><span data-stu-id="34b8d-110">Attributes</span></span>

<span data-ttu-id="34b8d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="34b8d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34b8d-112">子要素</span><span class="sxs-lookup"><span data-stu-id="34b8d-112">Child elements</span></span>

<span data-ttu-id="34b8d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="34b8d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34b8d-114">親要素</span><span class="sxs-lookup"><span data-stu-id="34b8d-114">Parent elements</span></span>

|<span data-ttu-id="34b8d-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="34b8d-115">**Element**</span></span>|<span data-ttu-id="34b8d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="34b8d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34b8d-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="34b8d-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="34b8d-118">[FindPeople 操作](findpeople-operation.md)の検索の引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="34b8d-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34b8d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="34b8d-119">Text value</span></span>

<span data-ttu-id="34b8d-120">**クエリ文字列**のテキスト値では、[高度なクエリ構文 (AQS)](http://msdn.microsoft.com/ja-jp/library/aa965711%28VS.85%29.aspx)のサブセットを使用してメールボックスのクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="34b8d-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/ja-jp/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="34b8d-121">この要素の構文については、[クエリ文字列 (QueryStringType)](querystring-querystringtype.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34b8d-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34b8d-122">備考</span><span class="sxs-lookup"><span data-stu-id="34b8d-122">Remarks</span></span>

<span data-ttu-id="34b8d-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="34b8d-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34b8d-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="34b8d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34b8d-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="34b8d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34b8d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="34b8d-126">Schema name</span></span>  <br/> |<span data-ttu-id="34b8d-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="34b8d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34b8d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="34b8d-128">Validation file</span></span>  <br/> |<span data-ttu-id="34b8d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="34b8d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34b8d-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="34b8d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="34b8d-131">False</span><span class="sxs-lookup"><span data-stu-id="34b8d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34b8d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="34b8d-132">See also</span></span>



[<span data-ttu-id="34b8d-133">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="34b8d-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="34b8d-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="34b8d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

