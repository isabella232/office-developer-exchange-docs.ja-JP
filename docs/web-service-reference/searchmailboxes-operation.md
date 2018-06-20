---
title: SearchMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: 操作 SearchMailboxes EWS についての情報を検索します。
ms.openlocfilehash: 141ea466a24f3cb400a8e0b63e2162c1eae5d7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833296"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="66825-103">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="66825-103">SearchMailboxes operation</span></span>

<span data-ttu-id="66825-104">**SearchMailboxes** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="66825-104">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="66825-105">**SearchMailboxes**操作は、メールボックスのアイテムに条件に一致する箇所のメールボックスを検索します。</span><span class="sxs-lookup"><span data-stu-id="66825-105">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="66825-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="66825-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="66825-107">SearchMailboxes 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="66825-107">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="66825-108">**SearchMailboxes**操作では、複数のメールボックスで探索検索を実行するのには多くの同時検索クエリを使用できます。</span><span class="sxs-lookup"><span data-stu-id="66825-108">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="66825-109">結果は、いずれかについての統計情報の検索条件が発生すると、または検索語句を含むアイテムのプレビューです。</span><span class="sxs-lookup"><span data-stu-id="66825-109">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="66825-110">SearchMailboxes 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66825-110">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="66825-111">**SearchMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="66825-111">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="66825-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="66825-112">**Header name**</span></span>|<span data-ttu-id="66825-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="66825-113">**Element**</span></span>|<span data-ttu-id="66825-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="66825-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66825-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="66825-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="66825-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="66825-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="66825-117">呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。</span><span class="sxs-lookup"><span data-stu-id="66825-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="66825-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66825-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="66825-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="66825-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="66825-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="66825-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="66825-121">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66825-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="66825-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66825-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="66825-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="66825-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="66825-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="66825-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="66825-125">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66825-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="66825-126">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66825-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="66825-127">SearchMailboxes 操作の要求の例: 検索語のヒット数のメールボックスを検索</span><span class="sxs-lookup"><span data-stu-id="66825-127">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="66825-128">**SearchMailboxes**操作要求の次の例では、メールボックスごとに用語が表示されますが何回かについての統計情報の 3 つの異なるメールボックスを検索するのには 2 つのクエリを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="66825-128">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="66825-129">この例では、[クエリ](query.md)の要素は空白のままに intentionaly です。</span><span class="sxs-lookup"><span data-stu-id="66825-129">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="66825-130">どの要求が成功するは、上のエラー条件を含めることができますが表示、検索ごとのメールボックス。</span><span class="sxs-lookup"><span data-stu-id="66825-130">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SearchMailboxes>
         <m:SearchQueries>
            <t:MailboxQuery>
               <t:Query>Test Item</t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=12311a742f0e47e392c8201a60d13ecf-Steve</t:Mailbox>
                     <t:SearchScope>All</t:SearchScope>
                  </t:MailboxSearchScope>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=f00c9f70539844beb52341d8f40c572e-Antho</t:Mailbox>
                     <t:SearchScope>PrimaryOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
            <t:MailboxQuery>
               <t:Query></t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=accba4fd5ddf12214a0e82ce1645f4e-Danie</t:Mailbox>
                     <t:SearchScope>ArchiveOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
         </m:SearchQueries>
         <m:ResultType>StatisticsOnly</m:ResultType>
      </m:SearchMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="66825-131">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66825-131">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66825-132">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="66825-132">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="66825-133">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="66825-133">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="66825-134">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="66825-134">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="66825-135">Query</span><span class="sxs-lookup"><span data-stu-id="66825-135">Query</span></span>](query.md)
    
- [<span data-ttu-id="66825-136">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="66825-136">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="66825-137">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-137">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="66825-138">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="66825-138">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="66825-139">SearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-139">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="66825-140">結果</span><span class="sxs-lookup"><span data-stu-id="66825-140">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="66825-141">SearchMailboxes 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="66825-141">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="66825-142">ターゲット メールボックスの検索用語が見つかった回数に関する統計情報を取得する**SearchMailboxes**操作要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66825-142">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="66825-143">最後のクエリには、失敗したメールボックスの検索を表示する、空の**クエリ**要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66825-143">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=35181a94327e392c8201a60d13ecf-Steve</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=f00c9f789572-beb04001d8f40c572e-Antho</t:Mailbox>
                              <t:SearchScope>PrimaryOnly</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>2</t:ItemCount>
                  <t:Size>20206</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:KeywordStats>
                     <t:KeywordStat>
                        <t:Keyword>Test Item</t:Keyword>
                        <t:ItemHits>2</t:ItemHits>
                        <t:Size>20206</t:Size>
                     </t:KeywordStat>
                  </t:KeywordStats>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=accba4as3df234234a0e82ce1645f4e-Danie</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>The search query can't be empty.</t:ErrorMessage>
                        <t:IsArchive>true</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="66825-144">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66825-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66825-145">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="66825-145">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="66825-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66825-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="66825-147">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66825-147">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="66825-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="66825-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="66825-149">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="66825-149">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="66825-150">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="66825-150">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="66825-151">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="66825-151">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="66825-152">Query</span><span class="sxs-lookup"><span data-stu-id="66825-152">Query</span></span>](query.md)
    
- [<span data-ttu-id="66825-153">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="66825-153">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="66825-154">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-154">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="66825-155">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="66825-155">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="66825-156">SearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-156">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="66825-157">結果</span><span class="sxs-lookup"><span data-stu-id="66825-157">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="66825-158">ItemCount</span><span class="sxs-lookup"><span data-stu-id="66825-158">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="66825-159">サイズ (長)</span><span class="sxs-lookup"><span data-stu-id="66825-159">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="66825-160">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="66825-160">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="66825-161">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="66825-161">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="66825-162">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="66825-162">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="66825-163">キーワード</span><span class="sxs-lookup"><span data-stu-id="66825-163">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="66825-164">ItemHits</span><span class="sxs-lookup"><span data-stu-id="66825-164">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="66825-165">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="66825-165">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="66825-166">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="66825-166">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="66825-167">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="66825-167">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="66825-168">エラー コード (int)</span><span class="sxs-lookup"><span data-stu-id="66825-168">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="66825-169">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="66825-169">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="66825-170">IsArchive</span><span class="sxs-lookup"><span data-stu-id="66825-170">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="66825-171">SearchMailboxes 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="66825-171">SearchMailboxes operation error response</span></span>

<span data-ttu-id="66825-172">**SearchMailboxes**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66825-172">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="66825-173">これは、メールボックスの id が正しくない場合、メールボックスを検索するための要求への応答です。</span><span class="sxs-lookup"><span data-stu-id="66825-173">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Error">
               <m:MessageText>No mailbox is specified for search operation. If specified in the request, 
               then it could be due to permission issue.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>subject:Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>0</t:ItemCount>
                  <t:Size>0</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>No mailbox is specified for search operation. If specified in the request, 
                        then it could be due to permission issue.</t:ErrorMessage>
                        <t:IsArchive>false</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="66825-174">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66825-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66825-175">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="66825-175">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="66825-176">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66825-176">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="66825-177">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66825-177">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="66825-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="66825-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="66825-179">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="66825-179">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="66825-180">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="66825-180">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="66825-181">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="66825-181">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="66825-182">Query</span><span class="sxs-lookup"><span data-stu-id="66825-182">Query</span></span>](query.md)
    
- [<span data-ttu-id="66825-183">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="66825-183">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="66825-184">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-184">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="66825-185">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="66825-185">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="66825-186">SearchScope</span><span class="sxs-lookup"><span data-stu-id="66825-186">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="66825-187">結果</span><span class="sxs-lookup"><span data-stu-id="66825-187">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="66825-188">ItemCount</span><span class="sxs-lookup"><span data-stu-id="66825-188">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="66825-189">サイズ (長)</span><span class="sxs-lookup"><span data-stu-id="66825-189">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="66825-190">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="66825-190">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="66825-191">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="66825-191">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="66825-192">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="66825-192">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="66825-193">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="66825-193">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="66825-194">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="66825-194">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="66825-195">エラー コード (int)</span><span class="sxs-lookup"><span data-stu-id="66825-195">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="66825-196">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="66825-196">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="66825-197">IsArchive</span><span class="sxs-lookup"><span data-stu-id="66825-197">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="66825-198">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66825-198">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="66825-199">関連項目</span><span class="sxs-lookup"><span data-stu-id="66825-199">See also</span></span>

- [<span data-ttu-id="66825-200">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="66825-200">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="66825-201">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="66825-201">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="66825-202">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="66825-202">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="66825-203">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="66825-203">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="66825-204">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="66825-204">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="66825-205">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="66825-205">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="66825-206">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="66825-206">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

