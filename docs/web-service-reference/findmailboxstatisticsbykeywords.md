---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: FindMailboxStatisticsByKeywords 要素は、キーワードによってメールボックス統計情報を検索する要求を指定します。
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462529"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="fca13-103">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="fca13-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="fca13-104">**FindMailboxStatisticsByKeywords**要素は、キーワードによってメールボックス統計情報を検索する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
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

 <span data-ttu-id="fca13-105">**FindMailboxStatisticsByKeywordsType**</span><span class="sxs-lookup"><span data-stu-id="fca13-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fca13-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fca13-106">Attributes and elements</span></span>

<span data-ttu-id="fca13-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fca13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fca13-108">属性</span><span class="sxs-lookup"><span data-stu-id="fca13-108">Attributes</span></span>

<span data-ttu-id="fca13-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fca13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fca13-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fca13-110">Child elements</span></span>

|<span data-ttu-id="fca13-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="fca13-111">**Element**</span></span>|<span data-ttu-id="fca13-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fca13-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fca13-113">メールボックス (ArrayOfUserMailboxesType)</span><span class="sxs-lookup"><span data-stu-id="fca13-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="fca13-114">保留の影響を受けるメールボックスの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="fca13-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="fca13-115">Keywords</span><span class="sxs-lookup"><span data-stu-id="fca13-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fca13-116">検索のキーワードを指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="fca13-117">Language</span><span class="sxs-lookup"><span data-stu-id="fca13-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="fca13-118">検索クエリに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fca13-118">Contains the language used for the search query.</span></span>  <br/> |
|<span data-ttu-id="fca13-119">[[Senders (送信者)](senders.md)]</span><span class="sxs-lookup"><span data-stu-id="fca13-119">[Senders](senders.md)</span></span> <br/> |<span data-ttu-id="fca13-120">SMTP アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="fca13-121">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="fca13-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="fca13-122">メッセージの受信者の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="fca13-123">FromDate</span><span class="sxs-lookup"><span data-stu-id="fca13-123">FromDate</span></span>](fromdate.md) <br/> |<span data-ttu-id="fca13-124">メッセージが送信された日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="fca13-125">半年</span><span class="sxs-lookup"><span data-stu-id="fca13-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="fca13-126">メッセージが受信された日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="fca13-127">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="fca13-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="fca13-128">検索するメッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="fca13-129">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="fca13-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="fca13-130">削除済みアイテムを検索するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="fca13-131">Includeパーソナルアーカイブ</span><span class="sxs-lookup"><span data-stu-id="fca13-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="fca13-132">検索に個人用アーカイブを含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="fca13-133">Include非 Searchableitems</span><span class="sxs-lookup"><span data-stu-id="fca13-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="fca13-134">検索できないアイテムを含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fca13-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fca13-135">親要素</span><span class="sxs-lookup"><span data-stu-id="fca13-135">Parent elements</span></span>

<span data-ttu-id="fca13-136">なし。</span><span class="sxs-lookup"><span data-stu-id="fca13-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fca13-137">注釈</span><span class="sxs-lookup"><span data-stu-id="fca13-137">Remarks</span></span>

<span data-ttu-id="fca13-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fca13-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fca13-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fca13-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fca13-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="fca13-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fca13-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fca13-141">Schema Name</span></span>  <br/> |<span data-ttu-id="fca13-142">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fca13-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="fca13-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fca13-143">Validation File</span></span>  <br/> |<span data-ttu-id="fca13-144">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fca13-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fca13-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fca13-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fca13-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="fca13-146">See also</span></span>



- [<span data-ttu-id="fca13-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fca13-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

