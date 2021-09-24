---
title: GetPersona 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: GetPersona EWS 操作に関する情報を検索します。
ms.openlocfilehash: 47713ee42b7d726693efe91a5bc29c10f3aea91c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533554"
---
# <a name="getpersona-operation"></a>GetPersona 操作

**GetPersona** EWS 操作に関する情報を検索します。 
  
**GetPersona 操作** は、ペルソナに関連付けられているプロパティのセットを返します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getpersona-operation"></a>GetPersona 操作の使用

**GetPersona 操作では**、ペルソナの形式で集計された連絡先情報にアクセスできます。 要求 [の PersonaId](personaid.md) 要素は、応答で返すペルサを識別します。 応答には、ペルサ プロパティの既定のセットまたはカスタム プロパティ セットを含めることができます。 使用されていないプロパティが処理され、サーバーからクライアントに送信されないので、カスタム プロパティ セットを指定することをお勧めします。 
  
### <a name="getpersona-operation-soap-headers"></a>GetPersona 操作 SOAP ヘッダー

**GetPersona 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a>GetPersona 操作要求の例: ペルソナの既定のプロパティセットを返す

**GetPersona 操作要求の次の** 例は、ペルソナに関連付けられている既定のプロパティ セットを返す方法を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetPersona](getpersona.md)
    
- [PersonaId](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a>GetPersona 操作の正常な応答

次の例は **、GetPersona 操作要求に対する正常な応答を** 示しています。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすさを維持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- GetPersonaResponseMessage
    
- [ResponseCode](responsecode.md)
    
- [ユーザー](persona.md)
    
- [PersonaId](personaid.md)
    
- [PersonaType](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [FileAsId](fileasid.md)
    
- [GivenName](givenname.md)
    
- [姓](surname.md)
    
- [CompanyName](companyname.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Attribution (string)](attribution-string.md)
    
- [ID (String)](id-string.md)
    
- [SourceId](sourceid.md) SourceId 
    
- [DisplayName (string)](displayname-string.md)
    
- [IsWritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FolderId](folderid.md)
    
- [DisplayNames](displaynames.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [Value (ArrayOfStringValueType)](value-arrayofstringvaluetype.md)
    
- [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [FileAses](fileases.md)
    
- [FileAsIds](fileasids.md)
    
- [GivenNames](givennames.md)
    
- [Surnames](surnames.md)
    
- [MobilePhones](mobilephones.md)
    
- [PhoneNumberAttributedValue](phonenumberattributedvalue.md)
    
- [Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md)
    
- [数値](number.md)
    
- [型 (文字列)](type-string.md)
    
- [CompanyNames](companynames.md)
    
## <a name="getpersona-operation-error-response"></a>GetPersona 操作エラー応答

次の例は **、GetPersona 操作要求に対するエラー応答を** 示しています。 これは、誤って指定されたペルサ識別子を含む要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetPersonaResponseMessage](getpersonaresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [Exchange 内の EWS のユーザーと連絡先](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [FindPeople 操作](findpeople-operation.md)
    

