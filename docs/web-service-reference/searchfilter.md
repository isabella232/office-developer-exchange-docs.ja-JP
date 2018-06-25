---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: SearchFilter 要素には、GetSearchableMailboxes 要求から返されるメールボックスをフィルター処理するクエリ文字列が含まれています。
ms.openlocfilehash: b71d8dd862e9338afc145545df4cd29e8bcc3dc8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833285"
---
# <a name="searchfilter"></a><span data-ttu-id="7c330-103">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="7c330-103">SearchFilter</span></span>

<span data-ttu-id="7c330-104">**SearchFilter**要素には、 **GetSearchableMailboxes**要求から返されるメールボックスをフィルター処理するクエリ文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c330-104">The **SearchFilter** element contains the query string to filter the mailboxes to be returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchFilter></SearchFilter>
```

 <span data-ttu-id="7c330-105">**string**</span><span class="sxs-lookup"><span data-stu-id="7c330-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c330-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c330-106">Attributes and elements</span></span>

<span data-ttu-id="7c330-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c330-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c330-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c330-108">Attributes</span></span>

<span data-ttu-id="7c330-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c330-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c330-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c330-110">Child elements</span></span>

<span data-ttu-id="7c330-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7c330-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c330-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7c330-112">Parent elements</span></span>

[<span data-ttu-id="7c330-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7c330-113">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="7c330-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7c330-114">Text value</span></span>

<span data-ttu-id="7c330-115">**SearchFilter**要素のテキスト値は、探索検索メールボックスをフィルターするクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="7c330-115">The text value of the **SearchFilter** element is a query string to filter mailboxes for discovery search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7c330-116">備考</span><span class="sxs-lookup"><span data-stu-id="7c330-116">Remarks</span></span>

<span data-ttu-id="7c330-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7c330-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c330-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c330-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c330-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c330-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c330-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c330-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c330-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c330-121">Schema name</span></span>  <br/> |<span data-ttu-id="7c330-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c330-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7c330-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c330-123">Validation file</span></span>  <br/> |<span data-ttu-id="7c330-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c330-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c330-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7c330-125">Can be empty</span></span>  <br/> ||
   

