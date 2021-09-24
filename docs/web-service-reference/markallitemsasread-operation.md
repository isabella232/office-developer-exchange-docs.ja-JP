---
title: MarkAllItemsAsRead 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: MarkAllItemsAsRead EWS 操作に関する情報を検索します。
ms.openlocfilehash: 104eed826df2b8734aa3159c976a6e1f388c302f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519283"
---
# <a name="markallitemsasread-operation"></a>MarkAllItemsAsRead 操作

**MarkAllItemsAsRead** EWS 操作に関する情報を検索します。 
  
**MarkAllItemsAsRead** 操作は、すべてのアイテムが読み取りまたは未読かどうかを示すために、1 つ以上のフォルダー内のすべてのアイテムに [IsRead](isread.md)プロパティを設定します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-markallitemsasread-operation"></a>MarkAllItemsAsRead 操作の使用

**MarkAllItemsAsRead** 操作では、Exchange Web Services (EWS) フォルダー識別子または既定の Exchange フォルダー名で識別されるフォルダー内のすべてのアイテムに [IsRead](isread.md)プロパティを設定できます。 **MarkAllItemsAsRead** 操作では、読み取りとしてマークされたアイテムの読み取りレシートの送信を抑制できます。 
  
### <a name="markallitemsasread-operation-soap-headers"></a>MarkAllItemsAsRead 操作 SOAP ヘッダー

**MarkAllItemsAsRead** 操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC 3066「言語の識別用タグ」で定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a>MarkAllItemsAsRead 操作要求の例: フォルダー内のすべてのアイテムを読み取りとしてマークする

**MarkAllItemsAsRead** 操作要求の次の例は、フォルダー内のすべてのアイテムに対して [IsRead](isread.md)プロパティ (読み取りフラグとも呼ばれる) を **true** に設定する方法を示しています。 この例では、読み取り確認要求に応答して、読み取りレシートが送信されない場合も示しています。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすさを維持するために短縮されています。 この操作では、変更キーは必要ありません。 
  
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
    
## <a name="successful-markallitemsasread-operation-response"></a>MarkAllItemsAsRead 操作応答の成功

次の例は、フォルダー内のすべてのアイテムを読み取りとしてマークする **MarkAllItemsAsRead** 操作要求に対する正常な応答を示しています。 
  
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
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a>MarkAllItemsAsRead 操作要求の例: フォルダー内のすべてのアイテムを未読としてマークする

**MarkAllItemsAsRead** 操作要求の次の例は、フォルダー内のすべてのアイテムで [IsRead](isread.md)プロパティを **false** に設定する方法を示しています。 この例では、読み取り確認要求に応答して、読み取りレシートが送信されない場合も示しています。 
  
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

すべてのアイテムを読み取りとしてマークする要求に対する正常な応答は、すべてのアイテムを未読としてマークする要求に対する応答と同じです。
  
要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAllItemsAsRead](markallitemsasread.md)
    
- [ReadFlag](readflag.md)
    
- [SuppressReadReceipts](suppressreadreceipts.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a>MarkAllItemsAsRead 操作エラー応答

次の例は、メールボックス内にフォルダーが存在しない場合に、フォルダー内のすべてのアイテムを読み取りまたは未読としてマークする **MarkAllItemsAsRead** 操作要求に対するエラー応答を示しています。 
  
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

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [FindFolder 操作](findfolder-operation.md)
    

