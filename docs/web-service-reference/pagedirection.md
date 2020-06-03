---
title: ページの方向
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 013947f3-cf3c-40b1-baf6-405f26bd375e
description: PageDirection 要素には、検索結果の改ページ位置の方向が含まれています。 値が Previous または Next。
ms.openlocfilehash: 22816ff73af49e0f029b5618fa3d45f8880d0f82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459729"
---
# <a name="pagedirection"></a><span data-ttu-id="97525-104">ページの方向</span><span class="sxs-lookup"><span data-stu-id="97525-104">PageDirection</span></span>

<span data-ttu-id="97525-105">**Pagedirection**要素には、検索結果の改ページ位置の方向が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97525-105">The **PageDirection** element contains the direction for pagination in the search result.</span></span> <span data-ttu-id="97525-106">値が Previous または Next。</span><span class="sxs-lookup"><span data-stu-id="97525-106">The value is Previous or Next.</span></span> 
  
```XML
<PageDirection> Previous | Next </PageDirection>
```

 <span data-ttu-id="97525-107">**Searchpagedirection 型**</span><span class="sxs-lookup"><span data-stu-id="97525-107">**SearchPageDirectionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97525-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="97525-108">Attributes and elements</span></span>

<span data-ttu-id="97525-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97525-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97525-110">属性</span><span class="sxs-lookup"><span data-stu-id="97525-110">Attributes</span></span>

<span data-ttu-id="97525-111">なし。</span><span class="sxs-lookup"><span data-stu-id="97525-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97525-112">子要素</span><span class="sxs-lookup"><span data-stu-id="97525-112">Child elements</span></span>

<span data-ttu-id="97525-113">なし。</span><span class="sxs-lookup"><span data-stu-id="97525-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97525-114">親要素</span><span class="sxs-lookup"><span data-stu-id="97525-114">Parent elements</span></span>

<span data-ttu-id="97525-115">[Searchmailboxes ボックス](searchmailboxes.md)  | [Getnonindexableitemdetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="97525-115">[SearchMailboxes](searchmailboxes.md) | [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="97525-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="97525-116">Text value</span></span>

<span data-ttu-id="97525-117">**Pagedirection**要素のテキスト値は、検索結果のページネーションの方向です。</span><span class="sxs-lookup"><span data-stu-id="97525-117">The text value of the **PageDirection** element is the direction for pagination the search results.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="97525-118">注釈</span><span class="sxs-lookup"><span data-stu-id="97525-118">Remarks</span></span>

<span data-ttu-id="97525-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="97525-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97525-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="97525-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97525-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="97525-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97525-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="97525-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97525-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="97525-123">Schema name</span></span>  <br/> |<span data-ttu-id="97525-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="97525-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97525-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="97525-125">Validation file</span></span>  <br/> |<span data-ttu-id="97525-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="97525-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97525-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97525-127">Can be empty</span></span>  <br/> ||
   

