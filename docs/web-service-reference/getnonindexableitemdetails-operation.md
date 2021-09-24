---
title: GetNonIndexableItemDetails 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: GetNonIndexableItemDetails EWS 操作に関する情報を検索します。
ms.openlocfilehash: d494765d56bc06c2e7f90b99174622b00449116d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516973"
---
# <a name="getnonindexableitemdetails-operation"></a>GetNonIndexableItemDetails 操作

**GetNonIndexableItemDetails** EWS 操作に関する情報を検索します。 
  
**GetNonIndexableItemDetails 操作は**、インデックスを作成できないアイテムの詳細を取得します。 これには、アイテム識別子、エラー コード、エラーの説明、アイテムのインデックス作成をしようとしたタイミング、ファイルに関する追加情報が含まれますが、これに限定されません。 
  
> [!NOTE]
> スキーマは複数のメールボックスを検索できると示しますが、最初のリリース バージョンの Exchange 2013 では、サービスは 1 つのメールボックス内のインデックスを作成できないアイテムのアイテムの詳細の取得のみをサポートします。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getnonindexableitemdetails-operation"></a>GetNonIndexableItemDetails 操作の使用

**GetNonIndexableItemDetails** 操作は、インデックスを作成できないメールボックス アイテムを識別し、アイテムをインデックス化できない理由に関する情報を提供します。 インデックスを作成できないアイテムは、探索検索中は検索されません。 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a>GetNonIndexableItemDetails 操作 SOAP ヘッダー

**GetNonIndexableItemDetails** 操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |呼び出し元が要求を行うのに必要なサーバーの役割を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a>GetNonIndexableItemDetails 操作要求の例: インデックスを作成できないアイテムの詳細を取得する

**GetNonIndexableItemDetails** 操作要求の次の例は、1 つのメールボックスに対してインデックスを作成できないアイテムの詳細を要求する方法を示しています。 検索は、プライマリ メールボックスとアーカイブ メールボックスの両方で実行されます。 
  
> [!NOTE]
> この例のすべての従来のドメイン名は、読みやすさを維持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文には、次の要素が含まれています。
  
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [Mailboxes (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [LegacyDN](legacydn.md)
    
- [SearchArchiveOnly](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a>GetNonIndexableItemDetails 操作応答の成功

次の例は、1 つのメールボックスに対してインデックスを作成できないアイテムを取得する **GetNonIndexableItemDetails** 操作要求に対する正常な応答を示しています。 インデックスを作成できないこの例のアイテムは、不明な形式の binaryfile.abc ファイルです。 
  
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
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)
    
- [NonIndexableItemDetail](nonindexableitemdetail.md)
    
- [ItemId](itemid.md)
    
- [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)
    
- [ErrorDescription](errordescription.md)
    
- [IsPartiallyIndexed](ispartiallyindexed.md)
    
- [IsPermanentFailure](ispermanentfailure.md)
    
- [SortValue](sortvalue.md)
    
- [AttemptCount](attemptcount.md)
    
- [LastAttemptTime](lastattempttime.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a>GetNonIndexableItemDetails 操作エラー応答

次の例は **、GetNonIndexableItemDetails** 操作要求に対するエラー応答を示しています。 これは、複数のメールボックスからインデックスを作成できないアイテムのアイテムの詳細を取得する要求に対する応答です。 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes 操作](getsearchablemailboxes-operation.md)
    
- [SearchMailboxes 操作](searchmailboxes-operation.md)
    
- [GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md)
    
- [SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)
    
- [GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md)
    
- [GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)
    

