---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: SearchMailboxesResult 要素には、SearchMailboxes ボックス要求の結果が含まれています。
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466704"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="e76f2-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="e76f2-103">SearchMailboxesResult</span></span>

<span data-ttu-id="e76f2-104">**SearchMailboxesResult**要素には、 **searchmailboxes ボックス**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e76f2-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="e76f2-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="e76f2-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e76f2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e76f2-106">Attributes and elements</span></span>

<span data-ttu-id="e76f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e76f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e76f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="e76f2-108">Attributes</span></span>

<span data-ttu-id="e76f2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e76f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e76f2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e76f2-110">Child elements</span></span>

<span data-ttu-id="e76f2-111">[Searchqueries](searchqueries.md)  | [ResultType](resulttype.md)  | [ItemCount](itemcount.md)  | [サイズ (長い)](size-long.md)  | [PageItemCount](pageitemcount.md)  | [Pageitemsize](pageitemsize.md)  | [KeywordStats](keywordstats.md)  | [アイテム (Arrayofsearchプレビュー Itemstype)](items-arrayofsearchpreviewitemstype.md)  | [失敗したメールボックス](failedmailboxes.md)  | [絞り込み条件](refiners.md)  | [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="e76f2-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e76f2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e76f2-112">Parent elements</span></span>

[<span data-ttu-id="e76f2-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e76f2-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="e76f2-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e76f2-114">Remarks</span></span>

<span data-ttu-id="e76f2-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e76f2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e76f2-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e76f2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e76f2-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e76f2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e76f2-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e76f2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e76f2-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e76f2-119">Schema name</span></span>  <br/> |<span data-ttu-id="e76f2-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e76f2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e76f2-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e76f2-121">Validation file</span></span>  <br/> |<span data-ttu-id="e76f2-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e76f2-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e76f2-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e76f2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e76f2-124">false</span><span class="sxs-lookup"><span data-stu-id="e76f2-124">false</span></span>  <br/> |
   

