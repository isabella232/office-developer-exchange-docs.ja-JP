---
title: GetSearchableMailboxes 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: 操作 GetSearchableMailboxes EWS についての情報を検索します。
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760852"
---
# <a name="getsearchablemailboxes-operation"></a>GetSearchableMailboxes 操作

**GetSearchableMailboxes** EWS の操作に関する情報を検索します。 
  
**GetSearchableMailboxes**操作は、スコープ指定された検索の検索可能なメールボックスのセットを取得します。 応答で返されるメールボックスを検索可能なスコープは、検索フィルターと配布グループのメンバーシップを展開するかどうかによって決まります。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getsearchablemailboxes-operation"></a>GetSearchableMailboxes 操作を使用します。

**GetSearchableMailboxes**操作は、検索可能なメールボックスに関する情報を取得します。 要求では、次の引数を渡すことができます。 
  
- [SearchFilter](searchfilter.md) : 引数として 1 つの電子メールのエイリアスを受け入れます。 
    
- [ExpandGroupMembership](expandgroupmembership.md)応答で返される結果の配布グループのメンバーシップを展開するかどうかを示します。 
    
検索フィルターに設定する電子メール エイリアスは、配布グループと配布グループのメンバーシップは展開されませんが、応答には、配布グループのメールボックスの情報が含まれます。 検索フィルターに設定する電子メール エイリアスは、配布グループと配布グループのメンバーシップが展開されている、応答には、配布グループのメンバーである各メールボックスのメールボックスの情報が含まれます。 検索フィルターには、単一のユーザーのエイリアスが含まれています、応答で 1 つのユーザーのメールボックス情報が含まれます。 [GetSearchableMailboxes](getsearchablemailboxes.md)要素が空の場合、応答は検索可能なすべてのメールボックスに格納されます。 これは、空の[SearchFilter](searchfilter.md)要素と[ExpandGroupMembership](expandgroupmembership.md)要素が**false**に設定することと同じです。
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>GetSearchableMailboxes 操作の SOAP ヘッダー

**GetSearchableMailboxes**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |呼び出し元が要求を行うために必要とされるサーバーの役割を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>GetSearchableMailboxes 操作の要求の例: 配布グループに関する情報を要求

**GetSearchableMailboxes**操作要求の次の例では、lolgroup の配布グループのメールボックス情報を取得する方法を示します。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchFilter](searchfilter.md)
    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>GetSearchableMailboxes 操作の成功の応答: 配布グループに関する情報を取得します。

Lolgroup の配布グループの検出情報を取得する**GetSearchableMailboxes**操作要求に正常な応答の例を次に示します。 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
- [表示名 (文字列)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [参照 id が](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>GetSearchableMailboxes 操作の成功の応答: 展開された配布グループに関する情報を取得します。

検出の lolgroup が展開された配布グループのメンバー情報を取得する**GetSearchableMailboxes**操作の要求に正常な応答の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
- [表示名 (文字列)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [参照 id が](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>GetSearchableMailboxes 操作のエラー応答

**GetSearchableMailboxes**操作の要求に対してエラー応答の例を次に示します。 これは、 **ExpandGroupMembership**引数が**true**に設定すると、検索可能なすべてのメールボックスを取得する要求に応答します。 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)
    
- [SearchMailboxes 操作](searchmailboxes-operation.md)
    
- [GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md)
    
- [GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md)
    
- [GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)
    
- [GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)
    

