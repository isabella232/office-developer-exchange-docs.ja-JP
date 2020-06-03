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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465283"
---
# <a name="resulttype"></a><span data-ttu-id="d78fd-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="d78fd-104">ResultType</span></span>

<span data-ttu-id="d78fd-105">**ResultType**要素には、実行する検索の種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d78fd-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="d78fd-106">検索の種類には、統計のみ、またはプレビューのみを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d78fd-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="d78fd-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="d78fd-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d78fd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d78fd-108">Attributes and elements</span></span>

<span data-ttu-id="d78fd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d78fd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d78fd-110">属性</span><span class="sxs-lookup"><span data-stu-id="d78fd-110">Attributes</span></span>

<span data-ttu-id="d78fd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d78fd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d78fd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d78fd-112">Child elements</span></span>

<span data-ttu-id="d78fd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d78fd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d78fd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="d78fd-114">Parent elements</span></span>

<span data-ttu-id="d78fd-115">[SearchMailboxesResult](searchmailboxesresult.md)  | [Searchmailboxes ボックス](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="d78fd-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d78fd-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d78fd-116">Text value</span></span>

<span data-ttu-id="d78fd-117">**ResultType**要素のテキスト値は、探索検索で返される結果の種類です。</span><span class="sxs-lookup"><span data-stu-id="d78fd-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="d78fd-118">**StatisticsOnly**のテキスト値は、検索統計を返します。</span><span class="sxs-lookup"><span data-stu-id="d78fd-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="d78fd-119">プレビュー**のみ**のテキスト値は、アイテムのプレビュー情報を返します。</span><span class="sxs-lookup"><span data-stu-id="d78fd-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d78fd-120">注釈</span><span class="sxs-lookup"><span data-stu-id="d78fd-120">Remarks</span></span>

<span data-ttu-id="d78fd-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d78fd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d78fd-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d78fd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d78fd-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d78fd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d78fd-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d78fd-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d78fd-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d78fd-125">Schema name</span></span>  <br/> |<span data-ttu-id="d78fd-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d78fd-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d78fd-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d78fd-127">Validation file</span></span>  <br/> |<span data-ttu-id="d78fd-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d78fd-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d78fd-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d78fd-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d78fd-130">false</span><span class="sxs-lookup"><span data-stu-id="d78fd-130">false</span></span>  <br/> |
   

