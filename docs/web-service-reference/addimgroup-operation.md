---
title: AddImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: 操作 AddImGroup EWS についての情報を検索します。
ms.openlocfilehash: 91236f9ad2236b3f6bee600b9d57bcf736090ed7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759283"
---
# <a name="addimgroup-operation"></a>AddImGroup 操作

**AddImGroup** EWS の操作に関する情報を検索します。 
  
**AddImGroup** Exchange Web サービス (EWS) の操作は、メールボックスに、新しいインスタント メッセージング (IM) グループを追加します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-addimgroup-operation"></a>AddImGroup 操作を使用します。

**AddImGroup**操作には、単一の表示名の引数はわずかです。 
  
この操作は、表示名、グループの種類、および新しいグループの Exchange ストアの識別子を返します。
  
**AddImGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
**表 1 です。AddImGroup 操作の SOAP ヘッダー**

|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 これは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 これは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 これは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 これは、応答に適用されます。  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>AddImGroup 操作の要求の例: IM グループの新規作成

**AddImGroup**操作要求の次の例では、MyCustomerGroup という名前の IM グループを作成する方法を示します。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [AddImGroup](addimgroup.md)
    
- [表示名 (文字列)](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a>AddImGroup 操作の成功の応答

**AddImGroup**操作の要求に正常な応答の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [AddImGroupResponse](addimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [表示名 (文字列)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>AddImGroup 操作のエラー応答

**AddImGroup**操作要求に対するエラー応答の例を次に示します。 これは、表示名に使用できない文字が含まれる要求への応答です。 これが SOAP フォールトとスキーマ ・ ベースのエラー メッセージではないことに注意してください。 要求で送信される表示名は、~! @# $% ^&amp;でエラーが発生し、&amp;の文字。 &amp;要求ペイロードの 11 行と 33rd の文字の文字が発生しました。 HTTP 500 コードで応答が返されました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>関連項目

- [Exchange 内の EWS のユーザーと連絡先](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [RemoveImGroup 操作](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

