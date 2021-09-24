---
title: RemoveContactFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: RemoveContactFromImList EWS 操作に関する情報を検索します。
ms.openlocfilehash: cc72dc1b0abf9032fabafbaac53d29f41968dafb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523587"
---
# <a name="removecontactfromimlist-operation"></a>RemoveContactFromImList 操作

**RemoveContactFromImList** EWS 操作に関する情報を検索します。 
  
**RemoveContactFromImList 操作では**、Lync が連絡先ストアに対して連絡先を使用するときに、Lync インスタント メッセージング (IM) リストから連絡先Exchange削除します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-removecontactfromimlist-operation"></a>RemoveContactFromImList 操作の使用

**RemoveContactFromImList** 操作は、連絡先サーバーに保存されている Lync 連絡先リストから削除する連絡先を識別する 1 つの引数Exchangeします。 この操作の対象となる連絡先の一覧は、2013 年に **Lync 連絡先** Outlookされます。 
  
> [!CAUTION]
> 連絡先リストから連絡先 [を削除するには、DeleteItem](deleteitem-operation.md) 操作を使用しない。 Lync 連絡先リストからの連絡先の削除をサポートするために、サーバー側の追加処理 **が必要になる場合** があります。 Lync 連絡先リスト **は、既定** の Lync 連絡先メールボックス フォルダーの概 **念に相当します** 。 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>RemoveContactFromImList 操作 SOAP ヘッダー

**RemoveContactFromImList 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC 3066「言語の識別用タグ」で定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>RemoveContactFromImList 操作要求の例: Lync 連絡先リストから連絡先を削除する

**RemoveContactFromImList** 操作要求の次の例は、Lync 連絡先リストから連絡先を削除 **する方法を示** しています。 **RemoveContactFromImList 操作は**、Lync 連絡先リストから削除された連絡先を識別する 1 つの一意の連絡先識別子 **を受け入** れます。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすさを維持するために短縮されています。 
  
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
    
## <a name="successful-removecontactfromimlist-operation-response"></a>成功した RemoveContactFromImList 操作応答

次の例は、Lync 連絡先リストから連絡先を削除する **RemoveContactFromImList** 操作要求に対する正常な応答 **を示** しています。 
  
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

次の例は **、RemoveContactFromImList** 操作要求に対するエラー応答を示しています。 これは、連絡先がリストに存在しなくなったときに Lync **連絡先** リストから連絡先を削除する要求に対する応答です。 
  
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

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [GetImItemList 操作](getimitemlist-operation.md)
    

