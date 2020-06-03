---
title: MarkAllItemsAsRead 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: MarkAllItemsAsRead EWS 操作に関する情報を検索します。
ms.openlocfilehash: aeeacea1cd5eed723f93027dd1ef75b34605fdfd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530531"
---
# <a name="markallitemsasread-operation"></a>MarkAllItemsAsRead 操作

**Markallitemsasread** EWS 操作に関する情報を検索します。 
  
**Markallitemsasread**操作は、すべてのアイテムが開封済みまたは未読であることを示すために、1つまたは複数のフォルダー内のすべてのアイテムに対する[isread](isread.md)プロパティを設定します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-markallitemsasread-operation"></a>MarkAllItemsAsRead 操作の使用

**Markallitemsasread**操作は、Exchange Web サービス (EWS) フォルダー識別子または既定の exchange フォルダー名のいずれかによって識別されるフォルダー内のすべてのアイテムに対して[isread](isread.md)プロパティを設定できます。 **Markallitemsasread**操作によって、開封済みとしてマークされたアイテムの開封確認メッセージの送信を抑制することもできます。 
  
### <a name="markallitemsasread-operation-soap-headers"></a>MarkAllItemsAsRead operation SOAP ヘッダー

**Markallitemsasread**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a>MarkAllItemsAsRead operation 要求の例: フォルダー内のすべてのアイテムを既読にします。

**Markallitemsasread**操作要求の次の例は、フォルダー内のすべてのアイテムに対して、 [isread](isread.md)プロパティ (read フラグとも呼ばれます) を**true**に設定する方法を示しています。 この例では、開封確認要求に対する応答で開封確認が送信されないことも示しています。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。 この操作では、キーを変更する必要はありません。 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAllItemsAsRead](markallitemsasread.md)
    
- [ReadFlag](readflag.md)
    
- [SuppressReadReceipts](suppressreadreceipts.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a>Successful MarkAllItemsAsRead operation 応答

次の例は、フォルダー内のすべてのアイテムを開封済みとしてマークするために、 **Markallitemsasread**操作要求に対する正常な応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [MarkAllItemsAsReadResponse](markallitemsasreadresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAllItemsAsReadResponseMessage](markallitemsasreadresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a>MarkAllItemsAsRead operation 要求の例: フォルダー内のすべてのアイテムを未読としてマークします

次の**Markallitemsasread**操作要求の例は、フォルダー内のすべてのアイテムで[isread](isread.md)プロパティを**false**に設定する方法を示しています。 この例では、開封確認要求に対する応答で開封確認が送信されないことも示しています。 
  
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
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

すべてのアイテムを開封済みとしてマークする要求に対する正常な応答は、すべてのアイテムを未読としてマークする要求に対する応答と同じです。
  
要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAllItemsAsRead](markallitemsasread.md)
    
- [ReadFlag](readflag.md)
    
- [SuppressReadReceipts](suppressreadreceipts.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a>MarkAllItemsAsRead 操作エラー応答

次の例は、フォルダーがメールボックス内に存在しない場合に、フォルダー内のすべてのアイテムに開封済みまたは未読マークを付けるための、 **Markallitemsasread**操作要求へのエラー応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [MarkAllItemsAsReadResponse](markallitemsasreadresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAllItemsAsReadResponseMessage](markallitemsasreadresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [FindFolder 操作](findfolder-operation.md)
    

