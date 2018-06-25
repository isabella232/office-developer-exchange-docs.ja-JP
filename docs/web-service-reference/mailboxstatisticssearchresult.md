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
ms.openlocfilehash: 5b40622cf15596d7ab8a7fa09c9a1998092c3ee7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832302"
---
# <a name="mailboxstatisticssearchresult"></a><span data-ttu-id="2e7d4-103">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="2e7d4-103">MailboxStatisticsSearchResult</span></span>

<span data-ttu-id="2e7d4-104">**MailboxStatisticsSearchResult**要素には、キーワード検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-104">The **MailboxStatisticsSearchResult** element contains the results of a keyword search.</span></span> 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

<span data-ttu-id="2e7d4-105">**MailboxStatisticsSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="2e7d4-105">**MailboxStatisticsSearchResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2e7d4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2e7d4-106">Attributes and elements</span></span>

<span data-ttu-id="2e7d4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e7d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e7d4-108">Attributes</span></span>

<span data-ttu-id="2e7d4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e7d4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2e7d4-110">Child elements</span></span>

<span data-ttu-id="2e7d4-111">[構成](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e7d4-111">[UserMailbox](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e7d4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2e7d4-112">Parent elements</span></span>

[<span data-ttu-id="2e7d4-113">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2e7d4-113">FindMailboxStatisticsByKeywordsResponseMessage</span></span>](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="2e7d4-114">備考</span><span class="sxs-lookup"><span data-stu-id="2e7d4-114">Remarks</span></span>

<span data-ttu-id="2e7d4-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e7d4-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e7d4-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="2e7d4-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e7d4-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="2e7d4-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e7d4-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2e7d4-119">Schema name</span></span>  <br/> |<span data-ttu-id="2e7d4-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2e7d4-120">messages schema</span></span>  <br/> |
|<span data-ttu-id="2e7d4-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2e7d4-121">Validation file</span></span>  <br/> |<span data-ttu-id="2e7d4-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2e7d4-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e7d4-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2e7d4-123">Can be empty</span></span>  <br/> ||
   

