---
title: RemoveContactFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: 操作 RemoveContactFromImList EWS についての情報を検索します。
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833080"
---
# <a name="removecontactfromimlist-operation"></a>RemoveContactFromImList 操作

**RemoveContactFromImList** EWS の操作に関する情報を検索します。 
  
**RemoveContactFromImList**操作は、Lync は、連絡先ストアの Exchange を使用すると、Lync のインスタント メッセージング (IM) の一覧から連絡先を削除します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-removecontactfromimlist-operation"></a>RemoveContactFromImList 操作を使用します。

**RemoveContactFromImList**操作は、Exchange サーバーに格納されている Lync 連絡先リストから削除するメンバーを識別する 1 つの引数を受け取ります。 この操作のターゲットがという名前の**Lync 連絡先**Outlook 2013 で連絡先の一覧です。 
  
> [!CAUTION]
> 連絡先リストから連絡先を削除するのには、 [DeleteItem の操作](deleteitem-operation.md)を使用しません。 追加のサーバー側の処理では、 **Lync の連絡先**リストから連絡先を削除することをサポートするために発生する必要があります。 **Lync の連絡先**の一覧は、既定の**Lync の連絡先**のメールボックス フォルダーの概念と同じであることを注意してください。 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>RemoveContactFromImList 操作の SOAP ヘッダー

**RemoveContactFromImList**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>RemoveContactFromImList 操作の要求の例: Lync の連絡先リストから連絡先を削除します。

**RemoveContactFromImList**操作要求の次の例では、 **Lync の連絡先**リストから連絡先を削除する方法を示します。 **RemoveContactFromImList**操作では、 **Lync の連絡先**の一覧から削除された連絡先を識別する 1 つ固有連絡先 id を受け入れます。 
  
> [!NOTE]
> すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

次の要素は、SOAP 本文の要求で使用されます。
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>RemoveContactFromImList 操作の成功の応答

次の例では、 **Lync の連絡先**リストから連絡先を削除するのには、 **RemoveContactFromImList**操作の要求に正常な応答を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文では、次の要素が使用されます。
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>RemoveContactFromImList 操作のエラー応答

**RemoveContactFromImList**操作の要求に対してエラー応答の例を次に示します。 これは、連絡先が一覧に存在しない場合は、 **Lync の連絡先**リストから連絡先を削除する要求に応答します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [GetImItemList 操作](getimitemlist-operation.md)
    

