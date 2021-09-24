---
title: GetSearchableMailboxes 操作
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: GetSearchableMailboxes EWS 操作に関する情報を検索します。
ms.openlocfilehash: 385a1e317069641c51249c9522cf404ecf961722
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523084"
---
# <a name="getsearchablemailboxes-operation"></a>GetSearchableMailboxes 操作

> [!IMPORTANT]
> 2020 年 4 月 1 日から、GetSearchableMailboxes 操作は、このページで使用できExchange Online。 この操作は、オンプレミスのバージョンのサーバーでは影響を受Exchange Server。 詳細については、「従来の電子[情報開示ツールの削除」を参照Exchange Online。](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api)

**GetSearchableMailboxes** EWS 操作に関する情報を検索します。 
  
**GetSearchableMailboxes 操作は**、探索検索用の検索可能なメールボックスのスコープセットを取得します。 応答で返される検索可能なメールボックスの範囲は、検索フィルターと配布グループ メンバーシップが展開されるかどうかによって決まります。 

> [!NOTE] 
> この操作は、検索フィルターと一緒に使用し、最初の数千のみを取得することを目的とします。これは、完全な取得を目的としていない。
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getsearchablemailboxes-operation"></a>GetSearchableMailboxes 操作の使用

**GetSearchableMailboxes 操作は、** 検索可能なメールボックスに関する情報を取得します。 要求には、次の引数を渡します。 
  
- [SearchFilter](searchfilter.md) - 1 つの電子メール エイリアスを引数として受け入れる。 
    
- [ExpandGroupMembership](expandgroupmembership.md) - 応答で返される結果で配布グループ メンバーシップが展開されるかどうかを示します。 
    
検索フィルターで設定された電子メール エイリアスが配布グループであり、配布グループのメンバーシップが展開されていない場合、応答には配布グループのメールボックス情報が含まれる。 検索フィルターで設定された電子メール エイリアスが配布グループであり、配布グループのメンバーシップが展開されている場合、応答には、配布グループのメンバーである各メールボックスのメールボックス情報が含まれる。 検索フィルターに 1 人のユーザーのエイリアスが含まれている場合、応答には 1 人のユーザーのメールボックス情報が含まれる。 [GetSearchableMailboxes](getsearchablemailboxes.md)要素が空の場合、応答には検索可能なすべてのメールボックスが含まれる。 これは、空の [SearchFilter](searchfilter.md) 要素と [ExpandGroupMembership](expandgroupmembership.md) 要素が false に設定されているのと同 **じです**。
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>GetSearchableMailboxes 操作 SOAP ヘッダー

**GetSearchableMailboxes 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|ヘッダー名|要素|説明|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |呼び出し元が要求を行うのに必要なサーバーの役割を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>GetSearchableMailboxes 操作要求の例: 配布グループに関する情報を要求する

**GetSearchableMailboxes** 操作要求の次の例は、lolgroup 配布グループのメールボックス情報を取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文には、次の要素が含まれています。
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)   
- [SearchFilter](searchfilter.md)    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>GetSearchableMailboxes 操作の応答の成功: 配布グループに関する情報を取得する

次の例は、Lolgroup 配布グループの検出情報を取得する **GetSearchableMailboxes** 操作要求に対する正常な応答を示しています。 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)   
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)   
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (string)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>GetSearchableMailboxes 操作の応答の成功: 展開された配布グループに関する情報を取得する

次の例は、展開された lolgroup 配布グループのメンバーに関する検出情報を取得する **GetSearchableMailboxes** 操作要求に対する正常な応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)    
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)    
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (string)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>GetSearchableMailboxes 操作エラー応答

次の例は **、GetSearchableMailboxes** 操作要求に対するエラー応答を示しています。 これは **、ExpandGroupMembership** 引数が true に設定されている場合に、すべての検索可能なメールボックスを取得する要求に対する **応答です**。 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)  
- [MessageText](messagetext.md)   
- [ResponseCode](responsecode.md)   
- [DescriptiveLinkKey](descriptivelinkkey.md) 
- [SearchableMailboxes](searchablemailboxes.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)   
- [SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)   
- [SearchMailboxes 操作](searchmailboxes-operation.md)   
- [GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md)    
- [GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md)   
- [GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)   
- [GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)
    

