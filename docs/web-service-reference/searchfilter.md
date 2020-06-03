---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: SearchFilter 要素には、Getsearchablemailemailrequest から返されるメールボックスをフィルター処理するためのクエリ文字列が含まれています。
ms.openlocfilehash: 5bc7389ecc54dd6d1c97debdb97e6fce42517ef4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467432"
---
# <a name="searchfilter"></a><span data-ttu-id="6a87b-103">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="6a87b-103">SearchFilter</span></span>

<span data-ttu-id="6a87b-104">**Searchfilter**要素には、 **Getsearchablemailemailrequest**から返されるメールボックスをフィルター処理するためのクエリ文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a87b-104">The **SearchFilter** element contains the query string to filter the mailboxes to be returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchFilter></SearchFilter>
```

 <span data-ttu-id="6a87b-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6a87b-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a87b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a87b-106">Attributes and elements</span></span>

<span data-ttu-id="6a87b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a87b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a87b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a87b-108">Attributes</span></span>

<span data-ttu-id="6a87b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a87b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a87b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a87b-110">Child elements</span></span>

<span data-ttu-id="6a87b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6a87b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a87b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a87b-112">Parent elements</span></span>

[<span data-ttu-id="6a87b-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="6a87b-113">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="6a87b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a87b-114">Text value</span></span>

<span data-ttu-id="6a87b-115">**Searchfilter**要素のテキスト値は、探索検索用のメールボックスをフィルター処理するためのクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="6a87b-115">The text value of the **SearchFilter** element is a query string to filter mailboxes for discovery search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6a87b-116">注釈</span><span class="sxs-lookup"><span data-stu-id="6a87b-116">Remarks</span></span>

<span data-ttu-id="6a87b-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a87b-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a87b-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6a87b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a87b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a87b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a87b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a87b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6a87b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a87b-121">Schema name</span></span>  <br/> |<span data-ttu-id="6a87b-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6a87b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6a87b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a87b-123">Validation file</span></span>  <br/> |<span data-ttu-id="6a87b-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6a87b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a87b-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a87b-125">Can be empty</span></span>  <br/> ||
   

