---
title: AddEntityFeedback 操作
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: AddEntityFeedback 操作では、サーバー側の問題に対応するエラー情報を返します。
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759285"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="137a2-103">AddEntityFeedback 操作</span><span class="sxs-lookup"><span data-stu-id="137a2-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="137a2-104">**AddEntityFeedback**操作では、サーバー側の問題に対応するエラー情報を返します。</span><span class="sxs-lookup"><span data-stu-id="137a2-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="137a2-105">この操作は、ログに記録されるイベントの種類に依存しています。</span><span class="sxs-lookup"><span data-stu-id="137a2-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="137a2-106">いずれかの最も重要なイベントは、 **EntityAdded**、選択されているエンティティに対応します。</span><span class="sxs-lookup"><span data-stu-id="137a2-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="137a2-107">この操作は、1 つの要求のバッチのエントリをログに記録するために使用できるように、バッチをします。</span><span class="sxs-lookup"><span data-stu-id="137a2-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="137a2-108">FindPeople 要求の例</span><span class="sxs-lookup"><span data-stu-id="137a2-108">FindPeople request examples</span></span>

<span data-ttu-id="137a2-109">**AddEntityFeedback**操作は、クライアント サービスによって返されるエンティティとの対話の詳細をログに記録するための手段を提供します。</span><span class="sxs-lookup"><span data-stu-id="137a2-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="137a2-110">これは、クライアントごとにバック グラウンドで関連性を向上させるために、信号として使用できます。</span><span class="sxs-lookup"><span data-stu-id="137a2-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="137a2-111">など、クライアントでは、 **FindPeople**から返されたユーザー エンティティに関するフィードバックを提供するのにこの操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="137a2-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="137a2-112">要求の SOAP 本文の内容</span><span class="sxs-lookup"><span data-stu-id="137a2-112">The request SOAP body contents</span></span>

<span data-ttu-id="137a2-113">Soap 要求には、 **EntityFeedbackEntries**の単一の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="137a2-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="137a2-114">これには、 **EntityFeedbackEntry**オブジェクトの配列に含まれています。</span><span class="sxs-lookup"><span data-stu-id="137a2-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="137a2-115">配列内の各エントリには、次の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="137a2-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="137a2-116">**要求パラメーター**</span><span class="sxs-lookup"><span data-stu-id="137a2-116">**Request Parameters**</span></span>|<span data-ttu-id="137a2-117">**必須**</span><span class="sxs-lookup"><span data-stu-id="137a2-117">**Required**</span></span>|<span data-ttu-id="137a2-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="137a2-118">**Description**</span></span>|<span data-ttu-id="137a2-119">**型**</span><span class="sxs-lookup"><span data-stu-id="137a2-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="137a2-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="137a2-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="137a2-121">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-121">Yes</span></span>  <br/> |<span data-ttu-id="137a2-122">UTC 時刻クライアント側のイベントが発生しました。</span><span class="sxs-lookup"><span data-stu-id="137a2-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="137a2-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="137a2-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="137a2-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="137a2-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="137a2-125">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-125">Yes</span></span>  <br/> |<span data-ttu-id="137a2-126">現地時刻は、クライアント側のイベントが発生しました。</span><span class="sxs-lookup"><span data-stu-id="137a2-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="137a2-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="137a2-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="137a2-128">**クライアント Id**</span><span class="sxs-lookup"><span data-stu-id="137a2-128">**ClientId**</span></span> <br/> |<span data-ttu-id="137a2-129">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-129">Yes</span></span>  <br/> |<span data-ttu-id="137a2-130">クライアント (たとえば、Outlook、OWA など) の種類です。</span><span class="sxs-lookup"><span data-stu-id="137a2-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="137a2-131">ClientIDType 列挙型</span><span class="sxs-lookup"><span data-stu-id="137a2-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="137a2-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="137a2-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="137a2-133">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-133">Yes</span></span>  <br/> |<span data-ttu-id="137a2-134">GUID は、セッション ID を識別します。</span><span class="sxs-lookup"><span data-stu-id="137a2-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="137a2-135">クライアント上で生成されます。</span><span class="sxs-lookup"><span data-stu-id="137a2-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="137a2-136">GUID</span><span class="sxs-lookup"><span data-stu-id="137a2-136">GUID</span></span>  <br/> |
|<span data-ttu-id="137a2-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="137a2-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="137a2-138">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-138">Yes</span></span>  <br/> |<span data-ttu-id="137a2-139">(15.01.0101.000 など) のクライアントのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="137a2-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="137a2-140">String</span><span class="sxs-lookup"><span data-stu-id="137a2-140">String</span></span>  <br/> |
|<span data-ttu-id="137a2-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="137a2-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="137a2-142">いいえ</span><span class="sxs-lookup"><span data-stu-id="137a2-142">No</span></span>  <br/> |<span data-ttu-id="137a2-143">EntityAded (など、EntityRelevanceAPI、種類、貼り付け) のソースです。</span><span class="sxs-lookup"><span data-stu-id="137a2-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="137a2-144">EntityAddSource 列挙型</span><span class="sxs-lookup"><span data-stu-id="137a2-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="137a2-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="137a2-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="137a2-146">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-146">Yes</span></span>  <br/> |<span data-ttu-id="137a2-147">クライアント セッションごとの増分の整数です。</span><span class="sxs-lookup"><span data-stu-id="137a2-147">An incremental integer per client session.</span></span> <span data-ttu-id="137a2-148">データの損失を検出するために使用します。</span><span class="sxs-lookup"><span data-stu-id="137a2-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="137a2-149">整数型 (Int)</span><span class="sxs-lookup"><span data-stu-id="137a2-149">Int</span></span>  <br/> |
|<span data-ttu-id="137a2-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="137a2-150">**EventType**</span></span> <br/> |<span data-ttu-id="137a2-151">はい</span><span class="sxs-lookup"><span data-stu-id="137a2-151">Yes</span></span>  <br/> |<span data-ttu-id="137a2-152">(などのエンティティが追加されると、エンティティが削除される) イベントの種類です。</span><span class="sxs-lookup"><span data-stu-id="137a2-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="137a2-153">String</span><span class="sxs-lookup"><span data-stu-id="137a2-153">String</span></span>  <br/> |
|<span data-ttu-id="137a2-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="137a2-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="137a2-155">いいえ</span><span class="sxs-lookup"><span data-stu-id="137a2-155">No</span></span>  <br/> |<span data-ttu-id="137a2-156">イベント (キーと値のペアの JSON blob) に関連付けられた追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="137a2-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="137a2-157">JSON Blob</span><span class="sxs-lookup"><span data-stu-id="137a2-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="137a2-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="137a2-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="137a2-159">いいえ</span><span class="sxs-lookup"><span data-stu-id="137a2-159">No</span></span>  <br/> |<span data-ttu-id="137a2-160">イベントに関連付けられているエンティティの一覧です。</span><span class="sxs-lookup"><span data-stu-id="137a2-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="137a2-161">JSON 文字列</span><span class="sxs-lookup"><span data-stu-id="137a2-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="137a2-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="137a2-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="137a2-163">いいえ</span><span class="sxs-lookup"><span data-stu-id="137a2-163">No</span></span>  <br/> |<span data-ttu-id="137a2-164">ID (GUID) クエリ ログの ID を関連付けることです。</span><span class="sxs-lookup"><span data-stu-id="137a2-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="137a2-165">String</span><span class="sxs-lookup"><span data-stu-id="137a2-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="137a2-166">AddEntityFeedback 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="137a2-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="137a2-167">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="137a2-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="137a2-168">エラー</span><span class="sxs-lookup"><span data-stu-id="137a2-168">Errors</span></span> 
  
<span data-ttu-id="137a2-169">フィードバック項目のバッチをログに記録できる API、ことをすべてログに記録しました。</span><span class="sxs-lookup"><span data-stu-id="137a2-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="137a2-170">このフィールドは、エラーのエントリが記録されていないの数を表します。</span><span class="sxs-lookup"><span data-stu-id="137a2-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="137a2-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="137a2-171">ErrorDetails</span></span>
  
<span data-ttu-id="137a2-172">によって上記のエラーに関連する詳細を分離`;`。</span><span class="sxs-lookup"><span data-stu-id="137a2-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="137a2-173">現在サポートされている値</span><span class="sxs-lookup"><span data-stu-id="137a2-173">Currently supported values</span></span>

|<span data-ttu-id="137a2-174">**ClientIdType 列挙型**</span><span class="sxs-lookup"><span data-stu-id="137a2-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="137a2-175">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="137a2-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="137a2-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="137a2-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="137a2-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="137a2-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="137a2-178">Lync</span><span class="sxs-lookup"><span data-stu-id="137a2-178">Lync</span></span>  <br/> |
|<span data-ttu-id="137a2-179">MacMail</span><span class="sxs-lookup"><span data-stu-id="137a2-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="137a2-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="137a2-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="137a2-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="137a2-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="137a2-182">Other</span><span class="sxs-lookup"><span data-stu-id="137a2-182">Other</span></span>  <br/> |
|<span data-ttu-id="137a2-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="137a2-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="137a2-184">OutlookService</span><span class="sxs-lookup"><span data-stu-id="137a2-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="137a2-185">POP3</span><span class="sxs-lookup"><span data-stu-id="137a2-185">POP3</span></span>  <br/> |
|<span data-ttu-id="137a2-186">Tablet</span><span class="sxs-lookup"><span data-stu-id="137a2-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="137a2-187">Web</span><span class="sxs-lookup"><span data-stu-id="137a2-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="137a2-188">**EntityAddSource 列挙型**</span><span class="sxs-lookup"><span data-stu-id="137a2-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="137a2-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="137a2-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="137a2-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="137a2-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="137a2-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="137a2-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="137a2-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="137a2-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="137a2-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="137a2-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="137a2-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="137a2-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="137a2-195">なし</span><span class="sxs-lookup"><span data-stu-id="137a2-195">None</span></span>  <br/> |
|<span data-ttu-id="137a2-196">その他</span><span class="sxs-lookup"><span data-stu-id="137a2-196">Other</span></span>  <br/> |
|<span data-ttu-id="137a2-197">貼り付け</span><span class="sxs-lookup"><span data-stu-id="137a2-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="137a2-198">AddEntityFeedback 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="137a2-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="137a2-199">EWS を汎用のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="137a2-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="137a2-200">FindPeople と共に AddEntityFeedback の例</span><span class="sxs-lookup"><span data-stu-id="137a2-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="137a2-201">FindPeople 要求</span><span class="sxs-lookup"><span data-stu-id="137a2-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

#### <a name="findpeople-response"></a><span data-ttu-id="137a2-202">FindPeople 応答</span><span class="sxs-lookup"><span data-stu-id="137a2-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

#### <a name="addentityfeedback-request"></a><span data-ttu-id="137a2-203">AddEntityFeedback 要求</span><span class="sxs-lookup"><span data-stu-id="137a2-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> <span data-ttu-id="137a2-204">FindPeople を使用して AddEntityFeedback 要求のトランザクションとしてトランザクション ID を応答の id。</span><span class="sxs-lookup"><span data-stu-id="137a2-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="137a2-205">AddEntityFeedback 応答</span><span class="sxs-lookup"><span data-stu-id="137a2-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


