---
title: SearchMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: SearchMailboxes EWS 操作に関する情報を検索します。
ms.openlocfilehash: 6e154525f5ff2c3d4f24ddc50e1dae1b04a891ba
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521682"
---
# <a name="searchmailboxes-operation"></a>SearchMailboxes 操作

> [!NOTE]
> この操作は廃止され、Microsoft ではサポートされなくなりました。  代わりとして [、FindItem 操作を使用](finditem-operation.md) してください。

**SearchMailboxes** EWS 操作に関する情報を検索します。 
  
**SearchMailboxes 操作は**、メールボックス アイテム内の用語の出現をメールボックスで検索します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-searchmailboxes-operation"></a>SearchMailboxes 操作の使用

**SearchMailboxes 操作では**、多数の同時検索クエリを使用して、複数のメールボックスで探索検索を実行できます。 検索結果には、検索用語の発生回数に関する統計情報、または検索用語を含むアイテムのプレビューのいずれかを指定できます。 
  
### <a name="searchmailboxes-operation-soap-headers"></a>SearchMailboxes 操作 SOAP ヘッダー

**SearchMailboxes 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |呼び出し元が要求を行うのに必要なサーバーの役割を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a>SearchMailboxes 操作要求の例: 検索用語のヒット数を検索するメールボックス

**SearchMailboxes** 操作要求の次の例は、2 つの異なるクエリを使用して 3 つの異なるメールボックスを検索して、各メールボックスに用語が表示される回数に関する統計情報を検索する方法を示しています。 
  
> [!NOTE]
> この例では [、Query 要素](query.md) は意図的に空白のままです。 これは、成功した要求にメールボックス検索ごとにエラー条件を含む方法を示しています。 
  
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

要求 SOAP 本文には、次の要素が含まれています。
  
- [SearchMailboxes](searchmailboxes.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [クエリ](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [Mailbox (string)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [ResultType](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a>SearchMailboxes 操作の応答の成功

次の例は **、SearchMailboxes** 操作要求に対する正常な応答を示し、検索用語がターゲット メールボックスで見つかった回数に関する統計情報を取得します。 最後のクエリには、失敗したメールボックスの検索を示す空の **Query** 要素が含まれている。 
  
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

応答 SOAP 本文には、次の要素が含まれています。
  
- [SearchMailboxesResponse](searchmailboxesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchMailboxesResult](searchmailboxesresult.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [クエリ](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [Mailbox (string)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [ResultType](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [Size (long)](size-long.md)
    
- [PageItemCount](pageitemcount.md)
    
- [KeywordStats](keywordstats.md)
    
- [KeywordStat](keywordstat.md)
    
- [キーワード](keyword.md)
    
- [ItemHits](itemhits.md)
    
- [FailedMailboxes](failedmailboxes.md)
    
- [FailedMailbox](failedmailbox.md)
    
- [Mailbox (string)](mailbox-string.md)
    
- [ErrorCode (int)](errorcode-int.md)
    
- [ErrorMessage](errormessage.md)
    
- [IsArchive](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a>SearchMailboxes 操作エラー応答

次の例は **、SearchMailboxes 操作要求に対するエラー応答を** 示しています。 これは、メールボックス識別子が正しくない場合にメールボックスを検索する要求に対する応答です。 
  
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

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [SearchMailboxesResponse](searchmailboxesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchMailboxesResult](searchmailboxesresult.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [クエリ](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [Mailbox (string)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [ResultType](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [Size (long)](size-long.md)
    
- [PageItemCount](pageitemcount.md)
    
- [PageItemSize](pageitemsize.md)
    
- [FailedMailboxes](failedmailboxes.md)
    
- [FailedMailbox](failedmailbox.md)
    
- [Mailbox (string)](mailbox-string.md)
    
- [ErrorCode (int)](errorcode-int.md)
    
- [ErrorMessage](errormessage.md)
    
- [IsArchive](isarchive.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes 操作](getsearchablemailboxes-operation.md)
    
- [SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)
    
- [GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md)
    
- [GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md)
    
- [GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)
    
- [GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)
    

