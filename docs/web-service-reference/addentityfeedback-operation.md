---
title: AddEntityFeedback 操作
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: AddEntityFeedback 操作は、サーバー側の問題に対応するエラー情報を返します。
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458440"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="41a93-103">AddEntityFeedback 操作</span><span class="sxs-lookup"><span data-stu-id="41a93-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="41a93-104">**Addentityfeedback**操作は、サーバー側の問題に対応するエラー情報を返します。</span><span class="sxs-lookup"><span data-stu-id="41a93-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="41a93-105">この操作では、ログに記録されるイベントの種類に依存します。</span><span class="sxs-lookup"><span data-stu-id="41a93-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="41a93-106">最も重要なイベントの1つは、選択されているエンティティに対応する**Entityadded が追加**されたことです。</span><span class="sxs-lookup"><span data-stu-id="41a93-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="41a93-107">この操作はバッチであるため、1回の要求でエントリのバッチをログに記録するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="41a93-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="41a93-108">FindPeople 要求の例</span><span class="sxs-lookup"><span data-stu-id="41a93-108">FindPeople request examples</span></span>

<span data-ttu-id="41a93-109">**Addentityfeedback**操作は、クライアントがサービスによって返されるエンティティとの対話の詳細をログに記録する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="41a93-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="41a93-110">これは、クライアントごとに、シーンの背後で関連性を向上させるための信号として使用できます。</span><span class="sxs-lookup"><span data-stu-id="41a93-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="41a93-111">例: クライアントは、この操作を使用して、 **findpeople**から返された人物エンティティについてのフィードバックを提供できます。</span><span class="sxs-lookup"><span data-stu-id="41a93-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="41a93-112">要求 SOAP 本文のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="41a93-112">The request SOAP body contents</span></span>

<span data-ttu-id="41a93-113">Soap 要求には、1つの要素の**エンティティフィードのバックエントリ**が含まれています。</span><span class="sxs-lookup"><span data-stu-id="41a93-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="41a93-114">これには、 **Entityフィードバック entry**オブジェクトの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="41a93-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="41a93-115">配列内の各エントリには、次の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="41a93-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="41a93-116">**要求のパラメータ**</span><span class="sxs-lookup"><span data-stu-id="41a93-116">**Request Parameters**</span></span>|<span data-ttu-id="41a93-117">**必須**</span><span class="sxs-lookup"><span data-stu-id="41a93-117">**Required**</span></span>|<span data-ttu-id="41a93-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="41a93-118">**Description**</span></span>|<span data-ttu-id="41a93-119">**型**</span><span class="sxs-lookup"><span data-stu-id="41a93-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="41a93-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="41a93-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="41a93-121">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-121">Yes</span></span>  <br/> |<span data-ttu-id="41a93-122">クライアント側でイベントが発生した UTC 時間。</span><span class="sxs-lookup"><span data-stu-id="41a93-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="41a93-123">DateTime
</span><span class="sxs-lookup"><span data-stu-id="41a93-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="41a93-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="41a93-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="41a93-125">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-125">Yes</span></span>  <br/> |<span data-ttu-id="41a93-126">クライアント側でイベントが発生したローカル時刻。</span><span class="sxs-lookup"><span data-stu-id="41a93-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="41a93-127">DateTime
</span><span class="sxs-lookup"><span data-stu-id="41a93-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="41a93-128">**ClientId**</span><span class="sxs-lookup"><span data-stu-id="41a93-128">**ClientId**</span></span> <br/> |<span data-ttu-id="41a93-129">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-129">Yes</span></span>  <br/> |<span data-ttu-id="41a93-130">クライアントの種類 (Outlook、OWA など)。</span><span class="sxs-lookup"><span data-stu-id="41a93-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="41a93-131">ClientIDType 列挙型</span><span class="sxs-lookup"><span data-stu-id="41a93-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="41a93-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="41a93-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="41a93-133">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-133">Yes</span></span>  <br/> |<span data-ttu-id="41a93-134">セッション ID を識別する GUID。</span><span class="sxs-lookup"><span data-stu-id="41a93-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="41a93-135">クライアントで生成されます。</span><span class="sxs-lookup"><span data-stu-id="41a93-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="41a93-136">GUID</span><span class="sxs-lookup"><span data-stu-id="41a93-136">GUID</span></span>  <br/> |
|<span data-ttu-id="41a93-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="41a93-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="41a93-138">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-138">Yes</span></span>  <br/> |<span data-ttu-id="41a93-139">クライアントのバージョン (例: 15.01.0101.000)。</span><span class="sxs-lookup"><span data-stu-id="41a93-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="41a93-140">文字列</span><span class="sxs-lookup"><span data-stu-id="41a93-140">String</span></span>  <br/> |
|<span data-ttu-id="41a93-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="41a93-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="41a93-142">いいえ</span><span class="sxs-lookup"><span data-stu-id="41a93-142">No</span></span>  <br/> |<span data-ttu-id="41a93-143">移行元のエンティティ (EntityRelevanceAPI、型、貼り付けなど)。</span><span class="sxs-lookup"><span data-stu-id="41a93-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="41a93-144">EntityAddSource 列挙</span><span class="sxs-lookup"><span data-stu-id="41a93-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="41a93-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="41a93-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="41a93-146">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-146">Yes</span></span>  <br/> |<span data-ttu-id="41a93-147">クライアントセッションあたりの増分整数。</span><span class="sxs-lookup"><span data-stu-id="41a93-147">An incremental integer per client session.</span></span> <span data-ttu-id="41a93-148">データ損失を検出するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="41a93-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="41a93-149">Int</span><span class="sxs-lookup"><span data-stu-id="41a93-149">Int</span></span>  <br/> |
|<span data-ttu-id="41a93-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="41a93-150">**EventType**</span></span> <br/> |<span data-ttu-id="41a93-151">はい</span><span class="sxs-lookup"><span data-stu-id="41a93-151">Yes</span></span>  <br/> |<span data-ttu-id="41a93-152">イベントの種類 (たとえば、エンティティが追加され、エンティティが削除された場合)。</span><span class="sxs-lookup"><span data-stu-id="41a93-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="41a93-153">文字列</span><span class="sxs-lookup"><span data-stu-id="41a93-153">String</span></span>  <br/> |
|<span data-ttu-id="41a93-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="41a93-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="41a93-155">いいえ</span><span class="sxs-lookup"><span data-stu-id="41a93-155">No</span></span>  <br/> |<span data-ttu-id="41a93-156">イベント (キー/値のペアの JSON blob) に関連付けられている追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="41a93-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="41a93-157">JSON Blob</span><span class="sxs-lookup"><span data-stu-id="41a93-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="41a93-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="41a93-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="41a93-159">いいえ</span><span class="sxs-lookup"><span data-stu-id="41a93-159">No</span></span>  <br/> |<span data-ttu-id="41a93-160">イベントに関連付けられているエンティティのリスト。</span><span class="sxs-lookup"><span data-stu-id="41a93-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="41a93-161">JSON 文字列</span><span class="sxs-lookup"><span data-stu-id="41a93-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="41a93-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="41a93-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="41a93-163">いいえ</span><span class="sxs-lookup"><span data-stu-id="41a93-163">No</span></span>  <br/> |<span data-ttu-id="41a93-164">Id (GUID) は、クエリログの ID を関連付けます。</span><span class="sxs-lookup"><span data-stu-id="41a93-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="41a93-165">文字列</span><span class="sxs-lookup"><span data-stu-id="41a93-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="41a93-166">AddEntityFeedback 操作の成功応答</span><span class="sxs-lookup"><span data-stu-id="41a93-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="41a93-167">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="41a93-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="41a93-168">エラー</span><span class="sxs-lookup"><span data-stu-id="41a93-168">Errors</span></span> 
  
<span data-ttu-id="41a93-169">API はフィードバックエントリのバッチをログに記録することができ、できることをすべてログに記録します。</span><span class="sxs-lookup"><span data-stu-id="41a93-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="41a93-170">このフィールドは、ログに記録されなかったエラーエントリの数を表します。</span><span class="sxs-lookup"><span data-stu-id="41a93-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="41a93-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="41a93-171">ErrorDetails</span></span>
  
<span data-ttu-id="41a93-172">上記のエラーに関連する詳細情報 `;` 。</span><span class="sxs-lookup"><span data-stu-id="41a93-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="41a93-173">現在サポートされている値</span><span class="sxs-lookup"><span data-stu-id="41a93-173">Currently supported values</span></span>

|<span data-ttu-id="41a93-174">**ClientIdType 列挙型**</span><span class="sxs-lookup"><span data-stu-id="41a93-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="41a93-175">Desktop</span><span class="sxs-lookup"><span data-stu-id="41a93-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="41a93-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="41a93-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="41a93-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="41a93-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="41a93-178">Lync</span><span class="sxs-lookup"><span data-stu-id="41a93-178">Lync</span></span>  <br/> |
|<span data-ttu-id="41a93-179">MacMail</span><span class="sxs-lookup"><span data-stu-id="41a93-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="41a93-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="41a93-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="41a93-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="41a93-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="41a93-182">Other</span><span class="sxs-lookup"><span data-stu-id="41a93-182">Other</span></span>  <br/> |
|<span data-ttu-id="41a93-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="41a93-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="41a93-184">Outlookservice.swift</span><span class="sxs-lookup"><span data-stu-id="41a93-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="41a93-185">POP3</span><span class="sxs-lookup"><span data-stu-id="41a93-185">POP3</span></span>  <br/> |
|<span data-ttu-id="41a93-186">Tablet</span><span class="sxs-lookup"><span data-stu-id="41a93-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="41a93-187">Web</span><span class="sxs-lookup"><span data-stu-id="41a93-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="41a93-188">**EntityAddSource 列挙**</span><span class="sxs-lookup"><span data-stu-id="41a93-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="41a93-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="41a93-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="41a93-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="41a93-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="41a93-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="41a93-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="41a93-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="41a93-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="41a93-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="41a93-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="41a93-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="41a93-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="41a93-195">なし</span><span class="sxs-lookup"><span data-stu-id="41a93-195">None</span></span>  <br/> |
|<span data-ttu-id="41a93-196">その他</span><span class="sxs-lookup"><span data-stu-id="41a93-196">Other</span></span>  <br/> |
|<span data-ttu-id="41a93-197">貼り付け</span><span class="sxs-lookup"><span data-stu-id="41a93-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="41a93-198">AddEntityFeedback 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="41a93-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="41a93-199">EWS に汎用のエラーコードについては[、「応答](responsecode.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41a93-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="41a93-200">FindPeople と共に追加される AddEntityFeedback の例</span><span class="sxs-lookup"><span data-stu-id="41a93-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="41a93-201">FindPeople 要求</span><span class="sxs-lookup"><span data-stu-id="41a93-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a><span data-ttu-id="41a93-202">FindPeople 応答</span><span class="sxs-lookup"><span data-stu-id="41a93-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a><span data-ttu-id="41a93-203">AddEntityFeedback 要求</span><span class="sxs-lookup"><span data-stu-id="41a93-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> <span data-ttu-id="41a93-204">FindPeople response トランザクション ID を AddEntityFeedback 要求トランザクション ID として使用します。</span><span class="sxs-lookup"><span data-stu-id="41a93-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="41a93-205">AddEntityFeedback の応答</span><span class="sxs-lookup"><span data-stu-id="41a93-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


