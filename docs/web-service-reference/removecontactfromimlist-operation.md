---
title: RemoveContactFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: RemoveContactFromImList EWS 操作についての情報を検索します。
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458468"
---
# <a name="removecontactfromimlist-operation"></a>RemoveContactFromImList 操作

**RemoveContactFromImList** EWS 操作についての情報を検索します。 
  
**RemoveContactFromImList**操作は、lync が連絡先ストアに対して Exchange を使用している場合に、lync インスタントメッセージング (IM) リストから連絡先を削除します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-removecontactfromimlist-operation"></a>RemoveContactFromImList 操作の使用

**RemoveContactFromImList**操作は、Exchange サーバーに格納されている Lync 連絡先リストから削除する連絡先を識別する1つの引数を受け取ります。 この操作対象の連絡先の一覧は、Outlook 2013 では**Lync 連絡先**と呼ばれます。 
  
> [!CAUTION]
> 連絡先リストから連絡先を削除する場合は、 [DeleteItem 操作](deleteitem-operation.md)を使用しないでください。 **Lync 連絡先**リストから連絡先を削除できるようにするには、追加のサーバー側処理が必要になることがあります。 **Lync 連絡先**リストは、既定の**lync 連絡先**メールボックスフォルダーに相当する概念であることに注意してください。 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>RemoveContactFromImList 操作の SOAP ヘッダー

**RemoveContactFromImList**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>RemoveContactFromImList 操作要求の例: Lync 連絡先リストから連絡先を削除します。

次の**RemoveContactFromImList**操作要求の例は、 **Lync 連絡先**リストから連絡先を削除する方法を示しています。 **RemoveContactFromImList**操作は、 **Lync の連絡先**リストから削除された連絡先を識別するための一意の連絡先識別子を1つだけ受け入れます。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文では、次の要素が使用されます。
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>成功した RemoveContactFromImList 操作の応答

次の例は、 **RemoveContactFromImList**操作要求に対する正常な応答を示しています。これは、 **Lync 連絡先**リストから連絡先を削除することです。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文では、次の要素が使用されます。
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>RemoveContactFromImList 操作エラー応答

次の例は、 **RemoveContactFromImList**操作要求へのエラー応答を示しています。 これは、連絡先がリストに存在しなくなったときに、 **Lync の連絡先**リストから連絡先を削除する要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本文では、次の要素が使用されます。
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [GetImItemList 操作](getimitemlist-operation.md)
    

