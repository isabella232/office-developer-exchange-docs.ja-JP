---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: QueryString 要素には、高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列が含まれています。
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459189"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="2ab91-103">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="2ab91-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="2ab91-104">**QueryString**要素には、高度なクエリ構文 (aqs) に基づくメールボックスクエリ文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="2ab91-105">**QueryStringType**</span><span class="sxs-lookup"><span data-stu-id="2ab91-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ab91-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2ab91-106">Attributes and elements</span></span>

<span data-ttu-id="2ab91-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ab91-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ab91-108">Attributes</span></span>

|<span data-ttu-id="2ab91-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2ab91-109">**Attribute**</span></span>|<span data-ttu-id="2ab91-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2ab91-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ab91-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="2ab91-111">ResetCache</span></span>  <br/> |<span data-ttu-id="2ab91-112">キャッシュをリセットする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="2ab91-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="2ab91-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="2ab91-114">削除されたアイテムが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="2ab91-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="2ab91-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="2ab91-116">強調表示された用語を返すことを示します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2ab91-117">子要素</span><span class="sxs-lookup"><span data-stu-id="2ab91-117">Child elements</span></span>

<span data-ttu-id="2ab91-118">なし。</span><span class="sxs-lookup"><span data-stu-id="2ab91-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ab91-119">親要素</span><span class="sxs-lookup"><span data-stu-id="2ab91-119">Parent elements</span></span>

|<span data-ttu-id="2ab91-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="2ab91-120">**Element**</span></span>|<span data-ttu-id="2ab91-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="2ab91-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ab91-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="2ab91-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="2ab91-123">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="2ab91-124">この要素の XPath 式は次のとおりです。/finditem。</span><span class="sxs-lookup"><span data-stu-id="2ab91-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ab91-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2ab91-125">Text value</span></span>

<span data-ttu-id="2ab91-126">**QueryString**要素のテキスト値は、[高度なクエリ構文 (aqs)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx)のサブセットを使用して作成されたメールボックスクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="2ab91-127">クエリ文字列に対してサポートされている構文オプションについては、「備考」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ab91-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ab91-128">注釈</span><span class="sxs-lookup"><span data-stu-id="2ab91-128">Remarks</span></span>

<span data-ttu-id="2ab91-129">Exchange Server 2010 では、この要素は XML スキーマ文字列型です。</span><span class="sxs-lookup"><span data-stu-id="2ab91-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="2ab91-130">Exchange Online を含む exchange Server 2013 以降のバージョンの Exchange では、この要素の型は**Querystringtype**になります。</span><span class="sxs-lookup"><span data-stu-id="2ab91-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="2ab91-131">この変更により、既存のクライアントは3つの新しいオプション属性が追加されるため、この変更による影響はありません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="2ab91-132">**QueryString**要素には、EWS の制限の使用は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="2ab91-133">EWS の AQS は、word フェーズの制限、日付範囲の制限、およびメッセージの種類の制限の3種類の制限をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="2ab91-134">次の表は、制限の種類ごとにサポートされている検索プロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="2ab91-135">**Word フェーズの制限**</span><span class="sxs-lookup"><span data-stu-id="2ab91-135">**Word phase restriction**</span></span>

|<span data-ttu-id="2ab91-136">**Property**</span><span class="sxs-lookup"><span data-stu-id="2ab91-136">**Property**</span></span>|<span data-ttu-id="2ab91-137">**例**</span><span class="sxs-lookup"><span data-stu-id="2ab91-137">**Example**</span></span>|<span data-ttu-id="2ab91-138">**Function**</span><span class="sxs-lookup"><span data-stu-id="2ab91-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ab91-139">from</span><span class="sxs-lookup"><span data-stu-id="2ab91-139">from</span></span>  <br/> |<span data-ttu-id="2ab91-140">From: 中</span><span class="sxs-lookup"><span data-stu-id="2ab91-140">From:Dean</span></span>  <br/> <span data-ttu-id="2ab91-141">From: "Halstead"</span><span class="sxs-lookup"><span data-stu-id="2ab91-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="2ab91-142">他の方法で送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="2ab91-143">Halstead から送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="2ab91-144">送信者は正確に "Halstead" である必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ab91-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="2ab91-145">to</span><span class="sxs-lookup"><span data-stu-id="2ab91-145">to</span></span>  <br/> |<span data-ttu-id="2ab91-146">宛先: "(中)"</span><span class="sxs-lookup"><span data-stu-id="2ab91-146">To:Dean</span></span>  <br/> |<span data-ttu-id="2ab91-147">送信されたアイテムは、"元にはなりません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="2ab91-148">cc</span><span class="sxs-lookup"><span data-stu-id="2ab91-148">cc</span></span>  <br/> |<span data-ttu-id="2ab91-149">Cc: (中)</span><span class="sxs-lookup"><span data-stu-id="2ab91-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="2ab91-150">[Cc] 行には、が中にあるアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="2ab91-151">bcc</span><span class="sxs-lookup"><span data-stu-id="2ab91-151">bcc</span></span>  <br/> |<span data-ttu-id="2ab91-152">Bcc: (中)</span><span class="sxs-lookup"><span data-stu-id="2ab91-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="2ab91-153">Bcc 行には、[(中)] というアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="2ab91-154">参加者</span><span class="sxs-lookup"><span data-stu-id="2ab91-154">Participants</span></span>  <br/> |<span data-ttu-id="2ab91-155">参加者: その他</span><span class="sxs-lookup"><span data-stu-id="2ab91-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="2ab91-156">[宛先]、[Cc]、または [Bcc] フィールドに入力されているアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="2ab91-157">件名</span><span class="sxs-lookup"><span data-stu-id="2ab91-157">Subject</span></span>  <br/> |<span data-ttu-id="2ab91-158">Subject: product</span><span class="sxs-lookup"><span data-stu-id="2ab91-158">Subject:product</span></span>  <br/> <span data-ttu-id="2ab91-159">件名: (製品開発)</span><span class="sxs-lookup"><span data-stu-id="2ab91-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="2ab91-160">Subject: "製品開発"</span><span class="sxs-lookup"><span data-stu-id="2ab91-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="2ab91-161">件名に製品が含まれるアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="2ab91-162">件名に製品と開発があるアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="2ab91-163">本文</span><span class="sxs-lookup"><span data-stu-id="2ab91-163">Body</span></span>  <br/> <span data-ttu-id="2ab91-164">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="2ab91-164">Content</span></span>  <br/> |<span data-ttu-id="2ab91-165">本文: 進行状況</span><span class="sxs-lookup"><span data-stu-id="2ab91-165">Body:progress</span></span>  <br/> <span data-ttu-id="2ab91-166">コンテンツ: 進行状況</span><span class="sxs-lookup"><span data-stu-id="2ab91-166">Content:progress</span></span>  <br/> |<span data-ttu-id="2ab91-167">本文の進行状況があるアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="2ab91-168">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="2ab91-168">Attachment</span></span>  <br/> |<span data-ttu-id="2ab91-169">添付ファイル: レポート</span><span class="sxs-lookup"><span data-stu-id="2ab91-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="2ab91-170">添付ファイルのファイル名またはファイル本文にレポートを含むアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="2ab91-171">(プロパティが指定されていない)</span><span class="sxs-lookup"><span data-stu-id="2ab91-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="2ab91-172">製品開発</span><span class="sxs-lookup"><span data-stu-id="2ab91-172">Product Development</span></span>  <br/> |<span data-ttu-id="2ab91-173">すべての word フェーズプロパティで、製品と開発の両方を含むアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="2ab91-174">Word フェーズ制限 match は、常に大文字と小文字を区別しません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="2ab91-175">Word フェーズ制限では、次の2つの一致する種類がサポートされます。プレフィックス一致または完全一致。</span><span class="sxs-lookup"><span data-stu-id="2ab91-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="2ab91-176">プレフィックス一致は、既定の一致動作です。</span><span class="sxs-lookup"><span data-stu-id="2ab91-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="2ab91-177">完全一致する場合は、二重引用符を使用します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="2ab91-178">たとえば、subject: "product" は "product" に一致しますが、件名では "production" ではありません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="2ab91-179">二重引用符で囲まれた複数の単語は、両方の単語のフェーズと順序を制限します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="2ab91-180">たとえば、"win product" は ' win product ' にのみ一致し、' win95 product ' または ' win of product ' とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="2ab91-181">アスタリスク () を使用すると \* 、順序制限付きのプレフィックス一致を定義できます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="2ab91-182">たとえば、"win product" は、「 \* win95 product」、「windows production line」と一致しますが、「windows new product」や「win of product」とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="2ab91-183">またはドメインから送信されたすべてのメッセージを検索できます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="2ab91-184">たとえば、from: "@hotmail" は、hotmail.com から送信されたすべてのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="2ab91-185">次の表では、日付範囲制限について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="2ab91-186">**日付範囲の制限**</span><span class="sxs-lookup"><span data-stu-id="2ab91-186">**Date range restriction**</span></span>

|<span data-ttu-id="2ab91-187">**Property**</span><span class="sxs-lookup"><span data-stu-id="2ab91-187">**Property**</span></span>|<span data-ttu-id="2ab91-188">**例**</span><span class="sxs-lookup"><span data-stu-id="2ab91-188">**Example**</span></span>|<span data-ttu-id="2ab91-189">**Function**</span><span class="sxs-lookup"><span data-stu-id="2ab91-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ab91-190">送信日時</span><span class="sxs-lookup"><span data-stu-id="2ab91-190">Sent</span></span>  <br/> |<span data-ttu-id="2ab91-191">送信日時: 先週</span><span class="sxs-lookup"><span data-stu-id="2ab91-191">Sent:last week</span></span>  <br/> <span data-ttu-id="2ab91-192">送信日時:01/01/2001</span><span class="sxs-lookup"><span data-stu-id="2ab91-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="2ab91-193">送信日時:01/01/2001. 01/15/2001</span><span class="sxs-lookup"><span data-stu-id="2ab91-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="2ab91-194">先週送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="2ab91-195">2001年1月1日に送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="2ab91-196">2001年1月1日から年1月 2001 15 日の間に送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="2ab91-197">受信済み</span><span class="sxs-lookup"><span data-stu-id="2ab91-197">Received</span></span>  <br/> |<span data-ttu-id="2ab91-198">受信: 今日</span><span class="sxs-lookup"><span data-stu-id="2ab91-198">Received:today</span></span>  <br/> <span data-ttu-id="2ab91-199">受信日時:01/01/2001</span><span class="sxs-lookup"><span data-stu-id="2ab91-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="2ab91-200">今日受信したアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-200">Search items received today.</span></span>  <br/> <span data-ttu-id="2ab91-201">2001年1月1日に受信したアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="2ab91-202">2つのドット (..) は範囲演算子です。</span><span class="sxs-lookup"><span data-stu-id="2ab91-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="2ab91-203">開始日と終了日を使用して範囲を定義することができます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="2ab91-204">日付を指定するには、相対日付を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="2ab91-205">次の相対日付がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="2ab91-206">相対日付: 今日、明日、昨日</span><span class="sxs-lookup"><span data-stu-id="2ab91-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="2ab91-207">複数の単語の相対日付: 今週、来月、先週、過去の月、または翌年</span><span class="sxs-lookup"><span data-stu-id="2ab91-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="2ab91-208">曜日: 日曜日、月曜日、火曜日、水曜日、木曜日、金曜日、土曜日</span><span class="sxs-lookup"><span data-stu-id="2ab91-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="2ab91-209">1月、2月、3月、4月、5月、6月、7月、5月、7月、7月、11月、10月、11月、12月</span><span class="sxs-lookup"><span data-stu-id="2ab91-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="2ab91-210">次の表では、メッセージの種類の制限について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="2ab91-211">**メッセージの種類の制限**</span><span class="sxs-lookup"><span data-stu-id="2ab91-211">**Message type restriction**</span></span>

|<span data-ttu-id="2ab91-212">**Property**</span><span class="sxs-lookup"><span data-stu-id="2ab91-212">**Property**</span></span>|<span data-ttu-id="2ab91-213">**例**</span><span class="sxs-lookup"><span data-stu-id="2ab91-213">**Example**</span></span>|<span data-ttu-id="2ab91-214">**Function**</span><span class="sxs-lookup"><span data-stu-id="2ab91-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ab91-215">Kind</span><span class="sxs-lookup"><span data-stu-id="2ab91-215">Kind</span></span>  <br/> |<span data-ttu-id="2ab91-216">種類: タスク</span><span class="sxs-lookup"><span data-stu-id="2ab91-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="2ab91-217">すべてのタスクアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="2ab91-218">EWS の AQS は、 **Kind**プロパティを使用してメッセージの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="2ab91-219">Kind プロパティは、次のアイテムの種類で使用できます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="2ab91-220">email</span><span class="sxs-lookup"><span data-stu-id="2ab91-220">email</span></span>
    
- <span data-ttu-id="2ab91-221">meetings</span><span class="sxs-lookup"><span data-stu-id="2ab91-221">meetings</span></span>
    
- <span data-ttu-id="2ab91-222">tasks</span><span class="sxs-lookup"><span data-stu-id="2ab91-222">tasks</span></span>
    
- <span data-ttu-id="2ab91-223">notes</span><span class="sxs-lookup"><span data-stu-id="2ab91-223">notes</span></span>
    
- <span data-ttu-id="2ab91-224">docs</span><span class="sxs-lookup"><span data-stu-id="2ab91-224">docs</span></span>
    
- <span data-ttu-id="2ab91-225">journals</span><span class="sxs-lookup"><span data-stu-id="2ab91-225">journals</span></span>
    
- <span data-ttu-id="2ab91-226">連絡先</span><span class="sxs-lookup"><span data-stu-id="2ab91-226">contacts</span></span>
    
- <span data-ttu-id="2ab91-227">im</span><span class="sxs-lookup"><span data-stu-id="2ab91-227">im</span></span>
    
<span data-ttu-id="2ab91-228">次の表では、グループ化論理コネクタについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="2ab91-229">**論理コネクタのグループ化**</span><span class="sxs-lookup"><span data-stu-id="2ab91-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="2ab91-230">**Connector**</span><span class="sxs-lookup"><span data-stu-id="2ab91-230">**Connector**</span></span>|<span data-ttu-id="2ab91-231">**例**</span><span class="sxs-lookup"><span data-stu-id="2ab91-231">**Example**</span></span>|<span data-ttu-id="2ab91-232">**Function**</span><span class="sxs-lookup"><span data-stu-id="2ab91-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ab91-233">AND</span><span class="sxs-lookup"><span data-stu-id="2ab91-233">AND</span></span>  <br/> |<span data-ttu-id="2ab91-234">件名: 製品と件名: 開発</span><span class="sxs-lookup"><span data-stu-id="2ab91-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="2ab91-235">Subject: (製品と開発)</span><span class="sxs-lookup"><span data-stu-id="2ab91-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="2ab91-236">件名: (製品開発)</span><span class="sxs-lookup"><span data-stu-id="2ab91-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="2ab91-237">件名に製品と開発の両方を含むアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="2ab91-238">OR</span><span class="sxs-lookup"><span data-stu-id="2ab91-238">OR</span></span>  <br/> |<span data-ttu-id="2ab91-239">本文: プロジェクトまたは本文: 提案</span><span class="sxs-lookup"><span data-stu-id="2ab91-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="2ab91-240">本文: (プロジェクトまたは提案)</span><span class="sxs-lookup"><span data-stu-id="2ab91-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="2ab91-241">本文で製品または開発のいずれかを使用してアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="2ab91-242">NOT</span><span class="sxs-lookup"><span data-stu-id="2ab91-242">NOT</span></span>  <br/> |<span data-ttu-id="2ab91-243">本文以外: 提案</span><span class="sxs-lookup"><span data-stu-id="2ab91-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="2ab91-244">本文: (提案されていません)</span><span class="sxs-lookup"><span data-stu-id="2ab91-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="2ab91-245">本文に提案のないメッセージを検索します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="2ab91-246">は常に既定のコネクタです。</span><span class="sxs-lookup"><span data-stu-id="2ab91-246">AND is always the default connector.</span></span> <span data-ttu-id="2ab91-247">たとえば、subject: project および body: 提案は、件名: プロジェクト本文: 提案と同じです。</span><span class="sxs-lookup"><span data-stu-id="2ab91-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="2ab91-248">論理コネクタは大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="2ab91-249">たとえば、body: (プロジェクトまたは提案) では、' project '、' または '、' ' 企画 ' ' の代わりに ' project '、' または '、' 提案 ' のメッセージが検索されます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="2ab91-250">正符号 (+) は、およびに相当します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="2ab91-251">ハイフン記号 (-) は、NOT と同じです。</span><span class="sxs-lookup"><span data-stu-id="2ab91-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="2ab91-252">たとえば、body: (プロジェクト-提案) は ' project ' でメッセージを検索しますが、本文には ' 提案 ' は含まれません。</span><span class="sxs-lookup"><span data-stu-id="2ab91-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="2ab91-253">クエリ文字列には、検索用のインデックスを持たないプロパティも含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="2ab91-254">クエリ文字列にインデックスなしのプロパティが含まれている場合、検索はインデックス付きプロパティに対して Exchange 検索を実行し、インデックスが設定されていないプロパティでストア検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="2ab91-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="2ab91-255">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="2ab91-256">例</span><span class="sxs-lookup"><span data-stu-id="2ab91-256">Example</span></span>

<span data-ttu-id="2ab91-257">次の例は、件名の自動検出を使用して受信トレイ内のメッセージを検索する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2ab91-258">次の例は、要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2ab91-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a><span data-ttu-id="2ab91-259">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2ab91-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ab91-260">Namespace</span><span class="sxs-lookup"><span data-stu-id="2ab91-260">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ab91-261">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ab91-261">Schema name</span></span>  <br/> |<span data-ttu-id="2ab91-262">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2ab91-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2ab91-263">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ab91-263">Validation file</span></span>  <br/> |<span data-ttu-id="2ab91-264">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2ab91-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ab91-265">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ab91-265">Can be empty</span></span>  <br/> |<span data-ttu-id="2ab91-266">正しくない</span><span class="sxs-lookup"><span data-stu-id="2ab91-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ab91-267">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ab91-267">See also</span></span>



[<span data-ttu-id="2ab91-268">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="2ab91-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="2ab91-269">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="2ab91-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="2ab91-270">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2ab91-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

