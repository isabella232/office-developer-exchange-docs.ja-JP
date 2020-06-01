---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: ResultType 要素には、実行する検索の種類が含まれています。 検索の種類には、統計のみ、またはプレビューのみを指定できます。
ms.openlocfilehash: 6617c8b4b64cd9b6728317d7247bcc5378e488f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465283"
---
# <a name="resulttype"></a><span data-ttu-id="937c9-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="937c9-104">ResultType</span></span>

<span data-ttu-id="937c9-105">**ResultType**要素には、実行する検索の種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="937c9-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="937c9-106">検索の種類には、統計のみ、またはプレビューのみを指定できます。</span><span class="sxs-lookup"><span data-stu-id="937c9-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="937c9-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="937c9-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="937c9-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="937c9-108">Attributes and elements</span></span>

<span data-ttu-id="937c9-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="937c9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="937c9-110">属性</span><span class="sxs-lookup"><span data-stu-id="937c9-110">Attributes</span></span>

<span data-ttu-id="937c9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="937c9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="937c9-112">子要素</span><span class="sxs-lookup"><span data-stu-id="937c9-112">Child elements</span></span>

<span data-ttu-id="937c9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="937c9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="937c9-114">親要素</span><span class="sxs-lookup"><span data-stu-id="937c9-114">Parent elements</span></span>

<span data-ttu-id="937c9-115">[SearchMailboxesResult](searchmailboxesresult.md)  | [Searchmailboxes ボックス](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="937c9-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="937c9-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="937c9-116">Text value</span></span>

<span data-ttu-id="937c9-117">**ResultType**要素のテキスト値は、探索検索で返される結果の種類です。</span><span class="sxs-lookup"><span data-stu-id="937c9-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="937c9-118">**StatisticsOnly**のテキスト値は、検索統計を返します。</span><span class="sxs-lookup"><span data-stu-id="937c9-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="937c9-119">プレビュー**のみ**のテキスト値は、アイテムのプレビュー情報を返します。</span><span class="sxs-lookup"><span data-stu-id="937c9-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="937c9-120">注釈</span><span class="sxs-lookup"><span data-stu-id="937c9-120">Remarks</span></span>

<span data-ttu-id="937c9-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="937c9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="937c9-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="937c9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="937c9-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="937c9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="937c9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="937c9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="937c9-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="937c9-125">Schema name</span></span>  <br/> |<span data-ttu-id="937c9-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="937c9-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="937c9-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="937c9-127">Validation file</span></span>  <br/> |<span data-ttu-id="937c9-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="937c9-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="937c9-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="937c9-129">Can be empty</span></span>  <br/> |<span data-ttu-id="937c9-130">false</span><span class="sxs-lookup"><span data-stu-id="937c9-130">false</span></span>  <br/> |
   

