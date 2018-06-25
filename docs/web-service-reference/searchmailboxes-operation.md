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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833296"
---
# <a name="searchmailboxes-operation"></a>SearchMailboxes 操作

**SearchMailboxes** EWS の操作に関する情報を検索します。 
  
**SearchMailboxes**操作は、メールボックスのアイテムに条件に一致する箇所のメールボックスを検索します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-searchmailboxes-operation"></a>SearchMailboxes 操作を使用します。

**SearchMailboxes**操作では、複数のメールボックスで探索検索を実行するのには多くの同時検索クエリを使用できます。 結果は、いずれかについての統計情報の検索条件が発生すると、または検索語句を含むアイテムのプレビューです。 
  
### <a name="searchmailboxes-operation-soap-headers"></a>SearchMailboxes 操作の SOAP ヘッダー

**SearchMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a>SearchMailboxes 操作の要求の例: 検索語のヒット数のメールボックスを検索

**SearchMailboxes**操作要求の次の例では、メールボックスごとに用語が表示されますが何回かについての統計情報の 3 つの異なるメールボックスを検索するのには 2 つのクエリを使用する方法を示します。 
  
> [!NOTE]
> この例では、[クエリ](query.md)の要素は空白のままに intentionaly です。 どの要求が成功するは、上のエラー条件を含めることができますが表示、検索ごとのメールボックス。 
  
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

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [SearchMailboxes](searchmailboxes.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [Query](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [メールボックス (文字列)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [結果](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a>SearchMailboxes 操作の成功の応答

ターゲット メールボックスの検索用語が見つかった回数に関する統計情報を取得する**SearchMailboxes**操作要求に正常な応答の例を次に示します。 最後のクエリには、失敗したメールボックスの検索を表示する、空の**クエリ**要素が含まれています。 
  
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

応答 SOAP 本文には、次の要素が含まれています。
  
- [SearchMailboxesResponse](searchmailboxesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchMailboxesResult](searchmailboxesresult.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [Query](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [メールボックス (文字列)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [結果](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [サイズ (長)](size-long.md)
    
- [PageItemCount](pageitemcount.md)
    
- [KeywordStats](keywordstats.md)
    
- [KeywordStat](keywordstat.md)
    
- [キーワード](keyword.md)
    
- [ItemHits](itemhits.md)
    
- [FailedMailboxes](failedmailboxes.md)
    
- [FailedMailbox](failedmailbox.md)
    
- [メールボックス (文字列)](mailbox-string.md)
    
- [エラー コード (int)](errorcode-int.md)
    
- [エラー メッセージ](errormessage.md)
    
- [IsArchive](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a>SearchMailboxes 操作のエラー応答

**SearchMailboxes**操作の要求に対してエラー応答の例を次に示します。 これは、メールボックスの id が正しくない場合、メールボックスを検索するための要求への応答です。 
  
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

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [SearchMailboxesResponse](searchmailboxesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchMailboxesResult](searchmailboxesresult.md)
    
- [SearchQueries](searchqueries.md)
    
- [MailboxQuery](mailboxquery.md)
    
- [Query](query.md)
    
- [MailboxSearchScopes](mailboxsearchscopes.md)
    
- [MailboxSearchScope](mailboxsearchscope.md)
    
- [メールボックス (文字列)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [結果](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [サイズ (長)](size-long.md)
    
- [PageItemCount](pageitemcount.md)
    
- [PageItemSize](pageitemsize.md)
    
- [FailedMailboxes](failedmailboxes.md)
    
- [FailedMailbox](failedmailbox.md)
    
- [メールボックス (文字列)](mailbox-string.md)
    
- [エラー コード (int)](errorcode-int.md)
    
- [エラー メッセージ](errormessage.md)
    
- [IsArchive](isarchive.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes 操作](getsearchablemailboxes-operation.md)
    
- [SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)
    
- [GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md)
    
- [GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md)
    
- [GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)
    
- [GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)
    

