---
title: RemoveImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: 操作 RemoveImGroup EWS についての情報を検索します。
ms.openlocfilehash: 85b312f0b156125a2d5395658ccea06d831abdde
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833097"
---
# <a name="removeimgroup-operation"></a>RemoveImGroup 操作

**RemoveImGroup** EWS の操作に関する情報を検索します。 
  
**RemoveImGroup**操作は、メールボックスからのインスタント メッセージング (IM) のグループは、1 つを削除します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-removeimgroup-operation"></a>RemoveImGroup 操作を使用します。

のみ、 **RemoveImGroup**操作は、1 つのグループ識別子の引数を取る。 
  
### <a name="removeimgroup-operation-soap-headers"></a>RemoveImGroup 操作の SOAP ヘッダー

**RemoveImGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a>RemoveImGroup 操作の要求の例

**RemoveImGroup**操作要求の次の例では、IM グループを削除する方法を示します。 
  
> [!NOTE]
> グループ ID が小さすぎると読みやすさを保持します。 
  
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
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [RemoveImGroup](removeimgroup.md)
    
- [グループ Id](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a>RemoveImGroup 操作の成功の応答

成功した要求への応答、 **RemoveImGroup**操作の例を次に示します。 
  
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
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a>RemoveImGroup 操作エラー応答の ErrorInvalidImGroupId

**RemoveImGroup**操作の要求に対してエラー応答の例を次に示します。 次のエラー応答は、メールボックス内に存在しないグループを削除しようとしましたがときに発生します。 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a>RemoveImGroup 操作エラー応答の ErrorInvalidIdMalformed

**RemoveImGroup**操作の要求に対してエラー応答の例を次に示します。 次のエラー応答は、誤った形式のグループ識別子を持つグループを削除しようとしましたがときに発生します。 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 内の EWS のユーザーと連絡先](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [AddImGroup 操作](addimgroup-operation.md)
    
- [SetImGroup 操作](setimgroup-operation.md)
    

