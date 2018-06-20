---
title: クエリ文字列 (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: クエリ文字列要素には、ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832943"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="73b14-103">クエリ文字列 (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="73b14-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="73b14-104">**クエリ文字列**要素には、ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="73b14-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="73b14-105">**QueryStringType**</span><span class="sxs-lookup"><span data-stu-id="73b14-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73b14-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="73b14-106">Attributes and elements</span></span>

<span data-ttu-id="73b14-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73b14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73b14-108">属性</span><span class="sxs-lookup"><span data-stu-id="73b14-108">Attributes</span></span>

|<span data-ttu-id="73b14-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="73b14-109">**Attribute**</span></span>|<span data-ttu-id="73b14-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="73b14-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73b14-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="73b14-111">ResetCache</span></span>  <br/> |<span data-ttu-id="73b14-112">キャッシュをリセットする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="73b14-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="73b14-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="73b14-114">削除済みアイテムが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="73b14-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="73b14-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="73b14-116">強調表示されている用語が返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="73b14-117">子要素</span><span class="sxs-lookup"><span data-stu-id="73b14-117">Child elements</span></span>

<span data-ttu-id="73b14-118">なし。</span><span class="sxs-lookup"><span data-stu-id="73b14-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73b14-119">親要素</span><span class="sxs-lookup"><span data-stu-id="73b14-119">Parent elements</span></span>

|<span data-ttu-id="73b14-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="73b14-120">**Element**</span></span>|<span data-ttu-id="73b14-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="73b14-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73b14-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="73b14-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="73b14-123">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="73b14-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="73b14-124">次は、この要素の XPath 式:/FindItem。</span><span class="sxs-lookup"><span data-stu-id="73b14-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73b14-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="73b14-125">Text value</span></span>

<span data-ttu-id="73b14-126">**クエリ文字列**要素のテキスト値は、[高度なクエリ構文 (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx)のサブセットを使用して作成されるメールボックスのクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="73b14-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="73b14-127">クエリ文字列の構文がサポートされているオプションの詳細については「解説」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="73b14-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73b14-128">備考</span><span class="sxs-lookup"><span data-stu-id="73b14-128">Remarks</span></span>

<span data-ttu-id="73b14-129">Exchange Server 2010 では、この要素は、XML スキーマの文字列の種類をします。</span><span class="sxs-lookup"><span data-stu-id="73b14-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="73b14-130">バージョンの Exchange が Exchange Server 2013 で始まる、 **QueryStringType**は、Exchange オンライン、この要素の型を含みます。</span><span class="sxs-lookup"><span data-stu-id="73b14-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="73b14-131">3 つの新しいオプション属性を追加するため、この変更は既存のクライアントを中断しません。</span><span class="sxs-lookup"><span data-stu-id="73b14-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="73b14-132">**クエリ文字列**要素は、EWS の制限の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="73b14-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="73b14-133">EWS で AQS の 3 種類の制限をサポートしています: word のフェーズの制限、日付範囲の制限、およびメッセージの種類の制限です。</span><span class="sxs-lookup"><span data-stu-id="73b14-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="73b14-134">次の表は、制限の種類ごとにサポートされている検索プロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="73b14-135">**Word フェーズの制限**</span><span class="sxs-lookup"><span data-stu-id="73b14-135">**Word phase restriction**</span></span>

|<span data-ttu-id="73b14-136">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="73b14-136">**Property**</span></span>|<span data-ttu-id="73b14-137">**例**</span><span class="sxs-lookup"><span data-stu-id="73b14-137">**Example**</span></span>|<span data-ttu-id="73b14-138">**�֐�**</span><span class="sxs-lookup"><span data-stu-id="73b14-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73b14-139">from</span><span class="sxs-lookup"><span data-stu-id="73b14-139">from</span></span>  <br/> |<span data-ttu-id="73b14-140">: 学部長</span><span class="sxs-lookup"><span data-stu-id="73b14-140">From:Dean</span></span>  <br/> <span data-ttu-id="73b14-141">:「Dean ハルステッド」</span><span class="sxs-lookup"><span data-stu-id="73b14-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="73b14-142">Dean から送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="73b14-143">Dean ハルステッドから送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="73b14-144">送信者は、正確に「Dean ハルステッド」である必要があります。</span><span class="sxs-lookup"><span data-stu-id="73b14-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="73b14-145">の行を</span><span class="sxs-lookup"><span data-stu-id="73b14-145">to</span></span>  <br/> |<span data-ttu-id="73b14-146">: 学部長</span><span class="sxs-lookup"><span data-stu-id="73b14-146">To:Dean</span></span>  <br/> |<span data-ttu-id="73b14-147">Dean に送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="73b14-148">cc</span><span class="sxs-lookup"><span data-stu-id="73b14-148">cc</span></span>  <br/> |<span data-ttu-id="73b14-149">Cc:Dean</span><span class="sxs-lookup"><span data-stu-id="73b14-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="73b14-150">[Cc] 行の Dean でアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="73b14-151">bcc</span><span class="sxs-lookup"><span data-stu-id="73b14-151">bcc</span></span>  <br/> |<span data-ttu-id="73b14-152">Bcc:Dean</span><span class="sxs-lookup"><span data-stu-id="73b14-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="73b14-153">[Bcc] 行の Dean でアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="73b14-154">Participants</span><span class="sxs-lookup"><span data-stu-id="73b14-154">Participants</span></span>  <br/> |<span data-ttu-id="73b14-155">参加者: 学部長</span><span class="sxs-lookup"><span data-stu-id="73b14-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="73b14-156">フィールドを Dean でアイテムを [宛先] ボックス、[cc]、または [bcc] に検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="73b14-157">件名</span><span class="sxs-lookup"><span data-stu-id="73b14-157">Subject</span></span>  <br/> |<span data-ttu-id="73b14-158">件名: 商品</span><span class="sxs-lookup"><span data-stu-id="73b14-158">Subject:product</span></span>  <br/> <span data-ttu-id="73b14-159">件名:(product development)</span><span class="sxs-lookup"><span data-stu-id="73b14-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="73b14-160">件名:「製品開発」</span><span class="sxs-lookup"><span data-stu-id="73b14-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="73b14-161">件名に製品を持つアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="73b14-162">製品と開発の主題にアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="73b14-163">本文</span><span class="sxs-lookup"><span data-stu-id="73b14-163">Body</span></span>  <br/> <span data-ttu-id="73b14-164">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="73b14-164">Content</span></span>  <br/> |<span data-ttu-id="73b14-165">本文: 進行状況</span><span class="sxs-lookup"><span data-stu-id="73b14-165">Body:progress</span></span>  <br/> <span data-ttu-id="73b14-166">: 進行中のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="73b14-166">Content:progress</span></span>  <br/> |<span data-ttu-id="73b14-167">本文の中でアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="73b14-168">Attachment</span><span class="sxs-lookup"><span data-stu-id="73b14-168">Attachment</span></span>  <br/> |<span data-ttu-id="73b14-169">添付ファイル: レポート</span><span class="sxs-lookup"><span data-stu-id="73b14-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="73b14-170">添付ファイルのファイル名またはファイルの本文にレポート アイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="73b14-171">(プロパティが指定されていません)</span><span class="sxs-lookup"><span data-stu-id="73b14-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="73b14-172">製品の開発</span><span class="sxs-lookup"><span data-stu-id="73b14-172">Product Development</span></span>  <br/> |<span data-ttu-id="73b14-173">製品と開発の両方で word のすべてのフェーズ プロパティを含む項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="73b14-174">一致する単語の段階の制限は、常に大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="73b14-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="73b14-175">Word フェーズの制限は、2 つの一致の種類をサポートしています: プレフィックスの一致または完全に一致します。</span><span class="sxs-lookup"><span data-stu-id="73b14-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="73b14-176">プレフィックスの一致は、マッチの既定の動作です。</span><span class="sxs-lookup"><span data-stu-id="73b14-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="73b14-177">正確に一致する場合は、二重引用符を使用します。</span><span class="sxs-lookup"><span data-stu-id="73b14-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="73b14-178">たとえば、件名:「製品」は、'製品' がない '' 内での生産、件名と一致します。</span><span class="sxs-lookup"><span data-stu-id="73b14-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="73b14-179">複数の単語を二重引用符では、word のフェーズとその順序の両方を制限します。</span><span class="sxs-lookup"><span data-stu-id="73b14-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="73b14-180">たとえば"win 製品"は、唯一の 'win 製品'、'win95 製品ではない' または '勝利の製品' と一致します。</span><span class="sxs-lookup"><span data-stu-id="73b14-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="73b14-181">アスタリスクを使用することができます (\*) 順で制限されているプレフィックスの一致を定義します。</span><span class="sxs-lookup"><span data-stu-id="73b14-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="73b14-182">たとえば、「win 製品」\* 'win95 製品'、' windows 生産ライン ' がない 'windows の新製品' または '勝利の製品' と一致します。</span><span class="sxs-lookup"><span data-stu-id="73b14-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="73b14-183">またはドメインから送信されたすべてのメッセージを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="73b14-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="73b14-184">たとえば、from:"@hotmail.com"は、hotmail.com から送信されたすべてのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="73b14-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="73b14-185">次の表では、日付の範囲の制限について説明します。</span><span class="sxs-lookup"><span data-stu-id="73b14-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="73b14-186">**日付範囲の制限**</span><span class="sxs-lookup"><span data-stu-id="73b14-186">**Date range restriction**</span></span>

|<span data-ttu-id="73b14-187">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="73b14-187">**Property**</span></span>|<span data-ttu-id="73b14-188">**例**</span><span class="sxs-lookup"><span data-stu-id="73b14-188">**Example**</span></span>|<span data-ttu-id="73b14-189">**�֐�**</span><span class="sxs-lookup"><span data-stu-id="73b14-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73b14-190">Sent</span><span class="sxs-lookup"><span data-stu-id="73b14-190">Sent</span></span>  <br/> |<span data-ttu-id="73b14-191">送信: 最後の週</span><span class="sxs-lookup"><span data-stu-id="73b14-191">Sent:last week</span></span>  <br/> <span data-ttu-id="73b14-192">送信: 2001 年 01 月 01 日</span><span class="sxs-lookup"><span data-stu-id="73b14-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="73b14-193">Sent:01/01/2001..01/15/2001</span><span class="sxs-lookup"><span data-stu-id="73b14-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="73b14-194">検索項目は、最後の週を送信します。</span><span class="sxs-lookup"><span data-stu-id="73b14-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="73b14-195">2001 年 1 月 1 日に送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="73b14-196">2001 年 1 月 1 日と 2001 年 1 月 15 日の間で送信されたアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="73b14-197">Received</span><span class="sxs-lookup"><span data-stu-id="73b14-197">Received</span></span>  <br/> |<span data-ttu-id="73b14-198">受信しました: 今日</span><span class="sxs-lookup"><span data-stu-id="73b14-198">Received:today</span></span>  <br/> <span data-ttu-id="73b14-199">受信: 2001 年 01 月 01 日</span><span class="sxs-lookup"><span data-stu-id="73b14-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="73b14-200">今日受信したアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-200">Search items received today.</span></span>  <br/> <span data-ttu-id="73b14-201">2001 年 1 月 1 日に受信したアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="73b14-202">2 つのドット (.) は、範囲演算子です。</span><span class="sxs-lookup"><span data-stu-id="73b14-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="73b14-203">開始日と終了日の範囲を定義して使用できます。</span><span class="sxs-lookup"><span data-stu-id="73b14-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="73b14-204">日付を指定するには、相対的な日付を使用できます。</span><span class="sxs-lookup"><span data-stu-id="73b14-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="73b14-205">次の相対日付がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="73b14-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="73b14-206">相対日時: 今日、明日、昨日</span><span class="sxs-lookup"><span data-stu-id="73b14-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="73b14-207">語の相対日付: 今週、来月、先週、過去の月、または今後 1 年以内</span><span class="sxs-lookup"><span data-stu-id="73b14-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="73b14-208">曜日: 日曜日、月曜日、火曜日、水曜日、木曜日、金曜日、土曜日</span><span class="sxs-lookup"><span data-stu-id="73b14-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="73b14-209">年 1 月、2 月、3 月 4 月、可能性があります、6 月、7 月、8 月、9 月、10 月、11 月、年 12 月</span><span class="sxs-lookup"><span data-stu-id="73b14-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="73b14-210">次の表では、メッセージの種類の制限について説明します。</span><span class="sxs-lookup"><span data-stu-id="73b14-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="73b14-211">**メッセージの種類の制限**</span><span class="sxs-lookup"><span data-stu-id="73b14-211">**Message type restriction**</span></span>

|<span data-ttu-id="73b14-212">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="73b14-212">**Property**</span></span>|<span data-ttu-id="73b14-213">**例**</span><span class="sxs-lookup"><span data-stu-id="73b14-213">**Example**</span></span>|<span data-ttu-id="73b14-214">**�֐�**</span><span class="sxs-lookup"><span data-stu-id="73b14-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73b14-215">種類</span><span class="sxs-lookup"><span data-stu-id="73b14-215">Kind</span></span>  <br/> |<span data-ttu-id="73b14-216">タスクの種類:</span><span class="sxs-lookup"><span data-stu-id="73b14-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="73b14-217">すべての作業項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="73b14-218">AQS EWS では、メッセージの種類を指定するのには**Kind**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="73b14-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="73b14-219">Kind プロパティは、次の項目の種類で使用できます。</span><span class="sxs-lookup"><span data-stu-id="73b14-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="73b14-220">email</span><span class="sxs-lookup"><span data-stu-id="73b14-220">email</span></span>
    
- <span data-ttu-id="73b14-221">会議</span><span class="sxs-lookup"><span data-stu-id="73b14-221">meetings</span></span>
    
- <span data-ttu-id="73b14-222">tasks</span><span class="sxs-lookup"><span data-stu-id="73b14-222">tasks</span></span>
    
- <span data-ttu-id="73b14-223">notes</span><span class="sxs-lookup"><span data-stu-id="73b14-223">notes</span></span>
    
- <span data-ttu-id="73b14-224">docs</span><span class="sxs-lookup"><span data-stu-id="73b14-224">docs</span></span>
    
- <span data-ttu-id="73b14-225">journals</span><span class="sxs-lookup"><span data-stu-id="73b14-225">journals</span></span>
    
- <span data-ttu-id="73b14-226">contacts</span><span class="sxs-lookup"><span data-stu-id="73b14-226">contacts</span></span>
    
- <span data-ttu-id="73b14-227">im</span><span class="sxs-lookup"><span data-stu-id="73b14-227">im</span></span>
    
<span data-ttu-id="73b14-228">論理コネクタをグループ化を次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="73b14-229">**論理コネクタをグループ化**</span><span class="sxs-lookup"><span data-stu-id="73b14-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="73b14-230">**コネクタ**</span><span class="sxs-lookup"><span data-stu-id="73b14-230">**Connector**</span></span>|<span data-ttu-id="73b14-231">**例**</span><span class="sxs-lookup"><span data-stu-id="73b14-231">**Example**</span></span>|<span data-ttu-id="73b14-232">**�֐�**</span><span class="sxs-lookup"><span data-stu-id="73b14-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73b14-233">AND</span><span class="sxs-lookup"><span data-stu-id="73b14-233">AND</span></span>  <br/> |<span data-ttu-id="73b14-234">件名: 製品および件名: 開発</span><span class="sxs-lookup"><span data-stu-id="73b14-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="73b14-235">件名:(product AND development)</span><span class="sxs-lookup"><span data-stu-id="73b14-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="73b14-236">件名:(product development)</span><span class="sxs-lookup"><span data-stu-id="73b14-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="73b14-237">件名に製品と開発の両方を持つアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="73b14-238">OR</span><span class="sxs-lookup"><span data-stu-id="73b14-238">OR</span></span>  <br/> |<span data-ttu-id="73b14-239">本文: プロジェクトまたは本文: 提案</span><span class="sxs-lookup"><span data-stu-id="73b14-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="73b14-240">本文:(project OR proposal)</span><span class="sxs-lookup"><span data-stu-id="73b14-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="73b14-241">本文の製品や開発のいずれかの項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="73b14-242">NOT</span><span class="sxs-lookup"><span data-stu-id="73b14-242">NOT</span></span>  <br/> |<span data-ttu-id="73b14-243">本文: 提案のないです。</span><span class="sxs-lookup"><span data-stu-id="73b14-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="73b14-244">本文:(NOT proposal)</span><span class="sxs-lookup"><span data-stu-id="73b14-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="73b14-245">提案なしのメッセージ本文の検索をします。</span><span class="sxs-lookup"><span data-stu-id="73b14-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="73b14-246">デフォルトのコネクタは、常にします。</span><span class="sxs-lookup"><span data-stu-id="73b14-246">AND is always the default connector.</span></span> <span data-ttu-id="73b14-247">など: プロジェクトの件名と本文: 提案は、プロジェクトの件名: 本文: 提案と同じ。</span><span class="sxs-lookup"><span data-stu-id="73b14-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="73b14-248">論理コネクタでは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="73b14-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="73b14-249">本文の例では、:(project Or proposal) 'プロジェクト'、メッセージの検索 'または' と '' 'プロジェクト' または '提案' ではなく本文にします。</span><span class="sxs-lookup"><span data-stu-id="73b14-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="73b14-250">プラス記号 (+) のと同じです。</span><span class="sxs-lookup"><span data-stu-id="73b14-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="73b14-251">ハイフン記号 (-) は、NOT と同じです。</span><span class="sxs-lookup"><span data-stu-id="73b14-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="73b14-252">本文の例では、:(project-proposal)、本文に 'プロジェクト'、'提案' なしのメッセージを検索します。</span><span class="sxs-lookup"><span data-stu-id="73b14-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="73b14-253">クエリ文字列は、検索用インデックス付けされていないプロパティを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="73b14-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="73b14-254">クエリ文字列にインデックス付けされていないプロパティが含まれている場合、検索は、インデックス付きのプロパティと、ストア、インデックス付けされていないプロパティの検索に Exchange 検索を実行する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="73b14-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="73b14-255">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="73b14-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="73b14-256">例</span><span class="sxs-lookup"><span data-stu-id="73b14-256">Example</span></span>

<span data-ttu-id="73b14-257">件名に自動検出と、受信トレイでメッセージを検索するための要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="73b14-258">要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73b14-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="73b14-259">要素情報</span><span class="sxs-lookup"><span data-stu-id="73b14-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73b14-260">名前空間</span><span class="sxs-lookup"><span data-stu-id="73b14-260">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73b14-261">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73b14-261">Schema name</span></span>  <br/> |<span data-ttu-id="73b14-262">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="73b14-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73b14-263">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73b14-263">Validation file</span></span>  <br/> |<span data-ttu-id="73b14-264">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73b14-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73b14-265">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="73b14-265">Can be empty</span></span>  <br/> |<span data-ttu-id="73b14-266">False</span><span class="sxs-lookup"><span data-stu-id="73b14-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73b14-267">関連項目</span><span class="sxs-lookup"><span data-stu-id="73b14-267">See also</span></span>



<span data-ttu-id="73b14-268">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="73b14-268">[FindItem operation](finditem-operation.md)</span></span>
  
<span data-ttu-id="73b14-269">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="73b14-269">[FindConversation operation](findconversation-operation.md)</span></span>


- [<span data-ttu-id="73b14-270">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="73b14-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

