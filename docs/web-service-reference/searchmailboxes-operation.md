---
title: SearchMailboxes ボックスの操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: SearchMailboxes ボックス EWS 操作についての情報を検索します。
ms.openlocfilehash: 9ec7e9dd4ef17f22f236e64ca1fdbeb65e6e56fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456773"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="cb533-103">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="cb533-103">SearchMailboxes operation</span></span>

> [!NOTE]
> <span data-ttu-id="cb533-104">この操作は推奨されておらず、Microsoft ではサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="cb533-104">This operation is deprecated, and no longer supported by Microsoft.</span></span>  <span data-ttu-id="cb533-105">代替として、 [FindItem](finditem-operation.md)操作を使用してください。</span><span class="sxs-lookup"><span data-stu-id="cb533-105">As a replacement, please use the [FindItem](finditem-operation.md) operation.</span></span>

<span data-ttu-id="cb533-106">**Searchmailboxes ボックス**EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="cb533-106">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="cb533-107">**Searchmailboxes**操作は、メールボックスアイテム内の用語の出現についてメールボックスを検索します。</span><span class="sxs-lookup"><span data-stu-id="cb533-107">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="cb533-108">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cb533-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="cb533-109">SearchMailboxes ボックス操作の使用</span><span class="sxs-lookup"><span data-stu-id="cb533-109">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="cb533-110">**Searchmailboxes ボックス**操作は、複数のメールボックスで探索検索を実行するために、多数の同時検索クエリを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cb533-110">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="cb533-111">結果には、検索語句の出現回数に関する統計情報、または検索語を含むアイテムのプレビューがあります。</span><span class="sxs-lookup"><span data-stu-id="cb533-111">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="cb533-112">SearchMailboxes ボックス操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb533-112">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="cb533-113">**Searchmailboxes ボックス**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cb533-113">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cb533-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="cb533-114">**Header name**</span></span>|<span data-ttu-id="cb533-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb533-115">**Element**</span></span>|<span data-ttu-id="cb533-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb533-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cb533-117">**Get-managementrole**</span><span class="sxs-lookup"><span data-stu-id="cb533-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="cb533-118">Get-managementrole</span><span class="sxs-lookup"><span data-stu-id="cb533-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="cb533-119">発信者が要求を行うために必要なサーバーの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb533-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="cb533-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cb533-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cb533-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cb533-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cb533-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cb533-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cb533-123">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cb533-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cb533-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cb533-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cb533-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cb533-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cb533-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cb533-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cb533-127">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cb533-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cb533-128">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cb533-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="cb533-129">SearchMailboxes ボックス操作要求の例: 検索用語の数の検索メールボックス</span><span class="sxs-lookup"><span data-stu-id="cb533-129">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="cb533-130">次の**searchmailboxes**操作要求の例は、2つの異なるクエリを使用して、用語が各メールボックスに表示される回数に関する統計情報を検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cb533-130">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cb533-131">この例では、 [Query](query.md)要素は空白のままに intentionaly ます。</span><span class="sxs-lookup"><span data-stu-id="cb533-131">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="cb533-132">これは、成功した要求に、メールボックスの検索基準ごとにエラー状態を含める方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cb533-132">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="cb533-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb533-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb533-134">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="cb533-134">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="cb533-135">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="cb533-135">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="cb533-136">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="cb533-136">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="cb533-137">Query</span><span class="sxs-lookup"><span data-stu-id="cb533-137">Query</span></span>](query.md)
    
- [<span data-ttu-id="cb533-138">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="cb533-138">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="cb533-139">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-139">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="cb533-140">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cb533-140">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cb533-141">SearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-141">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="cb533-142">ResultType</span><span class="sxs-lookup"><span data-stu-id="cb533-142">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="cb533-143">成功した SearchMailboxes ボックス操作の応答</span><span class="sxs-lookup"><span data-stu-id="cb533-143">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="cb533-144">次の例では、 **Searchmailboxes ボックス**操作要求に対する正常な応答を示し、検索用語が対象のメールボックス内で検索された回数に関する統計情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb533-144">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="cb533-145">最後のクエリに空の**クエリ**要素が含まれています。これは、失敗したメールボックスの検索を示します。</span><span class="sxs-lookup"><span data-stu-id="cb533-145">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="cb533-146">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb533-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb533-147">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="cb533-147">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="cb533-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cb533-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cb533-149">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cb533-149">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="cb533-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb533-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cb533-151">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="cb533-151">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="cb533-152">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="cb533-152">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="cb533-153">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="cb533-153">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="cb533-154">Query</span><span class="sxs-lookup"><span data-stu-id="cb533-154">Query</span></span>](query.md)
    
- [<span data-ttu-id="cb533-155">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="cb533-155">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="cb533-156">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-156">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="cb533-157">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cb533-157">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cb533-158">SearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-158">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="cb533-159">ResultType</span><span class="sxs-lookup"><span data-stu-id="cb533-159">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="cb533-160">ItemCount</span><span class="sxs-lookup"><span data-stu-id="cb533-160">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="cb533-161">サイズ (長い)</span><span class="sxs-lookup"><span data-stu-id="cb533-161">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="cb533-162">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="cb533-162">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="cb533-163">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="cb533-163">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="cb533-164">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="cb533-164">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="cb533-165">キーワード</span><span class="sxs-lookup"><span data-stu-id="cb533-165">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="cb533-166">ItemHits</span><span class="sxs-lookup"><span data-stu-id="cb533-166">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="cb533-167">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="cb533-167">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="cb533-168">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="cb533-168">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="cb533-169">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cb533-169">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cb533-170">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="cb533-170">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="cb533-171">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="cb533-171">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="cb533-172">IsArchive</span><span class="sxs-lookup"><span data-stu-id="cb533-172">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="cb533-173">SearchMailboxes ボックス操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="cb533-173">SearchMailboxes operation error response</span></span>

<span data-ttu-id="cb533-174">次の例は、 **Searchmailboxes ボックス**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cb533-174">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="cb533-175">これは、メールボックス識別子が正しくない場合にメールボックスを検索する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="cb533-175">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="cb533-176">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb533-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb533-177">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="cb533-177">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="cb533-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cb533-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cb533-179">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cb533-179">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="cb533-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb533-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cb533-181">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="cb533-181">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="cb533-182">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="cb533-182">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="cb533-183">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="cb533-183">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="cb533-184">Query</span><span class="sxs-lookup"><span data-stu-id="cb533-184">Query</span></span>](query.md)
    
- [<span data-ttu-id="cb533-185">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="cb533-185">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="cb533-186">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-186">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="cb533-187">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cb533-187">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cb533-188">SearchScope</span><span class="sxs-lookup"><span data-stu-id="cb533-188">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="cb533-189">ResultType</span><span class="sxs-lookup"><span data-stu-id="cb533-189">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="cb533-190">ItemCount</span><span class="sxs-lookup"><span data-stu-id="cb533-190">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="cb533-191">サイズ (長い)</span><span class="sxs-lookup"><span data-stu-id="cb533-191">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="cb533-192">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="cb533-192">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="cb533-193">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="cb533-193">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="cb533-194">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="cb533-194">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="cb533-195">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="cb533-195">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="cb533-196">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="cb533-196">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="cb533-197">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="cb533-197">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="cb533-198">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="cb533-198">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="cb533-199">IsArchive</span><span class="sxs-lookup"><span data-stu-id="cb533-199">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="cb533-200">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="cb533-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cb533-201">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb533-201">See also</span></span>

- [<span data-ttu-id="cb533-202">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="cb533-203">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="cb533-203">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="cb533-204">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-204">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="cb533-205">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-205">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="cb533-206">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-206">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="cb533-207">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-207">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="cb533-208">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="cb533-208">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

