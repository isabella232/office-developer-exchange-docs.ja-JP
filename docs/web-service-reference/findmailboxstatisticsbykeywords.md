---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: FindMailboxStatisticsByKeywords 要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760517"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="e86fc-103">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="e86fc-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="e86fc-104">**FindMailboxStatisticsByKeywords**要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 <span data-ttu-id="e86fc-105">**FindMailboxStatisticsByKeywordsType**</span><span class="sxs-lookup"><span data-stu-id="e86fc-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e86fc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e86fc-106">Attributes and elements</span></span>

<span data-ttu-id="e86fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e86fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="e86fc-108">Attributes</span></span>

<span data-ttu-id="e86fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e86fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e86fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e86fc-110">Child elements</span></span>

|<span data-ttu-id="e86fc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e86fc-111">**Element**</span></span>|<span data-ttu-id="e86fc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e86fc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e86fc-113">メールボックス (ArrayOfUserMailboxesType)</span><span class="sxs-lookup"><span data-stu-id="e86fc-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="e86fc-114">保留リストの影響を受けるメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e86fc-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-115">Keywords</span><span class="sxs-lookup"><span data-stu-id="e86fc-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e86fc-116">検索のキーワードを指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-117">Language</span><span class="sxs-lookup"><span data-stu-id="e86fc-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="e86fc-118">検索クエリで使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e86fc-118">Contains the language used for the search query.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-119">送信者</span><span class="sxs-lookup"><span data-stu-id="e86fc-119">Senders</span></span>](senders.md) <br/> |<span data-ttu-id="e86fc-120">SMTP アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-121">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="e86fc-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="e86fc-122">メッセージの受信者の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|<span data-ttu-id="e86fc-123">[[開始日](fromdate.md)</span><span class="sxs-lookup"><span data-stu-id="e86fc-123">[FromDate](fromdate.md)</span></span> <br/> |<span data-ttu-id="e86fc-124">メッセージが送信された日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-125">ToDate</span><span class="sxs-lookup"><span data-stu-id="e86fc-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="e86fc-126">メッセージを受信した日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-127">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="e86fc-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="e86fc-128">検索するメッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-129">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="e86fc-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="e86fc-130">削除済みアイテムを検索するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-131">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="e86fc-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="e86fc-132">個人用アーカイブを検索に含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="e86fc-133">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="e86fc-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="e86fc-134">検索できない項目を含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e86fc-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e86fc-135">親要素</span><span class="sxs-lookup"><span data-stu-id="e86fc-135">Parent elements</span></span>

<span data-ttu-id="e86fc-136">なし。</span><span class="sxs-lookup"><span data-stu-id="e86fc-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e86fc-137">備考</span><span class="sxs-lookup"><span data-stu-id="e86fc-137">Remarks</span></span>

<span data-ttu-id="e86fc-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e86fc-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e86fc-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="e86fc-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e86fc-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="e86fc-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e86fc-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e86fc-141">Schema Name</span></span>  <br/> |<span data-ttu-id="e86fc-142">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e86fc-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="e86fc-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e86fc-143">Validation File</span></span>  <br/> |<span data-ttu-id="e86fc-144">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e86fc-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e86fc-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e86fc-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e86fc-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="e86fc-146">See also</span></span>



- [<span data-ttu-id="e86fc-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e86fc-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

