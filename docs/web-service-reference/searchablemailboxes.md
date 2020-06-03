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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467446"
---
# <a name="searchablemailboxes"></a><span data-ttu-id="cc4a2-103">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="cc4a2-103">SearchableMailboxes</span></span>

<span data-ttu-id="cc4a2-104">**Searchablemaillevel要素**には、 **getsearchablemailemailrequest**要求から返されるメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-104">The **SearchableMailboxes** element contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailboxes>
   <SearchableMailbox/>
</SearchableMailboxes>
```

 <span data-ttu-id="cc4a2-105">**Arrayofsearchablemailboxestoff**</span><span class="sxs-lookup"><span data-stu-id="cc4a2-105">**ArrayOfSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc4a2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc4a2-106">Attributes and elements</span></span>

<span data-ttu-id="cc4a2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc4a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc4a2-108">Attributes</span></span>

<span data-ttu-id="cc4a2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc4a2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc4a2-110">Child elements</span></span>

[<span data-ttu-id="cc4a2-111">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="cc4a2-111">SearchableMailbox</span></span>](searchablemailbox.md)
  
### <a name="parent-elements"></a><span data-ttu-id="cc4a2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cc4a2-112">Parent elements</span></span>

[<span data-ttu-id="cc4a2-113">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="cc4a2-113">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="cc4a2-114">注釈</span><span class="sxs-lookup"><span data-stu-id="cc4a2-114">Remarks</span></span>

<span data-ttu-id="cc4a2-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc4a2-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc4a2-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cc4a2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc4a2-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc4a2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc4a2-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc4a2-119">Schema name</span></span>  <br/> |<span data-ttu-id="cc4a2-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cc4a2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc4a2-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc4a2-121">Validation file</span></span>  <br/> |<span data-ttu-id="cc4a2-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cc4a2-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc4a2-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cc4a2-123">Can be empty</span></span>  <br/> ||
   

