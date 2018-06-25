---
title: SearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eb0a7897-c642-4c93-a238-be03128af54e
description: SearchableMailboxes 要素には、GetSearchableMailboxes 要求から返されたメールボックスの配列が含まれています。
ms.openlocfilehash: 5e8fdfbf4e0087b3fc514cd68b92b746cfb70db4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833289"
---
# <a name="searchablemailboxes"></a><span data-ttu-id="dd054-103">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="dd054-103">SearchableMailboxes</span></span>

<span data-ttu-id="dd054-104">**SearchableMailboxes**要素には、 **GetSearchableMailboxes**要求から返されたメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd054-104">The **SearchableMailboxes** element contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailboxes>
   <SearchableMailbox/>
</SearchableMailboxes>
```

 <span data-ttu-id="dd054-105">**ArrayOfSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="dd054-105">**ArrayOfSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd054-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd054-106">Attributes and elements</span></span>

<span data-ttu-id="dd054-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd054-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd054-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd054-108">Attributes</span></span>

<span data-ttu-id="dd054-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd054-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd054-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd054-110">Child elements</span></span>

[<span data-ttu-id="dd054-111">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="dd054-111">SearchableMailbox</span></span>](searchablemailbox.md)
  
### <a name="parent-elements"></a><span data-ttu-id="dd054-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd054-112">Parent elements</span></span>

[<span data-ttu-id="dd054-113">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="dd054-113">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="dd054-114">備考</span><span class="sxs-lookup"><span data-stu-id="dd054-114">Remarks</span></span>

<span data-ttu-id="dd054-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dd054-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dd054-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dd054-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd054-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd054-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd054-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd054-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd054-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd054-119">Schema name</span></span>  <br/> |<span data-ttu-id="dd054-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dd054-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd054-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd054-121">Validation file</span></span>  <br/> |<span data-ttu-id="dd054-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd054-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd054-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dd054-123">Can be empty</span></span>  <br/> ||
   

