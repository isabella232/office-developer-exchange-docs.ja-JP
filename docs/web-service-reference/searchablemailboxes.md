---
title: SearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eb0a7897-c642-4c93-a238-be03128af54e
description: Searchablemaillevel要素には、Getsearchablemailemailrequest 要求から返されるメールボックスの配列が含まれています。
ms.openlocfilehash: 5de15e1c2ae4a587052f836b189651450a1e7482
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467446"
---
# <a name="searchablemailboxes"></a><span data-ttu-id="0585f-103">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0585f-103">SearchableMailboxes</span></span>

<span data-ttu-id="0585f-104">**Searchablemaillevel要素**には、 **getsearchablemailemailrequest**要求から返されるメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0585f-104">The **SearchableMailboxes** element contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailboxes>
   <SearchableMailbox/>
</SearchableMailboxes>
```

 <span data-ttu-id="0585f-105">**Arrayofsearchablemailboxestoff**</span><span class="sxs-lookup"><span data-stu-id="0585f-105">**ArrayOfSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0585f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0585f-106">Attributes and elements</span></span>

<span data-ttu-id="0585f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0585f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0585f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0585f-108">Attributes</span></span>

<span data-ttu-id="0585f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0585f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0585f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0585f-110">Child elements</span></span>

[<span data-ttu-id="0585f-111">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="0585f-111">SearchableMailbox</span></span>](searchablemailbox.md)
  
### <a name="parent-elements"></a><span data-ttu-id="0585f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0585f-112">Parent elements</span></span>

[<span data-ttu-id="0585f-113">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="0585f-113">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="0585f-114">注釈</span><span class="sxs-lookup"><span data-stu-id="0585f-114">Remarks</span></span>

<span data-ttu-id="0585f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0585f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0585f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0585f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0585f-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0585f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0585f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="0585f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0585f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0585f-119">Schema name</span></span>  <br/> |<span data-ttu-id="0585f-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0585f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0585f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0585f-121">Validation file</span></span>  <br/> |<span data-ttu-id="0585f-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0585f-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0585f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0585f-123">Can be empty</span></span>  <br/> ||
   

