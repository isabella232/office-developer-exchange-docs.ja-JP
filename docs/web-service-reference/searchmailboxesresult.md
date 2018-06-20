---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: SearchMailboxesResult 要素には、SearchMailboxes 要求の結果が含まれています。
ms.openlocfilehash: 93e5837216ef8942b77ac2a91f5ef5f0ad001756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833300"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="529cf-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="529cf-103">SearchMailboxesResult</span></span>

<span data-ttu-id="529cf-104">**SearchMailboxesResult**要素には、 **SearchMailboxes**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="529cf-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 <span data-ttu-id="529cf-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="529cf-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="529cf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="529cf-106">Attributes and elements</span></span>

<span data-ttu-id="529cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="529cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="529cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="529cf-108">Attributes</span></span>

<span data-ttu-id="529cf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="529cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="529cf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="529cf-110">Child elements</span></span>

<span data-ttu-id="529cf-111">[SearchQueries](searchqueries.md) | [結果](resulttype.md) | [ItemCount](itemcount.md) | [サイズ (長)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [(の項目ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [絞り込み条件](refiners.md) | [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="529cf-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="529cf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="529cf-112">Parent elements</span></span>

[<span data-ttu-id="529cf-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="529cf-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="529cf-114">備考</span><span class="sxs-lookup"><span data-stu-id="529cf-114">Remarks</span></span>

<span data-ttu-id="529cf-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="529cf-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="529cf-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="529cf-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="529cf-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="529cf-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="529cf-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="529cf-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="529cf-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="529cf-119">Schema name</span></span>  <br/> |<span data-ttu-id="529cf-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="529cf-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="529cf-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="529cf-121">Validation file</span></span>  <br/> |<span data-ttu-id="529cf-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="529cf-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="529cf-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="529cf-123">Can be empty</span></span>  <br/> |<span data-ttu-id="529cf-124">false</span><span class="sxs-lookup"><span data-stu-id="529cf-124">false</span></span>  <br/> |
   

