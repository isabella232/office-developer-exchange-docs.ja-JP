---
title: 結果
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: 結果の要素には、実行する検索の種類が含まれています。 検索の種類では、統計情報のみをするしたり、のみをプレビューすることができます。
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833211"
---
# <a name="resulttype"></a><span data-ttu-id="307b7-104">結果</span><span class="sxs-lookup"><span data-stu-id="307b7-104">ResultType</span></span>

<span data-ttu-id="307b7-105">**結果**の要素には、実行する検索の種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="307b7-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="307b7-106">検索の種類では、統計情報のみをするしたり、のみをプレビューすることができます。</span><span class="sxs-lookup"><span data-stu-id="307b7-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="307b7-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="307b7-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="307b7-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="307b7-108">Attributes and elements</span></span>

<span data-ttu-id="307b7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="307b7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="307b7-110">属性</span><span class="sxs-lookup"><span data-stu-id="307b7-110">Attributes</span></span>

<span data-ttu-id="307b7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="307b7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="307b7-112">子要素</span><span class="sxs-lookup"><span data-stu-id="307b7-112">Child elements</span></span>

<span data-ttu-id="307b7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="307b7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="307b7-114">親要素</span><span class="sxs-lookup"><span data-stu-id="307b7-114">Parent elements</span></span>

<span data-ttu-id="307b7-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="307b7-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="307b7-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="307b7-116">Text value</span></span>

<span data-ttu-id="307b7-117">**結果**要素のテキスト値は、探索の検索で返される結果の型です。</span><span class="sxs-lookup"><span data-stu-id="307b7-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="307b7-118">**StatisticsOnly**のテキスト値では、検索の統計情報を返します。</span><span class="sxs-lookup"><span data-stu-id="307b7-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="307b7-119">**PreviewOnly**のテキスト値では、アイテムのプレビュー情報を返します。</span><span class="sxs-lookup"><span data-stu-id="307b7-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="307b7-120">備考</span><span class="sxs-lookup"><span data-stu-id="307b7-120">Remarks</span></span>

<span data-ttu-id="307b7-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="307b7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="307b7-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="307b7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="307b7-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="307b7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="307b7-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="307b7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="307b7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="307b7-125">Schema name</span></span>  <br/> |<span data-ttu-id="307b7-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="307b7-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="307b7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="307b7-127">Validation file</span></span>  <br/> |<span data-ttu-id="307b7-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="307b7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="307b7-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="307b7-129">Can be empty</span></span>  <br/> |<span data-ttu-id="307b7-130">false</span><span class="sxs-lookup"><span data-stu-id="307b7-130">false</span></span>  <br/> |
   

