---
title: MailboxStatisticsSearchResult
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 73499df7-3d50-4e39-895d-6e15dd8b2777
description: MailboxStatisticsSearchResult 要素には、キーワード検索の結果が含まれています。
ms.openlocfilehash: c300c6c2ec9ab3c772709edd3e6a1c7fea19d6e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44440849"
---
# <a name="mailboxstatisticssearchresult"></a><span data-ttu-id="d830b-103">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="d830b-103">MailboxStatisticsSearchResult</span></span>

<span data-ttu-id="d830b-104">**MailboxStatisticsSearchResult**要素には、キーワード検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d830b-104">The **MailboxStatisticsSearchResult** element contains the results of a keyword search.</span></span> 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

<span data-ttu-id="d830b-105">**MailboxStatisticsSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="d830b-105">**MailboxStatisticsSearchResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d830b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d830b-106">Attributes and elements</span></span>

<span data-ttu-id="d830b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d830b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d830b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d830b-108">Attributes</span></span>

<span data-ttu-id="d830b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d830b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d830b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d830b-110">Child elements</span></span>

<span data-ttu-id="d830b-111">[Usermailbox](usermailbox.md)  | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="d830b-111">[UserMailbox](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d830b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d830b-112">Parent elements</span></span>

[<span data-ttu-id="d830b-113">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d830b-113">FindMailboxStatisticsByKeywordsResponseMessage</span></span>](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="d830b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d830b-114">Remarks</span></span>

<span data-ttu-id="d830b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d830b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d830b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d830b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d830b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d830b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d830b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d830b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d830b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d830b-119">Schema name</span></span>  <br/> |<span data-ttu-id="d830b-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d830b-120">messages schema</span></span>  <br/> |
|<span data-ttu-id="d830b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d830b-121">Validation file</span></span>  <br/> |<span data-ttu-id="d830b-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d830b-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d830b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d830b-123">Can be empty</span></span>  <br/> ||
   

